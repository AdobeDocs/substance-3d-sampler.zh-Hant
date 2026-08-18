---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/filters/hdri-tools/hdr-merge.html"
breadcrumb-title: ''
description: 使用 Substance 3D Sampler 中的 HDR 合併工具，將多重曝光影像合併成一張高動態範圍影像。
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > HDR Merge
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: HDR 合併
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---


# HDR 合併

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/S_HDRMerge_18_N_D.png)

**收錄於：** HDRI 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

**HDR 合併**&#x200B;**濾鏡**&#x200B;允許你將一組 SDR（標準動態範圍）影像合併成 HDR 影像。

下方圖片展示了 HDR 合併&#x200B;**的**&#x200B;結果。

![](../../assets/3d-2d-filters-cropped-0027-hdr-merge-in.jpg)

在完成 HDR 合併&#x200B;**之前**，3D 視角&#x200B;**中的**&#x200B;球體會反射預設環境光。**2D 視圖**&#x200B;預設顯示第一張掃描影像的匯入影像資料，此處為曝光最低的影像。

![](../../assets/3d-2d-filters-cropped-0026-hdr-merge-out.jpg)

加入 HDR 合併&#x200B;**&#x200B;**&#x200B;濾鏡&#x200B;**後**，球體會反射一個新的環境光——由輸入影像生成的 HDR 影像。

</td>
</tr>
</table>

## TParameters

**基本參數**

* **輸入曝光差（EV）：** 0-2\
  設定最高與最低輸入曝光的曝光差。 高曝光的 delta 會增加合併操作的對比度。
* **輸出自動曝光**：切換\
  啟用或關閉自動曝光調整。
* **輸出曝光偏移（EV）：**-5 到 5\
  抵銷曝光度。

## 使用指南

觀看這段影片，了解如何使用 **HDR 合併濾鏡** ，以及其他有助於將 SDR 影像轉換成 HDR 環境燈光的濾鏡。

使用 **HDR 合併**&#x200B;**濾鏡**&#x200B;的基本步驟如下：

1. 匯入要合併到圖層堆疊的圖片集合。
1. 把 **HDR 合併濾鏡** 加到圖層堆疊裡。
1. 修改參數以確保曝光值正確。
