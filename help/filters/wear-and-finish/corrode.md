---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/wear-and-finish/corrode.html"
breadcrumb-title: ''
description: 在 Substance 3D Sampler 中使用腐蝕過濾器，對金屬材料添加腐蝕和化學劣化效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Corrode
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 腐蝕
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---


# 腐蝕

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/corrode-filter-icon.png)

**內容：** 磨損與表面處理

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

腐蝕過濾器模擬酸蝕材料的效果，留下破洞和表面損傷。

</td>
</tr>
</table>

## 參數

**基本參數**

* **隨機種子**：\
  隨機種子決定了使用此濾波器中使用隨機性的其他參數的隨機值。
* **受影響地區**：\
  選擇表面曲率如何影響濾鏡效果。
* **穿孔等級**：0-1\
  調整產生的孔數。
* **曲率位置**：0-1\
  調整曲率範圍以受影響。
* **曲率平滑**：0-1\
  把曲率貼圖平滑。
* **傷害距離**：0-1\
  控制腐蝕區域周圍的傷害範圍。
* **傷害強度**：0-1\
  調整受影響部位的損傷程度。
* **身高強度**：0-1\
  控制傷害對高度地圖的影響。
* **擠出位置**：切換\
  在高度圖上切換傷害方向。 禁用時，傷害會侵蝕表面;啟用時，傷害會從表面向外累積。

**面具**

* **使用自訂遮罩**：切換\
  啟用或停用自訂遮罩的使用。 啟用後會出現以下參數：
  * **遮罩**：影像/筆刷\
    選擇一張圖片作為遮罩，或用畫筆直接在 2D 視圖中繪製自訂遮罩。
  * **自訂面具 - 模糊**：0-1\
    模糊面具。
  * **自訂遮罩 - 反轉**：切換\
    把面具倒過來。

**進階參數**

部分進階參數會影響整個材質，而非僅影響此濾鏡所修改的區域。

* **亮度**：0-1\
  調整整件材料的亮度或輕度。
* **對比**&#x200B;度：-1 比 1\
  調整全材質的反照率對比度。
* **色調變化**：0-1\
  在整個材質中抵消顏色的色調值。
* **戰績**：0勝1負\
  調整飽和度以符合整體素材。
* **正常強度**：0-1\
  調整法線貼圖被腐蝕濾波&#x200B;**器影響**&#x200B;的強度。
* **身高範圍**：0-1\
  擴大整個材質高度圖中數值的範圍。
* **身高位置**：0-1\
  讓整件材料的高度偏移。
* **環境遮蔽強度**：0-1\
  調整腐蝕 **過濾器**&#x200B;造成的AO衝擊強度。
