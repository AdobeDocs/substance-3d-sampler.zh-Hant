---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/scripting-and-development/manage-installed-plugins-and-scripts.html"
breadcrumb-title: ''
description: 學習如何在 Substance 3D Sampler 中管理已安裝的外掛和腳本，以安裝、修改及移除自訂擴充功能。
helpx_creative_field: ""
helpx_description: Sampler > Scripting and Development > Manage installed plugins and scripts
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 管理已安裝的外掛與腳本
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---


# 管理已安裝的外掛與腳本

要安裝、修改或移除外掛，請使用編輯>偏好設定，然後選擇外掛與腳本。

![](../assets/preferences-86.png)

從 Plugins and Scripts 面板可以啟用 Log 面板，顯示插件的輸出。 這對故障排除和除錯很有幫助。 啟用後，你可以從 Sampler 主介面右側欄開啟日誌面板。 Log面板可以像其他取樣面板一樣對接。

## 插件與腳本的比較

外掛和腳本的主要差異在於外掛包含 UI 元素，而腳本沒有。 插件至少需要一個 PY 和一個 QML 檔案。 QML 檔案定義使用者介面元素，PY 檔案則定義外掛的行為。 而腳本則僅包含一個 PY 檔案。

插件的 UI 元素意味著可以透過參數來修改插件的行為。 舉例來說，範例自動存檔外掛有控制項可以調整自動存檔之間的時間。 插件會成為取樣器介面的一部分，可以像標準取樣器面板一樣停靠和移動。

腳本不允許這種彈性，而是執行特定任務。 例如，每次呼叫 Export all 腳本時都會以相同方式運作。 腳本可從上方選單列存取——腳本選單只有在 Sampler 新增腳本後才會開放。

## 管理外掛

預設情況下，唯一可用的選項是「新增外掛」。 這會開啟檔案總管，你可以選擇一個 PY 檔案來載入。

![](../assets/manageplugins.png)

>[!NOTE]
>
> 外掛需要同時有 PY 和 QML 檔案才能運作。 當你選擇要匯入的 PY 檔案時，Sampler 會搜尋該資料夾中的 QML 檔案。 如果找不到 QML 檔案，插件載入將失敗。

安裝外掛後，會有幾個選項可用：

* 插件可以透過拖動插件左側的握柄來重新排序。
* 用切換開關開關開啟或關閉插件。
* 使用每個插件右側的選單按鈕來重新載入、移除或開啟該插件的資料夾位置。

已安裝的外掛最初會顯示在 Sampler 主介面的右側列。 接著你可以像標準取樣器面板一樣開啟、停靠並移動插件面板。

## 管理腳本

腳本可以像外掛一樣管理。

![](../assets/managescripts.png)

一旦安裝腳本，會有幾個選項可供選擇：

* 把handle放在腳本左側的腳本重新排序。
* 用切換開關開關切換腳本。
* 使用每個腳本右側的選單按鈕移除腳本，或打開腳本的資料夾位置。
* 匯入後，腳本會被複製到 **%\AppData\Roaming\Adobe\Adobe Substance 3D Sampler\scripts**
* 要編輯腳本，你應該修改 Sampler 複製的那個腳本
