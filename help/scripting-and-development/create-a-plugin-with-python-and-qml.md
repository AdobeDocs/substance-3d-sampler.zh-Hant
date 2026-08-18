---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/scripting-and-development/create-a-plugin-with-python-and-qml.html"
breadcrumb-title: ''
description: 學習如何使用 Python 和 QML 為 Substance 3D Sampler 製作外掛，建立自訂使用者介面並擴充功能。
helpx_creative_field: ""
helpx_description: Sampler > Scripting and Development > Create a Plugin with Python and QML
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 用 Python 和 QML 建立外掛
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---


# 用 Python 和 QML 建立外掛

本指南說明如何用 Python 和 QML 建立一個簡單的自動儲存外掛。

## 插件結構

取樣器外掛至少需要一個 Python 和 QML 檔案才能匯入，但也可以包含其他檔案，例如用於外掛面板圖示的圖片。 以下範例中有三個檔案：

* **autosave.py** 包含外掛的邏輯並決定其運作方式。
* **autosave.qml** 定義了 Sampler 中外掛的外觀。
* **autosave.svg**&#x200B;是一個向量圖形，作為插件的圖示。

當你把插件所需的檔案集中在一個資料夾後，可以透過編輯>偏好設定>插件與腳本，將插件加入 Sampler。 想了解更多關於管理插件的資訊，請點此[&#128279;](manage-installed-plugins-and-scripts.md)。

## Python

以下程式碼是自動存檔外掛的完整 Python 檔案。 以下是程式碼的簡要說明，但程式碼中也包含包含更多資訊的註解：

1. 匯入相關模組。
   1. Qt 是一個多平台的 GUI 工具包。 QtcCore、QtQml 和 QtQuick 是我們用來在 autosave.py 與 autosave.qml 之間通訊的模組。
1. 定義一個方法 **save（），** 每 X 分鐘儲存一次專案。
1. 建立一個自動存檔類別。 這個類別指定 save（）**方法如何**&#x200B;連接到插件 UI，讓參數能改變插件的行為
1. 定義一個方法&#x200B;**暫存器\_qml\_type（）** 來執行外掛的設定。
1. 在 Sampler 裡面呼叫外掛。

### autosave.py

```
## Import QT & QML modules to create the UI

from PySide2 import QtCore, QtQml, QtQuick 

## Import Sampler API

import substance_sampler as ssa 

## Import other modules for this specific example

import datetime 

import os 

import threading 

 

 

## Save the project every X minutes

def save(interval): 

    global t 

    ssa.save_project() 

    if ssa.save_project(): 

        now = datetime.datetime.now() 

        print("Autosave: %d:%d:%d" % (now.hour, now.minute, now.second)) 

    t = threading.Timer(interval, save, [interval]) 

    t.start() 

 

 

t = None 

 

 

## Declare the API AutoSave

class AutoSave(QtQuick.QQuickItem): 

    def __init__(self, parent=None): 

        super(AutoSave, self).__init__(parent) 

 

## Declare a first API function

## This function can be called from the QML file

## with 2 arguments, one string and one integer

    @QtCore.Slot(str, int) 

    def start_auto_save(self, default_path, interval): 

        if not ssa.save_project(): 

            ssa.save_project_as(os.path.join(default_path, "autosave.ssa")) 

        global t 

        t = threading.Timer(10, save, [interval]) 

        t.start() 

        print("Launch Autosave") 

 

## Second function of the API

## With no argument

    @QtCore.Slot(None) 

    def stop_auto_save(self): 

        global t 

        t.cancel() 

        print("Stop Autosave") 

 

 

## Function to declare the API and the panel

## First argument is Python class of your API

## Second argument is name of the API you will use in the QML file

## Third and fourth is the API version. In this case, 1.0

## Last is the name of the panel in Sampler UI

def register_qml_type(): 

    QtQml.qmlRegisterType(AutoSave, "AutoSave", 1, 0, "AutoSave") 

 

 

## Execute the plugin in Sampler UI thread

ssa.run_in_main_thread(register_qml_type)
```


## QML

QML 檔案定義了外掛的使用者介面。 QML 代表 Qt 標記語言，其行為類似於 HTML 和 XML 等其他標記語言。 你可以 [在這裡](https://doc.qt.io/qt-6/qmlapplications.html#:~:text=QML%20is%20a%20user%20interface%20specification%20and%20programming,imperative%20JavaScript%20expressions%20combined%20with%20dynamic%20property%20bindings。)了解更多關於量子力學的資訊。

autosave.qml 的一般結構如下：

1. 匯入模組。
   1. 匯入的 Qt 模組是檔案中 UI 元素所必需的。
   1. autosave.py **建立**&#x200B;的自動儲存 API 類別也會被匯入。QML 檔案在第 20 行引用這個類別。
1. 建立需要追蹤的變數。
   1. **autoSaveFolder** 是取樣器檔案會自動儲存的資料夾。
   1. **時間是指** 自動存檔之間的秒數。
   1. **textColor** 的使用是為了讓外掛使用者介面中的文字顏色能在同一地點更新。
1. 實例化 Python API
1. 定義使用者介面。
   1. 這包括 autosave.py **創建**&#x200B;的 Python API 的掛鉤。例如：
      1. 第 47 行會在 QML 檔案中更新&#x200B;**&#x200B;**「Autosave every （min）：」元素時更新時序變數值。
      1. 第 64 行從 API 呼叫 **start\_auto\_save** 函式，並將 timing **和** autoSaveFolder **變數作為參數傳遞**。
1. 建立一個方法來清理預設的檔案路徑。

### autosave.qml

```
/* 

Import Qt modules to design the UI 

https://doc.qt.io/qt-5/qtqml-syntax-basics.html 

*/ 

import QtQuick 2.15 

import QtQuick.Controls 2.15 

import Qt.labs.platform 1.1 

import AutoSave 1.0 // Import API defined in the Python file 

 

Rectangle { 

  id: root 

  anchors.fill: parent 

  color: "#333333" 

 

  property var autoSaveFolder: removeQmlFilePathPrefix(StandardPaths.writableLocation(StandardPaths.DocumentsLocation)) 

  property var timing: 300 

  property var textColor: "#b3b3b3" 

 

  AutoSave { 

      id: api // Instantiate the Python API 

  } 

 

  Column { 

    id: controls 

    anchors.top: parent.top + 10 

    anchors.left: parent.left + 10 

    anchors.right: parent.right 

    width: parent.width 

    spacing: 20 

    leftPadding: 10 

    topPadding: 10 

 

    Column { 

        spacing: 5 

        Text { 

            id: timingTitle 

            text: "Autosave every (min): " 

            color: root.textColor 

        } 

        SpinBox { 

            id: timingControl 

            from: 1 

            to: 10 

            stepSize: 1 

            value: 5 

 

            onValueModified: ()=>{ 

                root.timing = timingControl.value * 60 

            } 

        } 

    } 

    Row { 

        Text { 

            text: "Off" 

            color: root.textColor 

            anchors.verticalCenter: toggle.verticalCenter 

        } 

        Switch { 

            id: toggle 

            checked: false 

 

            onClicked: ()=>{ 

                if (checked === true) { 

                    api.start_auto_save(root.autoSaveFolder, root.timing) // Call a function of the API with 2 arguments 

                } 

                else if (checked === false) { 

                    api.stop_auto_save() // Call a function of the API 

                } 

            } 

        } 

        Text { 

            text: "On" 

            color: root.textColor 

            anchors.verticalCenter: toggle.verticalCenter 

        } 

 

    } 

    Column { 

        spacing: 5 

        Text { 

            text: "Default Autosave Path" 

            color: root.textColor 

            } 

        Row { 

            id: folderInput 

            TextField { 

                id: folderText 

                text: root.autoSaveFolder 

                readOnly: true 

            } 

            Button { 

                id: folderSelection 

                text: qsTr("...") 

                width: 40 

                onClicked: ()=>{ 

                    folderDialog.open() 

                    } 

            } 

        } 

    } 

 

    FolderDialog { 

        id: folderDialog 

 

        onAccepted: ()=>{ 

            root.autoSaveFolder = removeQmlFilePathPrefix(folderDialog.currentFolder) 

        } 

    } 

 

  } 

      function qmlFilePathPrefix() { 

        if (Qt.platform.os === "windows") { 

            return "file:///" 

        } 

        return "file://" 

    } 

    function removeQmlFilePathPrefix(filePath) { 

        var prefix = qmlFilePathPrefix() 

        return filePath.toString().replace(prefix, '') 

    } 

}
```


## SVG

你可能已經注意到&#x200B;**autosave.svg**&#x200B;在 autosave.py **或** autosave.qml **中**&#x200B;都沒有明確提及或被提及。這是因為 Sampler 會尋找與 PY 檔案同名的 SVG 檔案，並自動將其作為插件圖示使用。

>[!NOTE]
>
> 如果你的插件資料夾中有檔名與 PY 檔不符的 SVG，你的插件就不會包含圖示。 這會讓你覺得外掛還沒出現在取樣器介面裡。 如果是這樣，將游標移到 Sampler 的右側列上方，選取你的插件。
> 
> 您的瀏覽器不支援 HTML5 影片元素

如果你的插件資料夾沒有 SVG 檔案，就會用預設的插件圖示來代替。

以下是你可以用來做上述自動存檔插件的 SVG 範例。

[autosave.svg](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/sadoc/files/234455541/234455542/1/1662460696349/autosave.svg)

## 自動存檔外掛的限制

上面建立的自動存檔插件是可行的，但並不完美。 例如，啟用自動存檔後調整自動存檔間隔，實際上不會改變兩次自動存檔之間的時間——你需要先停用再啟用自動存檔，UI 中的數值才會傳送到 API。

如果你是第一次同時使用 Python 和 QML，修正這個錯誤是建立理解外掛不同部分如何相互溝通的有用方法。
