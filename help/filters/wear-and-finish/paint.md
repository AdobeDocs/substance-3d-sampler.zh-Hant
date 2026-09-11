---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/wear-and-finish/paint.html"
breadcrumb-title: ''
description: 在 Substance 3D Sampler 中使用 Paint 濾鏡，為你的材質添加顏料層、塗層和塗裝表面效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Paint
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 塗料
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---


# 塗料

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-paint-18-n-d.png)

**內容：** 磨損與表面處理

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

**Paint 濾鏡**&#x200B;讓你能在材料上覆蓋一層不同厚度的油漆。

*一種金屬材質，上面加了磨損的油漆。*

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0017-paint-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0016-paint-out.jpg){width="200px"}

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
* **顏色**：顏色選擇\
  設定油漆顏色。
* **粗糙度**：0-1\
  設定油漆覆蓋區域的粗糙度。
* **厚度**：0-1\
  調整顏料的黏度和厚度。 這會影響底層高度和法線資訊能透過油漆看到多少。
* **皮爾**：0-1\
  在油漆剝落的地方補貼。
* **穀粒**：0-1\
  改變顏料表面的紋理。
* **晶粒大小**：1-5\
  調整用來製作顆粒的紋理比例。

**面具**

* **腔體面罩**：切換\
  根據高度圖中找到的空腔建立遮罩。 啟用後會出現以下參數：
  * **腔室大小**：0-1\
    調整用來製作空腔遮罩的高度範圍。
  * **蛀牙強度**：0-1\
    根據腔體深度調整遮罩的不透明度。
  * **腔體反轉面罩**：切換\
    反轉腔體遮罩以改變它對高點或低點的影響。
* **使用自訂遮罩**：切換\
  啟用或停用自訂遮罩的使用。 啟用後會出現以下參數：
  * **遮罩**：影像/筆刷\
    選擇一張圖片作為遮罩，或用畫筆直接在 2D 視圖中繪製自訂遮罩。
  * **自訂面具 - 模糊**：0-1\
    模糊面具。
  * **自訂遮罩 - 反轉**：切換\
    把面具倒過來。

**進階參數**

* **基色**：切換\
  設定底色通道是否會受到濾鏡的影響。
* **金屬：**&#x200B;切換\
  設定金屬通道是否受濾波器影響。
  * **金屬價值**：0-1\
    調整塗裝區域的金屬值。
* **粗糙度**：切換\
  設定粗糙通道是否會受到濾波器的影響。
* **一般：**&#x200B;切換\
  設定正常頻道是否受濾波器影響。 若啟用，則會出現額外控制：
  * **正常 - 強度**：-1 比 1\
    調整法線強度。
* **高度**：切換\
  設定高度通道是否受濾波器影響。 若啟用，則會出現額外控制：
  * **身高 - 強度**：0-1\
    調整高度圖的對比度。
* **不透明度**：切換\
  設定不透明度通道是否會受到濾波器的影響。 若啟用，則會出現額外控制：
  * **不透明度 - 值**：0-1\
    改變材質的不透明度。
* **發射器**：切換\
  設定發射通道是否受濾波器影響。 若啟用，則會出現額外控制：
  * **發射體 - 顏色**：顏色選擇\
    設定發射通道的顏色。
* **環境遮蔽**：切換\
  設定環境遮蔽通道是否會受到濾波器的影響。 啟用後，會出現以下額外控制項：
  * **環境遮蔽 - 強度**：0-1\
    調整生成AO的強度。
  * **環境遮蔽** **- 半徑**：0-1\
    調整AO效果的半徑。
