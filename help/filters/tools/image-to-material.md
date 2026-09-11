---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/image-to-material.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的影像轉材質工具，利用AI驅動的處理將單一影像轉換為完整的PBR材質。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Image To Material
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 圖片到素材
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# 圖片到素材

![](../../assets/sat-icon-image-to-material.png)

**影像轉材質**&#x200B;範本允許從單一輸入影像產生高品質的 PBR 素材。

此範本有兩個主要演算法：

* **AI 驅動**
* **B2M**

以下將詳細說明每個演算法。

## 範例

以下是由單一輸入影像產生的材質通道範例：

![](../../assets/sat-image-to-material.jpg){width="500px"}

## 演算法

要將圖片轉換為材質&#x200B;**範本的演算法**，請點擊範本名稱下方的下拉選單：

![](../../assets/image-to-material-algo-setting.png)

### AI 驅動

AI <b>驅動</b> 的演算法利用機器學習辨識形狀與物體，精確生成法線、高度與粗糙度地圖，並消除陰影或高光中的反照率。

神經網路已訓練於多種材料，如布料、有機物、室內及室外表面。

>[!NOTE]
>
> 影像轉材質（AI 驅動）在高解析度影像上計算會花較長時間，我們建議使用 [圖層解析度](../../interface/preferences/layer-resolution.md) 系統來優化工作流程。

### B2M

**B2M** 演算法使用基於物質的點陣圖到材質方法，透過程序化技術產生多重通道，如基色、法線、金屬、粗糙度及環境遮蔽。

此演算法可能產生較不精確的結果，但能適用於更廣泛的輸入影像。

## Adobe 擷取

此功能也可在 Adobe Capture 行動應用程式（Android 與 iOS）上使用。 你可以隨時隨地拍照，直接用手機預覽結果。

輕鬆將結果送至 Substance 3D Sampler，以便後續版本。

![](../../assets/capture-qr-code.gif)

>[!NOTE]
>
> 此功能僅需訂閱 Adobe Substance 3D Collection 才能使用。
