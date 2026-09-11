---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/features-and-workflows/end-to-end-physical-size-workflow.html"
breadcrumb-title: ''
description: 瞭解如何使用Substance 3D Sampler的端對端實體尺寸工作流程，建立符合實際尺度的精確材質。
helpx_creative_field: ""
helpx_description: Sampler > Features and workflows > End to end Physical Size Workflow
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 端對端實體大小工作流程
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 端對端實體大小工作流程

在數位內容中比對掃描樣本與影像的實際大小，以跨應用程式建立精確的物理視覺效果。

## 匯入掃描

1. 選取材料建立範本。
1. 核取實體大小核取方塊。

   ![](../assets/screenshot-2022-01-20-at-16-15-53.png)
1. 設定實體大小的兩種方法：

   3a。 按一下「手動測量 — 測量」工具可讓您校準樣本兩個特徵之間的實體大小。\
   在兩點之間追蹤 — >輸入

   ![](../assets/screenshot-2022-01-20-at-16-31-26.png)

   3b。 自動測量 — 自動測量工具可讓您根據影像中繼資料(dpi)來取得樣本的估計實體大小。 它速度較快，但只適用於掃描，因為它使用儲存的dpi計算精確的起始大小。

   <b>您現在可以處理掃描</b>
1. 新增裁切，並將其調整至範例。 您可以看到更新的2D視見區右下角顯示的物理大小。

   在2D視見區中以實體比例顯示，以準確地檢視您正在處理的地圖。\
   您可以設定2D檢視以符合實體大小，讓熒幕比率的DPI符合您的材質比例。 換句話說，您可以將真實樣本放在熒幕旁以驗證尺寸。

   ![](../assets/cq5dam.web.1280.png)
1. 加入Equalize以去除任何漸層。
1. 新增鑲邊以修正鑲邊
1. 如果需要，彎曲變形只可用於重新對齊地圖的部分。

   <b>準備匯出</b>
1. 匯出為

   選擇 Sbsar 格式，Sampler 會將 Physical Size 作為元資料輸入。 它也將允許其他應用程式讀取並使用這些資訊。\
   你也可以匯出影像;它會尊重實體尺寸比例。

   如果你需要使用實體尺寸，請使用 *實體尺寸面板*。

   當匯出為影像時，現在可以強制影像大小以符合物理尺寸比例。

## 影片教學

你也可以找到影片教學，幫助你完成這個功能：
