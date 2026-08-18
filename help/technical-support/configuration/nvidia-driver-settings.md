---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/technical-support/configuration/nvidia-driver-settings.html"
breadcrumb-title: ''
description: 學習如何設定 NVIDIA 驅動程式設定以優化 Substance 3D Sampler 並解決遲滯行為。
helpx_creative_field: ""
helpx_description: Sampler > Technical Support > Configuration > NVIDIA Driver Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: NVIDIA 驅動程式設定
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---


# NVIDIA 驅動程式設定

如果你使用 NVIDIA 顯卡但覺得效能遲緩，有兩個常見原因：

1. 驅動程式遺失或不更新
1. 取樣器使用的顯示卡不正確

## 更新驅動程式

要更新你的 NVIDIA 驅動程式：

1. 前往 NVIDIA 的驅動下載頁面 - <https://www.nvidia.com/Download/index.aspx?lang=en-us>
1. 選擇你的顯示卡型號並下載驅動程式。
1. 用下載的檔案安裝驅動程式。

安裝最新驅動程式後，打開 Sampler 查看效能是否有改善。 如果效能較慢，Sampler 可能用錯了 GPU。

## 設定取樣器

要確認是哪個 GPU 取樣器，請做以下操作：

![](../../assets/nvidiacontrolpanel.png)

1. 打開 NVIDIA 控制面板。 要開啟 NVIDIA 控制面板，請執行以下其中一項操作：
   1. 使用開始選單搜尋 NVIDIA 控制面板
   1. 在系統托盤中，右鍵點擊 Geforce 圖示，選擇 NVIDIA 控制面板。
1. 在 NVIDIA 控制面板中，選擇左側選單的「管理 3D 設定」。
1. 選擇程式設定標籤。
1. 在「選擇一個可自訂的程式」中，使用下拉選單找到取樣器。
1. 如果下拉選單沒有 Sampler，請使用新增。
   1. 瀏覽以找到 Sampler 的安裝地點（預設安裝地點為 **C：/Program Files/Adobe/Adobe Substance 3D Sampler**）。
   1. 從安裝地點選擇 **Adobe Substance 3D Sampler.exe** 。
1. 選擇取樣器後，在「選擇本程式的首選顯示處理器」中，選擇「高效能 NVIDIA 處理器」。
1. 點擊「應用」。

完成此流程後，開啟 Sampler 查看效能是否有改善。
