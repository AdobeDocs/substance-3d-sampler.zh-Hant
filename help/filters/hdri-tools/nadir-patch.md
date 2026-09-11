---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/hdri-tools/nadir-patch.html"
breadcrumb-title: ''
description: 使用 Substance 3D Sampler 中的 Nadir Patch 工具，將 HDRI 影像的 Nadir 區域修補，打造無縫的環境貼圖。
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > Nadir Patch
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 低谷補丁
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---


# 低谷補丁

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-nadirpatch-18-n-d.png)

**收錄於：** HDRI 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

把環境燈的最低點補上，遮蓋瑕疵或接縫。

在下方圖片中，你可以看到 Nadir Patch **如何**&#x200B;用來移除這張全景影像中的相機支架。

![](../../assets/3d-2d-filters-cropped-0011-nadir-patch-in.jpg)![](../../assets/3d-2d-filters-cropped-0010-nadir-patch-out.jpg)

</td>
</tr>
</table>

## 參數

**基本參數**

* **啟用**：切換\
  開啟或關閉補丁——這很方便快速看到補丁的影響，而不必改變圖層可見性。
* **顯示框架輔助：**&#x200B;切換\
  開關框架。
* **車架厚度**：0-1\
  調整框架厚度。 當補丁來源遠離最低點時，這會很有幫助。
* **補丁等級**：0-1\
  調整待補丁區域的邊界。
* **補丁大小**：\
  調整補丁的尺寸。
* **補丁輪替**：0-1\
  旋轉補丁邊界。 這樣會同時旋轉來源和補丁的位置，因此補丁的方向仍然相同。 要在原地旋轉補丁，請使用 **來源旋轉偏移**。
* **Patch Alpha**：\
  選擇用來遮罩該補丁的形狀。 若 **選擇遮罩輸入** ，則會出現一個額外參數：
  * **遮罩輸入**：影像/筆刷\
    匯入圖片作為遮罩，或直接在 2D 視圖&#x200B;**中**&#x200B;繪製遮罩。
* **補丁硬度**：0-1\
  調整遮罩邊緣的模糊度。
* **源旋轉偏移**&#x200B;量：0-1\
  偏移光源的旋轉——這會產生旋轉音色的效果。

## 使用指南

從照片製作環境光時，常見的問題是貼圖頂端和底部的底層周圍會出現瑕疵。 **Nadir Patch** **過濾器**&#x200B;有助於減少這些問題。

1. 將 **Nadir Patch 濾波器** 加到圖層堆疊的頂端。
1. 在 2D 視圖&#x200B;**中使用 handle**，可以更改音色的來源位置。
   1. 斑塊天底會根據源的位置而改變。 若來源位於貼圖空間的下半部，底部天底會被修補;若來源位於上半部，則頂端天底會被補丁。
1. 修改參數以微調補丁的轉換，以最好地隱藏接縫和瑕疵。
