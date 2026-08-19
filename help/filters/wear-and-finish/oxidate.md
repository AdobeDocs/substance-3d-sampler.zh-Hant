---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/filters/wear-and-finish/oxidate.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的氧化濾鏡，為金屬材料添加氧化與氧化變色效果，呈現老化外觀。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Oxidate
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 氧化
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---


# 氧化

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-oxidate-18-n-d.png)

**內容：** 磨損與表面處理

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

在材料表面加一層氧化層。*皺摺的表面會貼上&#x200B;**氧化濾紙**。*

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0019-oxidate-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0018-oxidate-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## 參數

**基本參數**

* **隨機種子**：\
  隨機種子決定了使用此濾波器中使用隨機性的其他參數的隨機值。
* **目標區域**：切換\
  能夠改變氧化效應在材料上的應用方式。 啟用後，會出現以下控制項：
  * **目標區域實力**：0-1\
    調整目標區域效果的擴散範圍。
  * **擴大比分**：0-1\
    調整氧化物的擴散距離。
* **顏色**：顏色選擇\
  選擇濾鏡的基底色。 基底色會改變構成氧化效果的所有顏色的色調。
* **顏色變化**：0-1\
  調整色彩變化效果的比例。
* **密度**：0-1\
  改變效果的覆蓋密度。
* **邊緣出血**：0-1\
  調整氧化邊緣滲入未氧化區域的方式。
* **補丁**：0-1\
  這是一個獨立的控制，用來調整氧化與非氧化區域之間的遮罩。 結合密度和其他控制措施，微調氧化區域的邊緣。
* **切球**：0-1\
  敲開氧化區域，露出底層材料。
* **污漬：** 0-1\
  調整覆蓋在材料上的染色量。
* **腐蝕粗糙度**：0-1\
  調整氧化區域的粗糙度。
* **腐蝕金屬**：0-1\
  調整氧化區域的金屬值。
* **噪音強度**：0-1

**面具**

* **使用自訂遮罩**：切換\
  啟用或停用自訂遮罩的使用。 啟用後會出現以下參數：
  * **遮罩**：影像/筆刷\
    選擇一張圖片作為遮罩，或用畫筆直接在 2D 視圖中繪製自訂遮罩。
  * **自訂面具 - 模糊**：0-1\
    模糊面具。
  * **自訂遮罩 - 反轉**：切換\
    把面具倒過來。
  * **自訂遮罩不透明度**：0-1\
    調整遮罩的不透明度。

**技術參數**

以下參數允許你調整整個材質的命名值，而不必新增像 **是亮度/對比** 度或 **色相/飽和度等調整層**

* **亮度**：0-1
* **對比**&#x200B;度：-1 比 1
* **色調變化**：0-1
* **戰績**：0勝1負
* **正常強度**：0-1
* **身高範圍**：0-1
* **身高位置**：0-1
* **環境遮蔽強度**：0-1
