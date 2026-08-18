---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/version-4-4substance-3d-sampler.html"
breadcrumb-title: ''
description: 請參閱 Substance 3D Sampler 4.4 版本的發行說明，了解生成式工作流程，包括文字轉紋理及圖片轉貼圖功能。
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 版本 4.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 6cc0519fb8c0f74fa805691ec4adb9e449a627d5
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---


# 版本 4.4

<b>Substance 3D Sampler 4.4</b> 以測試版形式引入三種新的生成式工作流程：文字轉紋理、文字轉圖案與影像轉紋理。

<b>生成式 AI 功能僅在 Adobe 版本</b> 上提供，因為它需要 Adobe 帳號。 因此，這些功能在 Steam</b> 上無法<b>使用。

*上映日期：2024年5月23日*

## 文字轉貼圖

![](../assets/textToTexture_whatNewPanel.png)

文字轉材質讓你能透過文字提示</b>探索一種全新的材質創作<b>方式。你可以從詳細的文字描述產生平鋪紋理，並透過影像轉材質或任何取樣器濾鏡持續擴充，讓它成為獨一無二的。

## 影像到貼圖

![影像到貼圖](../assets/imagetoText_whatNewPanel.png "影像到貼圖")

透過 Image-to-texture，你可以從 <b>自己的參考影像</b>製作平鋪方形貼圖，不論是非正方形還是非平鋪。 這樣你就能更接近想要的結果，而不需要寫出完美的提示。\
圖片轉材質也能幫助你節省時間，透過從已創作的內容中創造變化。

## 文字轉模式

![文字轉圖案插圖](../assets/patterns_whatNewPanel.png)

文字轉圖案功能會利用你的<b> 文字提示</b> 生成方形拼貼圖案。 接著你可以用布料織布濾鏡作為底色，創造原創布料材料，也可以用作圖案濾鏡的輸入，還有更多功能！

## 發行說明

*（發行日期：2024年5月23日）*

<b>補充</b>：

* [應用程式] 3D 擷取快取現在被儲存在一個獨立的子資料夾中
* [生成式人工智慧]圖片轉材質（測試版）
* [生成式 AI]文字轉模式（測試版）
* [生成式人工智慧]文字轉紋理（測試版）
* [腳本操作]資產現在擁有「資源」屬性
* [腳本操作]圖層現在擁有「輸出\_usages」屬性

<b>修正：</b>

* [應用程式]打開損壞的專案檔案時當機
* [應用程式]當專案包含損壞的資產時會當機
* [應用程式]在 Windows 拔掉螢幕時會當機
* [應用程式]Windows 工作列中的應用程式圖示錯誤
* [應用程式]主要設定檔損壞可能導致檔案被刪除
* [應用]彈出視窗前會出現面板
* [內容]材質產生器的縮圖會模糊
* [匯出]匯入影像產生的不透明度通道在匯出 .sbs/.sbsar 時會出問題
* [濾波器]升頻可能會根據輸入層數當機
* [生成式人工智慧]收到服務意外結果時可能當機
* [腳本操作]自動載入環境變數外掛時會當機
* [腳本操作]在將輸出使用權指派給 API 時可能會當機
