---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/features-and-workflows/end-to-end-physical-size-workflow.html"
breadcrumb-title: ''
description: 學習如何運用 Substance 3D Sampler 中的端到端物理尺寸工作流程，創造出與真實比例相符的物理精確材質。
helpx_creative_field: ""
helpx_description: Sampler > Features and workflows > End to end Physical Size Workflow
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 端對端實體尺寸工作流程
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 端對端實體尺寸工作流程

在數位環境中，將掃描樣本和影像的實際尺寸相匹配，以創造跨應用程式的物理精確視覺效果。

## 匯入掃描

1. 選擇素材製作範本。
1. 勾選實體尺寸勾選框。

   ![](../assets/screenshot-2022-01-20-at-16-15-53.png)
1. 設定實體尺寸有兩種方法：

   3a。 點擊手動測量 - 測量工具允許您校準樣品兩個特徵間的物理尺寸。\
   兩點之間的軌道 -> 進入

   ![](../assets/screenshot-2022-01-20-at-16-31-26.png)

   3b。 自動測量 - 自動測量工具允許您根據影像元資料（dpi）估算樣本的物理尺寸。 它比較快，但只適用於掃描，因為它會利用儲存的 dpi 來計算精確的起始尺寸。

   <b>你現在可以處理掃描了</b>
1. 加一個裁切圖，然後根據取樣調整。 你可以在 2D 視窗右下角看到實體尺寸的更新。

   在 2D 視窗中以物理比例顯示，這樣才能準確看到你正在製作的地圖。\
   你可以設定 2D 視角以符合實體尺寸，這樣螢幕比例的 DPI 就會和材質比例相符。 換句話說，你可以把真實樣品放在螢幕旁邊，來驗證尺寸。

   ![](../assets/cq5dam.web.1280.png)
1. 加一個均衡器來消除漸變。
1. 加裝平鋪來修正平鋪看起來
1. 如果需要，曲速變換只適合重新對齊地圖的部分區域。

   <b>準備出口</b>
1. 出口為

   選擇 Sbsar 格式，Sampler 會將 Physical Size 作為元資料輸入。 它也將允許其他應用程式讀取並使用這些資訊。\
   你也可以匯出影像;它會尊重實體尺寸比例。

   如果你需要使用實體尺寸，請使用 *實體尺寸面板*。

   當匯出為影像時，現在可以強制影像大小以符合物理尺寸比例。

## 影片教學

你也可以找到影片教學，幫助你完成這個功能：
