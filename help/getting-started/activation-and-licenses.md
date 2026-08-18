---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/getting-started/activation-and-licenses.html"
breadcrumb-title: ''
description: 了解如何啟用並管理 Substance 3D Sampler 的授權，以便開始使用該應用程式並存取所有功能。
helpx_creative_field: ""
helpx_description: Sampler > Getting Started > Activation and licenses
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 啟動與執照
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---


# 啟動與執照

本頁有關於如何啟用和管理授權的資訊，讓你能開始使用 Sampler。

## 依應用程式類型的啟動流程

啟動流程取決於你在哪裡購買或能取得 Sampler：

| 應用類型 | 啟動過程 |
| --- | --- |
| 創意雲端桌面 | 請參閱 HelpX 文件[&#128279;](https://helpx.adobe.com/tw/support/substance-3d-sampler.html)中的專屬頁面。若有任何問題， [Creative Cloud 的文件](https://helpx.adobe.com/tw/creative-cloud/user-guide.html) 可能會提供更多解答。 |
| 蒸汽 | 直接從 Steam 遊戲庫啟動產品。 |
| Substance 3D 獨立版 | 請參考下方說明的啟動流程。 |

## 啟動步驟

### 啟動巫師

![](../assets/activation-wizard.png){width="350px"}

有三種選擇：

* **評估此產品**：舊有試驗已不再提供。 你可以在這裡或使用 Creative Cloud Desktop 開始為每個 Substance 3D 應用程式[&#128279;](https://www.adobe.com/creativecloud/3d-augmented-reality.html)開啟 30 天試用。每個試驗都獨立於其他Substance 3D應用程式，所以你可以一次嘗試一個或全部。
* **使用授權檔案**&#x200B;啟用：請於 2022 年 9 月 30 日前，使用 Substance 3D 網站[&#128279;](https://store.substance3d.com/user)帳號頁面下載的授權檔案（**\*.key**）啟用產品。
* **使用您的帳戶**&#x200B;啟用：舊有物質帳戶已無法再用於啟用。 [更多關於Substance帳戶的資訊請見此](https://helpx.adobe.com/tw/substance-3d/unlisted/faq-end-of-life-accounts.html)處。

>[!WARNING]
>
> 要用啟用精靈安裝授權檔案，請確保以管理員身份執行 Sampler，並暫時停用防毒軟體。

### 手動啟動

你可以手動啟用 Sampler，方法是將 license.key **檔案放入**&#x200B;以下資料夾：

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>平台</th><th>版本</th><th colspan="2">路徑</th></tr><tr><td rowspan="4"><strong>窗戶</strong></td><td rowspan="2"><strong>3.0</strong> 或更新版本</td><td colspan="1">App Data（本地）</td><td colspan="1">C：\Users\[username]\AppData\Local\Adobe\Adobe Substance 3D 取樣器</td></tr><tr><td colspan="1">App Data（漫遊）</td><td colspan="1">C：\Users\[用戶名]\AppData\Roaming\Adobe\Adobe Substance 3D 取樣器</td></tr><tr><td rowspan="2">遺產</td><td colspan="1">App Data（本地）</td><td colspan="1">C：\Users\[用戶名]\AppData\Local\Allegorithmic\Substance Alchemist</td></tr><tr><td colspan="1">App Data（漫遊）</td><td colspan="1">C：\Users\[用戶名]\AppData\Roaming\Allegorithmic\物質煉金術師</td></tr><tr><td rowspan="2"><strong>麥克</strong></td><td colspan="1"><strong>3.0</strong> 或更新版本</td><td colspan="2">/使用者/[使用者名稱]/函式庫/應用程式支援/Adobe/Adobe Substance 3D 取樣器</td></tr><tr><td colspan="1">遺產</td><td colspan="2">/使用者/[用戶名]/圖書館/應用程式支援/寓言/物質煉金術師</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>3.0</strong> 或更新版本</td><td colspan="2">/home/[username]/.local/share/Adobe/Adobe Substance 3D 取樣器</td></tr><tr><td>遺產</td><td colspan="2">/home/[用戶名]/.local/share/Allegorithmic/物質煉金術士</td></tr></tbody></table>

>[!NOTE]
>
> 上述路徑中的部分目錄可能預設是隱藏的。 在檔案總管手動輸入路徑，或顯示隱藏檔案以查看。

>[!NOTE]
>
> 請確保檔案被呼叫 **license.key** 否則應用程式找不到。

### 環境變數

你可以用[環境變數](../pipeline-and-integrations/environment-variables.md)覆蓋 Sampler 檢查 **license.key** 檔案的位置。
