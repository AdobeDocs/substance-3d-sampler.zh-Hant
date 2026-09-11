---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/filters/tools/upscale.html"
breadcrumb-title: ''
description: 使用 Substance 3D Sampler 中的放大工具，利用 AI 驅動的放大技術提升材質解析度。
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 高級化
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 1%

---


# 高級化

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![過濾器圖示](../../assets/SAPR_SuperResolution_18_N_D.png)

**收錄於：** 工具

</td>
<td style="border: 0;" valign="top">

## 說明

<b>升頻</b>濾鏡使用 AI 從下方層級的 PBR 通道（基色、粗糙度、法線、金屬感、高度）進行上采樣。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">



</td>
<td style="border: 0;" valign="top">

![](../../assets/F5W_vAHaYAQLsz7.jpg)

</td>
</tr>
</table>

在這個範例中，我們從一張 1024x1024px 的影像開始，但輸出結果是 4098x4098px。 使用 <b>升頻</b>濾波器的結果更明確。

</td>
<td style="border: 0;" valign="top">

>[!NOTE]
>
> **進階濾波器**
> 
> <b>升頻</b>是進階過濾器。\
> 為了最大化使用並避免結果模糊，我們建議在「圖層輸入最大」或「圖層輸入最小」中設定低於 <b>升頻</b>的圖層。
> 
> 升級濾波器的數量沒有限制<b></b>，但超過 8k 解析度的升頻可能會大幅影響效能。

</td>
</tr>
</table>

## 參數

<b>基本參數</b>

* <b>上行範例</b>：切換按鈕群組\
  選擇放大倍率因子

## 如何

![](../../assets/SAPR_Upscale_screen_001.png)

在上方圖片中，低解析度影像由影像轉材質（AI 驅動）[&#128279;](image-to-material.md)處理。

![](../../assets/SAPR_Upscale_Screen_003.png)

<b>會加上升頻</b>濾波器來提升取樣結果。它透過幻覺細節來達到更高的解析度，同時保持材料的品質。 你可以在屬性中選擇上採樣 2 或 4。
