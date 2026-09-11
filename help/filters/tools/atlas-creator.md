---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/filters/tools/atlas-creator.html"
breadcrumb-title: ''
description: 使用 Substance 3D Sampler 中的 Atlas Creator 工具，從多張圖片中建立材質圖集，以高效組織材質。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Atlas Creator
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 地圖集創造者
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---


# 地圖集創造者

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-atlasgenerator-18-n-d.png)

**收錄於：** 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

**Atlas Creator** **篩選**&#x200B;器允許你將材質和圖片轉換成地圖集。接著你可以用其他濾鏡，比如 **Atlas Scatter** 和 **Atlas Splitter** ，在材質中加入 Atlas 元素。

下方圖片展示了一張叢林落葉圖譜， **記錄了圖譜**&#x200B;創作者處理前後的圖譜。

![](../../assets/3d-2d-filters-cropped-0041-atlas-creator-in.jpg)

在上方圖片中，一張圖集影像已被匯入並轉換成材質，但它仍不是圖集材質，因為不透明度貼圖沒有考慮個別元素。

![](../../assets/3d-2d-filters-cropped-0040-atlas-creator-out.jpg)

執行 **Atlas Creator** 後，會產生不透明度地圖，並在基礎色彩通道中填補圖集元素間的區域。

</td>
</tr>
</table>

參數

**基本參數**

* **移除小形狀**：0-1

  用這個來調整圖譜中物件的最小大小。 這對移除雜物很有用。
* **不透明度 - 色度影響**：0-2

  根據顏色值微調圖集元素的邊緣。
* **新增不透明度**：影像/筆刷

  匯入檔案當作遮罩，或用畫筆直接在 2D 視圖&#x200B;**中繪製本應不**&#x200B;透明的區域。

使用指南

## 準備圖集影像

在使用 **地圖集編輯器**&#x200B;篩選器之前，最好確保你的地圖集圖片是正確準備的。

**Atlas Creator** 是根據圖片的顏色來運作，並不考慮透明度。這表示準備圖集影像的最佳方法是確保元素間的空間是一致的黑白，這樣圖集創建&#x200B;**器就能更容易**&#x200B;產生不透明度遮罩。

## 從影像產生圖譜材料

**Atlas Creator** 的設計目的是將圖譜影像轉換成實體圖集。

1. 將你的原始影像匯入圖層堆疊。
1. 如果被要求選擇材質建立範本，請選擇「影像轉材質」。 否則，圖層堆疊中的圖片，在圖片上方加一個 **Image to Material（由 AI 驅動）濾鏡** 。
1. 等 **Image to Material** 濾鏡把你的原始影像轉換成材質。 調整參數直到你對結果滿意為止。
1. 把 Atlas Creator 過濾器&#x200B;**加**&#x200B;到圖層堆疊的頂端。
1. 調整地圖集生成器&#x200B;**的**&#x200B;參數，直到你對結果滿意為止。

1. 將圖片加入圖層堆疊。 若被要求選擇材質建立範本，請選擇 **「作為點陣圖**&#x200B;使用」。
1. 選取影像圖層後，在屬性面板中&#x200B;**將輸出使用**&#x200B;量改&#x200B;**為**&#x200B;基礎色&#x200B;**。**
1. 把地圖集創建&#x200B;**器加**&#x200B;到圖層堆疊的頂端。
1. 調整 Atlas Creator **的**&#x200B;參數直到你滿意為止——在 2D 視圖&#x200B;**中查看不透明度通道**，能更清楚地看到濾鏡結果。
1. 使用 **匯出面板** 來匯出產生的頻道。
