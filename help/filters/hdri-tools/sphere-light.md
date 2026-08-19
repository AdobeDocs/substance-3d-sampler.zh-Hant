---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/filters/hdri-tools/sphere-light.html"
breadcrumb-title: ''
description: 在 Substance 3D Sampler 中使用 Sphere Light 工具，為 HDRI 環境加入球形光源，以產生點光效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > Sphere Light
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 球光
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---


# 球光

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-spherelight-18-n-d.png)

**收錄於：** HDRI 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

在你的環境中加入球形光源。

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
  * **範例背景**
    * 取樣背景不會提供新的參數——它會根據背景值來決定光色。
* **曝光（EV）：** 0-10\
  調整光線的曝光或亮度。
* **球半徑**：0-1\
  調整燈的大小。
* **位置模式**：\
  改變用來判斷燈光位置的方法。 位置座標&#x200B;**區塊的**&#x200B;參數會根據選擇而改變。

**位置座標**

可用參數取決於基本參數的選擇 **>位置模式**。 若 **選擇「距離原點** 」，則可參考以下參數：

* **距離起點**&#x200B;距離：0-20\
  調整光線與相機的距離。
* **攝影機位置**：0-1\
  調整相機在 X、Y 和 Z 軸上與光線的相對位置。

若 **選擇世界位置** ，則可參考以下參數：

* **向上向量**：\
  改變上方方向。
* **球面世界位置**：-2 到 2\
  調整球光在X軸、Y軸和Z軸的位置。
* **距離起點**&#x200B;距離：0-20\
  調整光線與相機的距離。
* **攝影機位置**：0-1\
  調整相機在 X、Y 和 Z 軸上與光線的相對位置。

**形狀**

* **球體硬度**：0-1\
  軟化或硬化球體光的邊緣
* **陰影：**\
  根據不同現實光線風格改變光線曝光的漸層。 **選擇陰影燈**&#x200B;後，會顯示額外參數：
  * **陰影光世界位置**：-1 到 1\
    調整陰影區域在燈光上的位置
  * **半影透明**&#x200B;隊：0-1\
    調整光線陰影區域的透明度。

**背景**

* **背景伽瑪**：\
  選擇用來判定背景伽瑪的顏色系統。
