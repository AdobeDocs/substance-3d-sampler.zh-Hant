---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/filters/tools/make-it-tile.html"
breadcrumb-title: ''
description: 在 Substance 3D Sampler 中使用 Make it Tile 工具，自動從非平鋪材質中創造無縫的平鋪圖案。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Make it Tile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 做成瓷磚
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---


# 做成瓷磚

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-tiling-18-n-d.png)

**收錄於：** 《發電機》

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

使用 **「製作圖塊」篩選器** ，讓你的材質可以平鋪。 **平鋪濾鏡**&#x200B;也會讓你的材質可以平鋪，但每個濾鏡的運作方式都不同。如果你發現 **Make it Tile 過濾器** 不適合你，可以試試 **Tiling 過濾器**。

在下面的圖片中，你可以看到 Make it Tile 過濾器&#x200B;**如何**&#x200B;將非拼貼材質轉換成可鋪磚材質。這種材質鋪得很好，因為它遵循格子狀圖案，沒有特定點會吸引焦點。

![](../../assets/3d-2d-filters-cropped-0015-make-it-tile-in.jpg)

在上方圖片中，紅線顯示了材料的邊界。 很明顯有一條很強的接縫，而且這種材料不適合鋪磚。

![](../../assets/3d-2d-filters-cropped-0014-make-it-tile-out.jpg)

經過 **Make it Tile** 後，這種材質鋪得很好，沒有紅線的話，根本看不到材料邊界的接縫。

</td>
</tr>
</table>

## 參數

**基本參數**

* **門檻**：0-1\
  調整尺寸和最上層的匹配度。
* **平滑度**：0-1\
  將最上層的接縫磨平。
* **比分**：0-1\
  調整接縫的對比度。 降低對比度的效果和模糊接縫是一樣的。
* **斑點移除**：切換\
  啟用後，濾波器會嘗試去除頂層與底層接縫附近的雜訊。
* **色彩均衡器**：0-50\
  平衡色彩值以降低接縫的可見度。
* **身高匹配**：\
  改變濾鏡頂層和底層的高度貼圖混合方式。 想更清楚地看到結果，請在 2D 視圖&#x200B;**中查看高度通道**。請注意，高度匹配不會影響除高度通道外的其他通道，因此法線與 AO 不會因高度匹配的變更而受影響。

**進階參數**

* **色度影響**：0-1\
  調整顏色值對接縫的影響程度。
* **面具倒置**：切換\
  把頂層和底層的遮罩反轉。
* **高度匹配平滑度**：0-16\
  調整上下層高度的模糊度。
* **左右音色來源**：-1 到 1\
  調整左右音色的來源位置。
* **上下補丁來源**：-1比1\
  調整頂部和底部補丁的來源位置。

## 使用指南

**Make it Tile** **濾鏡**&#x200B;是透過將多份材質疊加在一起來運作的。

下方圖片顯示了圖層的配置：

* 綠色邊界顯示了 **Make it Tile 濾鏡所產生材料的邊緣**
* 紅線顯示底層的邊界。 底層在 X 軸和 Y 軸上被 50% 的 UV 空間偏移，所以紅線是需要覆蓋的平鋪接縫。
* 藍色方形和半圓形覆蓋紅色接縫。 濾鏡的參數允許你調整藍色形狀的邊界，確保紅色接縫不被看見，同時保持藍色接縫盡可能平滑。

![](../../assets/makeittilediagram.png){width="512px"}

左右半圓彼此匹配，確保材料磚是水平排列的，上下的半圓形則確保材料磚垂直排列。 中央的藍色方塊會移除所有剩餘的接縫，形成完全可拼貼且無接縫的材質。
