---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/hdri-tools/shape-light.html"
breadcrumb-title: ''
description: 使用 Substance 3D Sampler 中的 Shape Light 工具，為 HDRI 環境新增自訂形狀的光源，營造創意光影效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > Shape Light
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 形狀光
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---


# 形狀光

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-shapelight-18-n-d.png)

**收錄於：** HDRI 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

創造一個長方形或圓盤形狀的燈光。

</td>
</tr>
</table>

## 參數

**基本參數**

* **形狀色彩模式**：\
  選擇用哪種方法來判斷燈光的顏色。 可用參數會根據這個選擇而改變。
  * **溫度（開爾文）**
    * **溫度**：1000 - 27000\
      調整燈光的溫度。
  * **RGB**
    * **顏色**：顏色選擇\
      選擇燈的顏色。
  * **影像輸入**
    * **形狀影像輸入**：image/brush\
      匯入一張圖片作為顏色。 你可以用筆刷工具直接在 **2D 視圖**&#x200B;中繪製，但用這個濾鏡可能會產生不可預測的結果。
* **熱點暴露（EV）：** 0-10\
  調整熱點的曝光。 熱點有時難以或無法被看見——在新的 **Shape Light 濾鏡**&#x200B;中，將 Shape Temperature **設**&#x200B;為 1000，**並將熱點曝光****（EV）**&#x200B;設為 10，這樣就能看到形狀中心的熱點。
* **形狀**：\
  設定燈的形狀。

**職位**

* **熱點位置**：0-1\
  偏移熱點的位置
* **矩陣偏移**&#x200B;量：-2 到 2\
  改變形狀燈的位置。 你也可以在 2D 視角&#x200B;**拖曳光源**&#x200B;來重新定位。

**形狀**

* **形狀曝光（EV）：** 0-10\
  調整光線曝光
* **形狀硬度**：0-1\
  柔化光線的邊緣
* **熱點大小**：0-1
* **熱點衰減**：0-1\
  調整熱點邊緣的柔軟度。

**背景**

* **背景伽瑪**：\
  選擇用來判定背景伽瑪的顏色系統。
