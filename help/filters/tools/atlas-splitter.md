---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/atlas-splitter.html"
breadcrumb-title: ''
description: 使用 Substance 3D Sampler 中的 Atlas Splitter 工具，將材質圖集拆分成獨立的貼圖以便材質編輯。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Atlas Splitter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Atlas 分裂器
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---


# Atlas 分裂器

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-atlassplitter-18-n-d.png)

**收錄於：** 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

**Atlas Splitter** 是一個有用的工具，可以組織和檢視地圖集的元素。

下方圖片展示了 **Atlas Splitter** 的實際運作。

![](../../assets/3d-2d-filters-cropped-0039-atlas-splittter-in.jpg)

上圖顯示了將圖集材質加入圖層堆疊。 使用 **地圖集分割器** 從地圖集中選擇特定元素。

![](../../assets/3d-2d-filters-cropped-0038-atlas-splitter-out.jpg)

新增 **圖集分割** 器後，可以聚焦在單一葉子或圖譜材質的其他元素上。

</td>
</tr>
</table>

## 參數

**基本參數**

* **格狀視圖**：切換\
  在格子視圖和元素的個別視圖之間切換。 若啟用，會出現以下額外參數：
  * **網格不透明度**：0-1\
    修改網格的不透明度
  * **格子選擇不透明度**：0-1\
    修改選取元素周圍邊框的不透明度
  * **自動縮放**：切換\
    切換圖集元素是否縮放以填滿每個格子格。
* **自動裁切**：切換\
  選擇是否調整所選形狀的裁切。 若啟用，將會出現額外選項：
  * **自動裁切模式**：\
    選擇如何裁切選取元素以填補材質空間。
* **形狀選擇**：1-10\
  更改選取圖集的哪個元素。 對於超過 10 個元素的圖集，你可以在形狀選擇&#x200B;**值中**&#x200B;輸入數字，以改變滑桿的範圍。
* **輪值**：0勝1敗\
  旋轉元素

**進階參數**

* **小尺寸公差**：0-1\
  調整Atlas Splitter **要拾取**&#x200B;的最小形狀大小。這對於過濾雜訊很有用
* **自動旋轉**：切換\
  啟用後，元素會自動旋轉以呈現相似的方向。
* **下階不透明度遮罩**：0-4\
  調整不透明度遮罩的比例。 請注意，增加此值可能會降低不透明度遮罩的品質。
* **形狀偵測精確**&#x200B;度：\
  選擇要使用的形狀偵測演算法。
* **膨脹寬度**：0-32\
  修改放大——這會將元素邊框的顏色擠出到遮罩區域，幫助避免圖集元素邊緣的透明度問題。 在 2D 視圖&#x200B;**中查看基底色彩通道**&#x200B;以查看結果。
* **自訂背景色**：切換\
  啟用時，會出現一個控制項來修改正常頻道的背景顏色：
  * **普通背景色彩**：色彩選擇\
    在材質透明部分選擇法線通道的自訂背景色。
* **身高 Bg 顏色**：0-1\
  調整高度通道的背景色。 通常建議讓背景高度與圖集元素邊界的平均高度相符，以避免元素邊界出現雜訊。
