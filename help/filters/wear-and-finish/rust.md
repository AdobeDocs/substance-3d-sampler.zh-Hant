---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/filters/wear-and-finish/rust.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的鏽蝕濾鏡，為金屬材料和表面添加逼真的鏽蝕與腐蝕效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Rust
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 生鏽
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---


# 生鏽

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-rust-18-n-d.png)

**內容：** 磨損與表面處理

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

用 **防鏽過濾器** 在材料上加一層氧化金屬。

在下面的圖片中，你可以看到裝上 **防鏽過濾器**&#x200B;前後的金屬材質。

![](../../assets/3d-filters-cropped-0002-rust-out.jpg){width="200px"}

</td>
</tr>
</table>

## 參數

**基本參數**

* **隨機種子**：\
  隨機種子決定了使用此濾波器中使用隨機性的其他參數的隨機值。
* **Rust 讓分**：0-1\
  控制鏽蝕的擴散或數量。
* **邊線影響力**：0勝1負\
  根據曲率貼圖調整鏽蝕與邊緣的互動方式。
* **散布平滑度**：0-1\
  增加這個比例讓生鏽區域變得更團結，或降低它讓細節更豐富。
* **僅限**&#x200B;情感金屬：切換\
  啟用後， **Rust 濾波器** 只會影響金屬值大於 0 的區域。

**生鏽**

* **鏽蝕形狀**：\
  改變鏽蝕的圖案。
* **鏽蝕強度**：0-1\
  調整生鏽效應的強度。 提高這個數值會讓鏽看起來更老更堅固。

**皮爾**

* **皮爾等級**：0-1\
  改變剝落鐵鏽的比例。
* **剝皮 正常強度**：0-1\
  調整剝皮法線的可見度。
* **剝皮高度**&#x200B;強度：0-1\
  調整剝離對高度圖的影響。

**滴落**

* **Drips 強度**：0-1\
  改變滴水效果的強度。
* **水滴方向**：0-1\
  讓滴水方向符合重力或風向。
* **滴水長度**：0-1\
  調整滴水距離源頭的距離。

**面具**

* **使用面罩**：切換\
  啟用或停用自訂遮罩的使用。 啟用後會出現以下參數：
  * **遮罩**：影像/筆刷\
    選擇一張圖片作為遮罩，或用畫筆直接在 2D 視圖中繪製自訂遮罩。
  * **自訂面具 - 模糊**：0-1\
    模糊面具。
  * **自訂遮罩 - 反轉**：切換\
    把面具倒過來。
