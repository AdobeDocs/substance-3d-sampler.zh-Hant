---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/scripting-and-development/create-a-script-with-python.html"
breadcrumb-title: ''
description: 學習如何為 Substance 3D Sampler 撰寫 Python 腳本，以自動化工作流程並擴展應用程式功能。
helpx_creative_field: ""
helpx_description: Sampler > Scripting and Development > Create a Script with Python
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 用 Python 建立腳本
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---


# 用 Python 建立腳本

本指南說明如何用 Python 建立一個簡單的自動存檔外掛。

## 文字結構

腳本需要一個 PY 檔案才能匯入 Sampler。 你可以把下面的範例腳本存成 PY 檔，然後匯入到 Sampler。

## 範例文字

下面的腳本會自動為材質中的每一層選擇一個新的隨機種子，來產生不同的材質變化。 這有助於確保你的材料能在一般情況下使用，而非依賴特定的隨機種子。

### 隨機_seed\_variations.py

```
import substance_sampler as ssa 

from random import randrange 

 

## Get the current asset loaded in the layer stack

my_asset = ssa.get_selected_asset() 

 

## Create a list of all layers of the current asset

my_asset_layers = my_asset.get_layers() 

 

## Go through the layers list

for layer in my_asset_layers: 

## Go through all parameters of each layer

    for parameter in layer.parameters: 

## if the parameter is Random Seed, change is value

        if parameter.label == "$randomseed": 

            parameter.value = randrange(10000) 

            print(f"Random Seed for layer {layer.name}: {parameter.value}") 

 
```


上述程式碼包含註解，用以說明每行發生了什麼。

## 匯入腳本

當你把上面的腳本存成 PY 檔後，可以用編輯>偏好設定 > 插件和腳本匯入。 匯入後，**選單列中會出現「腳本」** 選項，與 **「檔案** 」和 **「編輯**」並列。 接著你可以執行腳本。

你可以在這裡[&#128279;](../manage-installed-plugins-and-scripts.md)了解更多關於管理你的劇本的資訊。
