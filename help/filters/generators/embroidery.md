---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/generators/embroidery.html"
breadcrumb-title: ''
description: 使用 Substance 3D Sampler 中的刺繡產生器，為材料製作刺繡布料圖案和縫線紋理。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Embroidery
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 刺繡
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---


# 刺繡

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-embroidery-18-n-d.png)

**收錄於：** 《發電機》

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

刺繡濾鏡讓你能快速將圖片轉換成刺繡版塊。 你可以自訂補丁的外觀，並利用色彩管理工具作為多種材質的遮罩。

下方圖片展示了 **刺繡濾鏡** 的運作。

![](../../assets/3d-2d-filters-cropped-0035-embroidery-in.jpg)

在上方圖片中，原始圖片已被匯入。 請注意，影像是不透明的，背景是白色的。

![](../../assets/3d-2d-filters-cropped-0034-embroidery-out.jpg)

在上方圖片中， **刺繡濾鏡** 已加入圖層堆疊，並將原始圖片轉換成刺繡版塊。 請注意，雖然原始影像是不透明的，但刺繡濾鏡&#x200B;**的輸出**&#x200B;是透明的。

</td>
</tr>
</table>

## 田島刺繡插件

有興趣試用田島刺繡插件嗎？ \
點此[&#128279;](../../pipeline-and-integrations/tajima-exporter-plugin.md)了解更多資訊。

## 參數

<b>基本參數</b>

* <b>隨機種子</b>：\
  這個隨機種子，而這個過濾器中所有其他隨機參數都是基於它。
* <b>圖片</b>來源：image/mask\
  從你的系統中選擇一張圖片，或是繪製一個自訂遮罩。
* <b>顏色數量</b>：1-8\
  刺繡濾鏡會嘗試將匯入的圖片拆分成不同顏色——修改此值以改變使用的顏色數量。
* <b>密度</b>：80-300\
  選擇纖維密度。
* <b>設計</b>：填滿、輪廓、填補+輪廓、頂縫\
  選擇刺繡模式： *填充* 填滿所有色區， *輪廓* 建立色區輪廓， *填充 + 輪廓* 在每個色區同時建立輪廓，頂 *繡* 則建立該色區的頂繡輪廓。
* <b>補片/大綱： </b>0-1\
  改變纖維在色區的分布方式。
* <b>討論串</b>：\
  調整螺紋的粗細和長度。
* <b>Smooth Areas： </b>0-1\
  均勻化色區並影響線的行為。
* <b>不完美：</b>0-1\
  在線上加一些瑕疵，有助於打破圖案

<b>顏色1</b>

使用控制鍵逐一調整每個色區。

* <b>填充</b>：切換\
  讓色區可見或隱形。
* <b>身高</b>：\
  偏移螺紋的方向

<b>縫合處理</b>

* <b>自訂顏色：</b>\
  自訂整個刺繡的顏色
* <b>粗糙度： </b>0-1\
  將粗糙度值調整，使刺繡呈現粗糙或光澤。
* <b>金屬： </b>0-1\
  改變金屬感值，讓螺紋帶有金屬感。
* <b>各向異性等級： </b>0-1\
  改變各向異性以強調金屬性。

<b>進階</b>

* <b>正常強度</b>：0-1\
  調整法線強度。
* <b>身高範圍：</b> 0-1\
  調整刺繡在基材上的高度位置。
* <b>身高位置：</b>0-1\
  調整刺繡在基材上的高度位置。

## 使用指南

刺繡過濾器一開始可能會有點混亂，但只要先掌握幾個重要參數，你很快就能為材料添加補丁。

>[!NOTE]
>
> 如果你用過 [Weave](weave.md)濾網，刺繡濾芯的原理類似。

使用刺繡濾鏡：

1. 把刺繡濾鏡加到你的層疊裡。
1. 使用 <b>基本參數> Image</b> 將圖片加入濾鏡，或將圖片加入 Embroidery 濾鏡下方的圖層堆疊（非輸入槽）。 若影像未加入 <b>Basic 參數>影像</b>，濾鏡會自動擷取掃描通道中的影像（若有的話）。
1. 調整 <b>基本參數>色彩計數 </b>，直到色彩平衡看起來符合你的影像。 在限制 8 種顏色時，啟用或關閉顏色以分離你需要的顏色。\
   刺繡濾鏡最適合用在純色和插畫圖片上。
1. 調整其他參數以微調補丁的外觀。

在刺繡濾鏡中可以使用透明影像，但預設情況下，這些也會影響材質的不透明度貼圖——影像中透明的部分也會讓材質變得透明。 要用刺繡濾鏡製作一個補丁，讓它放在下方的層上，請使用貼花濾鏡。

1. 建立貼花濾鏡。
1. 將刺繡濾鏡加到貼花濾鏡的輸入槽。
1. 按照正常步驟調整刺繡圖案。

Decal 圖層會把 Embroidery 輸入轉換成 Decal——所以 Embroidery 圖層的透明度會告訴貼紙圖層如何遮蔽刺繡圖案。 透過 Decal 圖層，你也可以在材質上移動圖案，或啟用像是平鋪等功能。
