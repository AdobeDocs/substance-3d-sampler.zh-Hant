---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/release-notes/old-versions/version-0-8-0.html"
breadcrumb-title: ''
description: 請參閱 Substance 3D Sampler 0.8.0 版本的發行說明，了解新功能、更新與改進。
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Old Versions > Version 0.8.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 版本 0.8.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---


# 版本 0.8.0

**補充：**

* [資源]將你的材料資料夾連接並鏡像到本地磁碟
* [資源]瀏覽你的資料資料夾及其子資料夾
* [資源]將你的材料資源面板分開到另一個視窗，就能全螢幕查看你的資源
* [資源]新資源面板版面以支援資料夾及子資料夾導航
* [資源]利用麵包屑瀏覽你的資料夾
* [資源]強制同步你的本地資料夾，並透過點擊可開啟的同步選項
* [資源]使用「斷線」選項，透過右鍵點擊解除連結，解除您的本地資料夾
* [管理]顯示Substance檔案的嵌入標籤
* [管理]新增、編輯及刪除你資料的標籤
* [管理]評分你的材料
* [圖層]支援全景輸出
* [圖層]你可以在 Image 匯入圖層中刪除圖片輸入
* [圖層]自動選擇新增圖層
* [圖層]圖層刪除後自動選擇下方圖層
* [用戶體驗]切換到其他實驗室時，保持左側面板的可見性
* [使用者體驗]匯入非空圖層堆疊中的圖片時，請勿建立基底圖層或開啟材質工作流程彈窗
* [使用者介面]新的文字欄位樣式
* [使用者介面]新搜尋框風格
* [使用者介面]新面板標頭樣式
* [使用者介面]新的忙碌指示器風格
* [使用者介面]新圖層堆疊背景樣式
* [使用者介面]使用 Adobe Clean 字型
* [使用者介面]移除滴管圖示中顏色輸入參數的佔位符
* [效能]忙碌指標優化
* [內容]新模式產生器濾波器
* [內容]新模糊濾鏡

**修正：**

* [啟發]修正使用超過10種顏色時的崩潰
* [2D 視圖]在 2D 視圖的頻道列表中固定滾動條
* [檢視器]修正匯入非2次方環境貼圖時的崩潰問題
* [內容]修正 PNG 匯入以支援壓紋與穿孔濾鏡的自訂圖案
* [匯出]修正法線，且每個通道匯出高度為 16 位元
* 在匯入兩個同名預設的材質時，修正無限迴圈
* 修正基礎材質圖層中長檔案路徑顯示的問題

**已知問題：**

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 不建議快速切換 Delighter 舞台
* Tif 影像在 Image 匯入圖層的屬性面板中沒有顯示
* 在滑桿中輸入特定值時，可以忽略逗點或點
* 在 MacOS 上，法線到高度過濾器可能會當機
* 在 MacOS 上退出時可能會隨機當機
