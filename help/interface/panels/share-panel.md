---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/interface/panels/share-panel.html"
breadcrumb-title: ''
description: 學習如何使用 Substance 3D Sampler 的匯出面板，將材質匯出成檔案或直接傳送到其他應用程式。
helpx_creative_field: ""
helpx_description: Sampler > Interface > Panels > Export panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 匯出面板
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 1%

---


# 匯出面板

<b>匯出面板</b>是你可以匯出資產成一般檔案或直接傳送到其他應用程式的地方。

## 傳送至...

「傳送至...」選項允許你直接將資產傳送到系統上安裝的其他應用程式。 這通常比進出口資產快得多。

目前 Sampler 支援傳送至：

* **Substance 3D Painter**：匯入材質和環境，讓你在素材貼圖時可以使用。
* **Substance 3D Stager**：匯入環境燈光以改變場景氛圍。 僅在環境燈下使用，且材料無法使用。

材料總是以 SBSAR 形式傳送，環境則以 EXR 形式傳送。

## 匯出

點擊 **匯出為......** 以匯出你目前正在製作的資產。 從左側選單選擇要修改一般設定還是材質設定。

### 一般設定

選擇一般設定後，你可以更改材質名稱和存檔位置。 你也可以切換是否要為素材建立子資料夾。 這在匯出產生多個檔案的影像格式時非常有用。

### 材質設定

選擇材質設定後，你可以調整各種參數來控制材質的匯出方式：

| 背景設定 | 說明 |
| --- | --- |
| 格式 | 可選擇匯出為 SBS、SBSAR，或是以特定影像格式匯出的影像集合 |
| 預設集 | 選擇預設，自動組織特定應用程式的匯出。 [更多關於預設的資訊請見此](../../getting-started/export/default-presets/default-presets.md)處。 預設只有在選擇影像格式時才可用。 |
| 壓縮 | 選擇壓縮優先考量速度還是效率 <br> <ul> <li> **自動**：讓取樣者選擇。 <li> **最佳方案**：最大化較小檔案的壓縮效率。 <li> **無：**&#x200B;沒有壓縮代表匯出檔案開啟和關閉速度較快，但檔案大小會變大。 </ul> |
| 解決方法 | 更改你的匯出解析度。 這個選項會根據選擇的格式而有所不同 <br> <ul> <li> **SBSAR/SBS**：選擇材質的預設寬度與高度。 這些資料可以之後再更新。 <li> **圖片格式**：選擇 **圖層輸出（Layers output** ），將每個地圖匯出到依圖層堆疊定義的大小，或 **覆蓋所有** 圖層，讓你能指定寬度和高度以供匯出。 |
| 材質模型 | 選擇匯出為 Adobe 標準材質或 OpenPBR 材質。 你選擇哪個選項，應該取決於你管線中還使用哪些其他應用程式。 根據材質模型，將開放不同的通道。 |
| 管道 | 切換哪些頻道應該匯出到你的資產中。 |

>[!NOTE]
>
> 欲了解更多關於匯出對話框選項及檔案格式等資訊，請參閱[匯出](../../getting-started/export/export.md)文章[&#128279;](../../getting-started/export/export-window/export-window.md)及其子條目（匯出視窗）。

當你對匯出設定滿意後，點擊 **匯出**。 你的匯出會出現在匯出佇列中，佇列會顯示最近的匯出清單。 點擊任何匯出時的資料夾圖示，即可開啟該匯出的檔案位置。
