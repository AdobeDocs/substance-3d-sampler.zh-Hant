---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/hdri-tools/exposure-preview.html"
breadcrumb-title: ''
description: 在 Substance 3D Sampler 中使用曝光預覽工具，在 HDRI 影像中預覽曝光調整，再進行修改。
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > Exposure Preview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 曝光預覽
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---


# 曝光預覽

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-exposurepreview-18-n-d.png)

**收錄於：** HDRI 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

**曝光預覽****濾鏡**&#x200B;讓你能快速預覽一系列曝光值。

下面你可以看看曝光預覽濾鏡&#x200B;**的作用**。

![](../../assets/3d-2d-filters-cropped-0029-exposure-preview-in.jpg)

在上方圖片中，環境光已經建立，HDR 影像資料在 2D 視圖&#x200B;**中可見**。

![](../../assets/filters-cropped-0028-exposure-preview-out.jpg)

隨著&#x200B;**層層堆疊中新增曝光預覽****濾鏡**，新增一個通道——環境診斷（Environment Diagnostics），可顯示不同曝光下的環境光源。

</td>
</tr>
</table>

## 參數

**基本參數**

* **最小曝光（EV）：**-8 到 8\
  設定曝光曝光率為曝光最少的影像。
* **最大曝光（EV）：**-8 到 8\
  設定曝光曝光率最高的影像。

## 使用指南

**曝光預覽濾鏡**&#x200B;的運作方式與其他取樣濾鏡略有不同。這是一個幫助你找到環境光源正確曝光的工具，但它實際上並不影響環境通道——相反地，當你將&#x200B;**曝光預覽濾鏡**&#x200B;加入圖層堆疊時，2D 視圖&#x200B;**中會多一個通道可供觀看**——環境診斷通道。

如果你查看環境診斷頻道，應該能看到幾個不同曝光值下的 2D 環境影像實例。 調整曝光預覽濾鏡&#x200B;**的**&#x200B;參數，以改變環境診斷頻道中可見的曝光範圍。
