---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/filters/generators/decal.html"
breadcrumb-title: ''
description: 使用 Substance 3D Sampler 中的貼花產生器來建立貼花圖案和材質表面的疊加貼圖。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Decal
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 貼花/印花
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 1%

---


# 貼花/印花

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-decal-18-n-d.png)

**收錄於：** 《發電機》

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

貼花過濾器允許你在特定位置新增其他材質的實例。 這對於添加像貼紙或某些程序生成不容易的細節很有用。

下方圖片顯示 **貼紙過濾器** 被用來對混凝土造成損害。

![](../../assets/3d-2d-filters-cropped-0045-decal-in.jpg)

貼貼貼紙前，混凝土底層是乾淨且未受損的。

![](../../assets/3d-2d-filters-cropped-0044-decal-out.jpg)

貼 **上貼紙濾鏡** 後，材質會增加真實的裂紋與損傷。

</td>
</tr>
</table>

## 參數

**基本參數**

* **平鋪模式**：\
  決定是否要在 2D 視圖&#x200B;**中鋪**&#x200B;設把手之外的平板。\
  H代表水平，V代表垂直。
* **底料顏色比賽**：0-1\
  調整貼紙材質的顏色，使其與下方層的顏色相符。
* **一般混合模式**：\
  調整貼花材質與底層之間法線的混合方式
* **正常不透明度混合**：0-1\
  改變貼紙材質法線的不透明度
* **貼紙高度位置**：0-1\
  調整貼紙相對於底層高度的高度
* **貼紙高度刻度**：0-1\
  改變貼花材質高度圖的對比度

**進階參數**

* **貼紙變換**：\
  調整貼花的矩陣轉換值。 一般來說，直接用 2D 視角&#x200B;**的把**&#x200B;手來調整貼紙的轉換會比較簡單。
* **貼紙**&#x200B;**偏移**：-1 比 1\
  調整貼紙的偏移量。

## 使用指南

使用貼紙濾鏡：

1. 把貼花濾波器加到你的圖層堆疊裡
1. 在貼紙層下方，會出現一個輸入槽
1. 把你的貼紙材質拖到貼紙層的輸入槽

你可以在 **屬性面板** 中選擇貼花層來調整濾鏡參數。

你可以在 **屬性面板** 中選擇輸入槽中的材質，調整貼紙輸入材質的參數。
