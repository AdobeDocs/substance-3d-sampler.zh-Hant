---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/getting-started/export/managing-custom-presets.html"
breadcrumb-title: ''
description: 學習如何在 Substance 3D Sampler 中使用 Substance Designer 建立並編輯自訂匯出預設，以優化工作流程。
helpx_creative_field: ""
helpx_description: Sampler > Getting Started > Export > Managing custom presets
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 建立與編輯自訂預設
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# 建立與編輯自訂預設

可以用 Substance 3D Designer 建立自訂預設。

建立自訂預設與為 Sampler 建立自訂濾波器相同規則。 相關文件可在此[&#128279;](../../filters/custom-filters.md)取得。

## 成立

## 建立圖表

打開 Substance Designer 並建立一個新的 Substance 圖表。

打開圖屬性並填寫以下必填資訊：

* 標籤：輸入你在取樣器介面中會使用的自訂預設名稱
* 使用者資料： <b>alchemist：：type=filter</b>

## 輸入與輸出的定義

### 輸入

輸入代表你想在匯出前轉換的材質通道。

為每個材質通道建立一個輸入色彩節點（或灰階），並在每個輸入節點的屬性中使用中加入<b></b>，確保材質與自訂預設之間有連結。

範例：基底色彩輸入的定義

![](../../assets/custom-input.png){width="600px"}

### 輸出

輸出代表你材質匯出的結果。

每個材質建立一個輸出節點，並在每個輸出節點的屬性中加入 <b>使用量</b> 和 <b>標籤</b> 。 標籤<b></b>會顯示在匯出器視窗的通道清單中，以及你的材質檔案名稱中。

範例：自訂材質色彩不透明度的定義

![](../../assets/custom-output.png){width="600px"}

#### 通道包裝與通道轉換的範例

將三個灰階通道打包在一個 RGB 材質中：

![](../../assets/channel-packing-example.png){width="600px"}

從 PBR 金屬/粗糙感轉換為 PBR 高光/光澤：

![](../../assets/channel-conversion.png){width="600px"}

## 匯入

要匯入你的新預設：

1. 點擊<b>預設下拉選單</b>右側<b>的管理預設</b>按鈕。
1. 請使用<b>預設列表</b>底部<b>的匯入預設</b>按鈕。

![](../../assets/Managing-presets-Dropdown.png.img.png){width="400px"}
