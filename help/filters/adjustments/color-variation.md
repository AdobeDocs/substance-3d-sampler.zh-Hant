---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/filters/adjustments/color-variation.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的色彩變化濾鏡，為材質增添色彩多樣性與變化，讓材質更自然。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Adjustments > Color Variation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 顏色變量
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 1%

---


# 顏色變量

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-colorpalette-18-n-d.png)

**收錄於：** 調整

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

色彩變化濾鏡允許你一次替換底色或漫射通道中的多種顏色。 這類似 **於色彩替換濾鏡**，但色彩 **變化** 能讓你在一個濾鏡中調整多種顏色，而 **色彩替換** 則讓你能更精確地控制替換顏色的遮罩，且可在多個頻道使用。

在下方圖片中， **色彩變化濾鏡** 不僅用來調整底層白色，使其呈現淡綠松石色，還能提升許多較小斑點的對比度。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0047-color-variation-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0046-color-variation-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## 參數

**基本參數**

* **顏色數量**：1-10\
  修改將取代通道顏色的顏色數量
* **亮度變化**：0-1\
  調整被替換顏色對亮度值的影響程度
* **分段**：\
  把用來套用顏色的遮罩放在另一個通道。
* **色彩選擇模式**：\
  選擇是手動選擇來源顏色還是自動。 若 **選擇手動** 選取模式，請 **在 2D 視圖** 中使用 handles 來選擇顏色。
  * **顯示文字助手**：切換\
    這個控制項只有在 **色彩選擇模式** 設為 **手動**&#x200B;時才會顯示。 啟用後，**顯示文字助手**&#x200B;會在 2D 視圖&#x200B;**的** handles 上加上文字標籤，讓 color selection handle 更輕鬆區分
* **顏色X**：顏色選擇\
  可用的色彩控制數量取決於色彩 **計數**&#x200B;所選的數值。 對每個顏色，選擇新的顏色來取代原本材質的顏色。

## 使用指南

**色彩變化濾鏡**&#x200B;讓你能快速修改基礎色彩通道的多個顏色。對某些材質來說，這有助於做些微調整，但 **色彩變化濾鏡** 最適合用單一濾鏡徹底改造材質的顏色。

使用 **色彩變化濾鏡**：

1. 將色彩變化濾鏡&#x200B;**加入**&#x200B;圖層堆疊
1. 用顏色數量&#x200B;**調整你想替換**&#x200B;的顏色數量。濾鏡會替換通道中的所有顏色—— **色彩計數** 控制可以讓你設定現有顏色要替換多少新顏色。
1. 可選擇&#x200B;**&#x200B;**&#x200B;分割或其他頻道作為顏色的基礎。例如，你可以選擇金屬通道，並使用 **手冊** >色彩選擇模式，將一個把柄放在黑色金屬值上，另一個把柄放在白色金屬值上。 透過這個設定，你可以分別控制材質中金屬和非金屬部分的顏色。
1. 選擇 **顏色選擇模式**。 開啟手動模式時，2D 視圖&#x200B;**中會出現**&#x200B;把手，讓你選擇新顏色會取代的原始基色。啟用 **顯示文字助手** ，以追蹤哪個帳柄連結到哪個顏色。
1. 用 **Color 1 到 10** 控制項修改色彩值。
1. 調整 **亮度變化** ，以調整顏色替換對亮度的影響程度。 使用低 **亮度變化**&#x200B;時，你可以完全壓平材質的顏色，或使用高 **亮度變化** 來保持原始顏色的細節。
