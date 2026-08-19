---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/filters/tools/delight-ai-powered.html"
breadcrumb-title: ''
description: 在 Substance 3D Sampler 中使用 AI 驅動的 Delight 濾鏡，去除影像中的光線資訊並創造中性基材。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Delight (AI Powered)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Delight（AI 驅動）
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---


# Delight（AI 驅動）

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-lightgeneric-18-n-d.png)

**收錄於：** 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

Delighter 允許你從基色通道移除光照資訊。 這在將影像轉換成材質時非常重要，因為一般材質不應該包含光照資訊。 材料是一組解釋光應該如何與表面反應的資訊集合，所以如果通道裡已經內建了光資訊，而該通道本不該有光資訊，就可能破壞材料真實呈現表面的能力。

*一個圖片在 Delight（AI 驅動）濾鏡&#x200B;**處理前後**&#x200B;的範例。注意陰影和高光已被移除，只剩底色。*

![](../../assets/120-0-comparison.png)

下方圖片展示了材料在被 **Delight（AI 驅動）濾鏡**&#x200B;處理前後。

![](../../assets/3d-2d-filters-cropped-0043-delighter-in.jpg)

在上圖中，材質在基色通道中仍包含大量光照資訊。 磚塊間的暗影不應該出現在基色通道中。

![](../../assets/3d-2d-filters-cropped-0042-delight-out.jpg)

在愉悅過鏡後，陰影會被移除，以創造出更為物理精確的底色通道。 雖然這個例子中的效果看起來不明顯，但讓影像愉悅是將影像轉化為材料的重要一步。

在光源影像中，光來自靜態光源，但材質必須能承受任何角度的光。 例如：如果一張光線從上而下照射的來源影像，未經愉悅步驟轉換成材質，它可以顯示在光線從下而上照射的三維空間中。 材料會很快看起來格格不入，因為它同時看起來像是從多個光源投射陰影，而只有一個光源。

</td>
</tr>
</table>

## 參數

Delighter 沒有任何參數——它是自動運作的。

## 使用指南

怎麼用？

把 Delighter 濾鏡&#x200B;**加**&#x200B;到圖層堆疊的最上方。

### 什麼時候該用？

使用 **影像到材質（B2M）**&#x200B;時，當你從圖片中提取所有通道並讓材質可平鋪後，使用愉悅器移除底色中的光照資訊。 **Image to Material（AI 驅動）** 包含 Delighter 通道，所以你不需要搭配 **Delighter（AI 驅動）濾鏡** 。
