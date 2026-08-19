---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/pipeline-and-integrations/hp-z-captis-support/faq-hp-z-captis-support-in-sampler.html"
breadcrumb-title: ''
description: 請參閱有關 Substance 3D Sampler 中 HP Z Captis 支援的常見問題，以了解硬體整合與使用方式的相關資訊。
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 關於 HP Z Captis 在 Sampler 中支援的常見問題
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '1547'
ht-degree: 0%

---


# 最常見問題

## 材料樣本

+++Captis 涵蓋哪些使用情境？
此解決方案涵蓋跨產業應用場景（汽車、服裝、產品設計、媒體與娛樂、建築等）。 Studio 模式支援桌面擷取（可重複、高效且簡單），而 Explorer 模式則支援行動擷取，「靈活、隨時隨地，適應各種情況」。

+++

+++哪些材質類型可以用 Captis 掃描並捕捉？
除了多層透明塗層外，任何材質類型都可以掃描並捕捉（汽車漆不包含在 Captis 範圍內）。 某些特定材料可能需要在 Sampler 中進行額外處理以優化結果。 請注意，處理演算法將持續優化。

+++

+++材料樣本大小或形狀有什麼限制——樣品是否必須是平坦的？
Captis 可以掃描各種大小或形狀的材料樣本。 它會附帶磁鐵，用來壓扁樣品托盤上的樣本。 使用 Captis 有多種採集材料樣本的模式：

* 攝影棚模式：無論在你的桌上、錄音室或工廠裡，Captis 都能取樣尺寸達 30cm x 30cm，並搭配背光以提升不透明度。 樣本托盤深度為1.8公分。

* 探索模式：你可以在現場、片場或特殊環境中使用探索環，並啟用超過 30cm x 30cm 的樣本的彈性捕捉。 目前限制：請注意，探索模式仍處於早期版本，尚未優化（截至 2024 年 7 月 29 日發行）。

+++

## 軟體

+++HP Z Captis 裝置需要軟體訂閱或授權才能使用嗎？
Captis 裝置需持有有效的 Substance 3D Sampler Enterprise、Teams 或 University 授權，且該授權在 Substance 3D Collection 中可取得，條件與使用條款與 Substance 3D 訂閱相同。

裝置（HP Z Captis）與授權（Substance 3D Sampler）是分開販售的。

+++

+++Adobe 的 Substance 套件整合程度如何？
HP Z Captis 裝置完全由 Adobe Substance 3D 取樣器控制與操作：你可以從 Substance 3D 取樣器預覽並啟動擷取，擷取完成後會自動將 PBR 通道載入為圖層並建立 3D 材質。 你可以繼續使用Sampler中所有可用的工具和濾鏡來處理你的材料。

一旦你捕捉到的素材進入 Substance 3D Sampler，你可以將其匯出到 Substance 3D 套件中的任何應用程式（Substance 3D Designer、Painter、Stager）以及任何支援 Substance 的第三方應用程式，包括 3DS Max、Maya、Blender、Unreal Engine、CLO、Browzwear、VRED、Rhino、Cinema4D 等（完整列表請見此處：<https://www.adobe.com/tw/products/substance3d/plugins.html>）。

+++

+++使用 Substance 3D Sampler 搭配 Captis 的建議規格是什麼？
取樣器硬體規格可在此[&#128279;](system-requirements-to-use-hp-z-captis.md)查閱。

+++

+++HP Z Captis 的工作流程在 Windows 和 Mac 上都能使用嗎？
截至 2025 年 2 月 20 日版本，搭配 HP Z Captis 的 Sampler 工作流程僅支援 Windows。

+++

+++我在哪裡可以找到 Substance 3D Sampler 搭配 HP Z Captis 工作流程的版本？
自 2025 年 2 月 20 日版本起，你可以透過 Captis 的 Adobe Substance 3D Sampler 工作流程，作為從 Creative Cloud 桌面應用程式下載的 Substance 3D Sampler 常規編譯的一部分。 現在不需要再從 Adobe 預發布版下載它們。

+++

+++哪些還沒上市？
*截至 2025 年 8 月（Sampler 5.1.0 版本）的限制：*

* 目前 HP Z Captis 的 Sampler 工作流程僅支援 Windows。

* 目前匯出的五張地圖分別是基底色、粗糙度、法線、高度、不透明度。

* 探索模式仍是早期版本，尚未優化。

* 平鋪是在取樣器層堆疊中使用目前平鋪濾波器進行的。

+++

+++有哪些PBR頻道可以使用？
截至 2025 年 8 月 7 日的發行，匯出的五張地圖分別是基礎色、粗糙度、法線、高度和不透明度。 目前的處理流程尚未處理金屬性地圖。

+++

+++磁磚是自動完成的嗎？
平鋪是在取樣器層堆疊中使用目前的平鋪濾波器執行的。

自動平鋪濾波器可用於自動鋪設具有明確重複結構或小圖案的材料，每個方向至少有三個圖案。 想了解更多關於這個過濾器的資訊，請參閱 [文件](../../filters/tools/auto-tiling.md)的專屬章節。

+++

+++掃描後的資料可以匯出哪些格式？
HP Z Captis 由 Adobe Substance 3D Sampler 原生操作。 HP Z Captis 可擷取 64 張原始影像（可從本地資料夾擷取）及 PBR 地圖（由原始影像處理後自動載入 Substance 3D Sampler）。 Substance 3D Sampler 會根據擷取後自動載入 Sampler 圖層堆疊的 PBR 通道，建立一個 3D 材質。

從 Adobe Substance 3D Sampler，你可以以 Substance 3D Sampler 中任何可用的匯出格式匯出你的數位素材：作為 Substance 檔案（.SBS 和 .SBSAR 檔案）或以點陣貼圖，包括 .PNG、.JPG、.TIFF......（詳情請參見 Sampler 文件網頁：[https://helpx.adobe.com/tw/substance-3d-sampler/getting-started/export.html](../../getting-started/export/export.md)）。

+++

+++在拍攝時，LDR 和 HDR 有什麼不同？
預覽時，你可以選擇輸出類型，選擇低動態範圍（LDR）和高動態範圍（HDR）。\
即使選擇遠距離，HDR 地圖也會被擷取並儲存在你的裝置上。\
建議你選擇 LDR，這樣可以在 Sampler 以及任何會使用 sbsar 檔案的第三方應用程式中，讓專案的大小更容易管理。

+++

## 處理中

+++如果我使用特定的檔案格式、標準與規範，或是第三方應用程式，我該如何在目前的 3D 流程中使用 Captis？
HP Z Captis 由 Adobe Substance 3D Sampler 原生操作。 一旦你在 Substance 3D Sampler 中擷取並數位化你的材料樣本，就能無縫匯出你的數位材料：

在 Substance 3D 生態系統的任何應用中（包括支援多種匯出格式的 Substance 3D Designer 或 Substance 3D Painter：https://experienceleague.adobe.com/en/docs/substance-3d/general-knowledge/ecosystem/import-and-export-formats）。

在任何整合 Substance 檔案格式的應用程式中，如 3DS Max、Maya、Blender、C4D、Rhino、Browzwear、CLO......（完整列表請見此處：<https://www.adobe.com/tw/products/substance3d/plugins.html>）。 如果你使用的應用程式未列入該格式，也可以匯出 PBR 材質圖片，手動插入任何原生不支援 Substance 檔案格式的應用程式中。

+++

+++製作地圖需要拍攝多少張照片？
[8 個燈面板 + 1 個背光] x [8 個偏振狀態] x [8 次 HDR 包圍曝光] x [4 次超幅以降低雜訊] = 2048 + 256（背光）

+++

## 裝置管理

想了解更多關於裝置及其規格，請造訪[惠普官網](https://www.hp.com/us-en/workstations/z-captis.html "HP Z Captis")。

+++我可以更改裝置的 IP 位址嗎？
要更改裝置的 IP 位址，可以透過新增一行程式碼修改 Windows 檔案 C：\Windows\System32\drivers\etc\hosts.txt：

例如你可以新增 192.168.55.1 captis-device，然後在 <b>Sampler 的設定>儲存與快取>素材擷取 Captis 位址</b> >將 IP 換成 captis-device。

+++

## 使用問題

+++Sampler 無法偵測到 HP Z Capti。
確定 HP Z Captis 是接到 USB 3.0 埠。

確保 USB 線是接在 HP Z Captis 的底座上，而不是接在錐形上。

+++

+++我的預覽在取樣視窗裡完全是黑色的。
確保你已經拆掉攝影機保護裝置。

+++

+++從 HP Z Captis 複製檔案到我的電腦很慢。
確定 HP Z Captis 是接到 USB 3.0 埠。

如果你要求同時取得材料和光度影像，複製過程通常會花更多時間。

+++

+++Sampler 沒有把圖片複製到我的電腦。 我需要重新開始掃描嗎？
不，你沒有。 你可以瀏覽裝置內容，並透過作業系統的檔案總管複製 Adobe 資料夾中的圖片。

+++

+++選單顯示裝置處於恢復模式。
按電源鍵幾秒鐘就能關機。 再打開一次。

+++

+++我把錐筒從底座移到探測環，結果無法再掃描了。
建議在拔掉 HP Z Captis 從底座或瀏覽器環拔除前，先關閉它。

+++

+++在 SBSAR 匯出資料很慢。
請確保圖片在屬性面板中不是 32 位元浮點格式。

你也可以把壓縮等級設成「無」來加快匯出速度。

+++

+++我想更改捕捉材質和光度測量影像的儲存路徑。
現在可以在「編輯>偏好設定」>「儲存與快取」>素材擷取中編輯擷取材料與光度影像的儲存位置。

+++

+++視窗比螢幕還大，我無法調整大小。
Captis 視窗確實無法調整大小。 你可能用的是沒有處理的螢幕放大倍率。 Captis 支持以下內容：

* 解析度：1920x1080
  * 最大放大倍率：100%

* 最大放大倍率：100%

* 解析度：2560x1440
  * 最大放大倍率：125%

* 最大放大倍率：125%

* 解析度：3840x2160
  * 最大放大倍率：200%

* 最大放大倍率：200%

* 低於 1920x1080 的解析度不支援。



+++
