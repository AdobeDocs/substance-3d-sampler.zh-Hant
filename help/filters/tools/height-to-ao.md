---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/filters/tools/height-to-ao.html"
breadcrumb-title: ''
description: 在 Substance 3D Sampler 中使用 Height to AO 工具，將高度圖轉換成環境遮蔽圖以製作材質。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Height to AO
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 高度至AO
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 1%

---


# 高度至AO

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-hbao-18-n-d.png)

**收錄於：** 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

從高度和法線資料產生環境遮蔽地圖。

請參見下方圖片中高度到AO濾波器的&#x200B;**結果**。

![](../../assets/3d-2d-filters-cropped-0025-height-to-ao-in.jpg)

在上方圖片中， **2D 視圖** 顯示高度圖。 這張圖片中沒有任何環境遮蔽資訊。

![](../../assets/3d-2d-filters-cropped-0024-height-to-ao-out.jpg)

在這張圖片中，環境&#x200B;**遮蔽貼圖是由 Height to AO 濾鏡**&#x200B;建立的，並在 2D 視圖&#x200B;**中可見**。環境遮蔽通常是細微的效果，所以在這材質裡不太容易看出來——試著用 **材質上的高度轉AO濾鏡** 來提升AO強度，並熟悉環境遮蔽的操作方式。

</td>
</tr>
</table>

## 參數

**基本參數**

* **模式**：\
  選擇是從高度通道、正常通道，或是兩個通道一起產生資料。
* **環境遮蔽 - 強度**：0-1\
  調整產生的AO資料強度
* **環境遮蔽 - 擴散**：0-1\
  調整產生的AO資料的半徑
