---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/old-versions/version-0-7-0.html"
breadcrumb-title: ''
description: 請參閱 Substance 3D Sampler 0.7.0 版本的發行說明，了解更新、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Old Versions > Version 0.7.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 版本 0.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---


# 版本 0.7.0

上映日期： **2019/06/13**

補充：

* [篩選器]按空白鍵快速進入你的篩選器
* [篩選器]新的專用面板用來管理、瀏覽及匯入你的篩選器
* [元資料]右鍵點擊素材以查看其元資料
* [元資料]右鍵點擊素材以查看其在磁碟上的位置
* [滑桿]按 Ctrl 鍵將滑鼠懸停時，讓滑桿動畫化
* [滑桿]按下 P 鍵停止並重新啟動滑桿動畫
* [出口]SBSAR出口遵循物質來源指引
* [授權]使用環境變數啟動物質煉金術師
* [UX]檔案對話框會記住最後選擇的檔案路徑
* [UX]資料夾對話框會記住最後選擇的資料夾路徑
* [使用者介面]更新資源面板 UI
* [使用者介面]更新搜尋欄 UI
* [使用者介面]新增素材圖示已更新
* [求助]網址已更新至 [substance3d.com](http://substance3d.com) 網域
* [網格]布網現已推出
* [內容]新腐蝕過濾器
* [內容]新氧化過濾器
* [內容]新苔蘚過濾器
* [內容]新塵埃過濾器
* [內容]新磚牆模式濾波器
* [內容]新石牆模式濾波器
* [內容]新木質飾面過濾器
* [內容]新金屬處理濾網
* [內容]新雪濾
* [內容]新隨機濾波器
* [內容]你現在可以直接在基底材質過濾器中匯入你的貼圖

修正：

* 修復儲存層堆疊時的崩潰
* 可以在環境旋轉滑桿中加入高於 1 的值
* 當混合圖層在不同素材圖層之間來回轉換時，不要失去混合參數
* 在產生同一層堆疊多次變體時，修正重複問題
* 重新開啟材料時，煉金術士會記住你調整過的滑桿範圍（最小值和最大值）

已知問題：

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 不建議快速切換 Delighter 舞台
* 自訂環境匯入可能會變成黑色
* Tif 影像在 Image 匯入圖層的屬性面板中沒有顯示
* 在滑桿中輸入特定值時，可以忽略逗點或點
* 在 MacOS 上，法線到高度過濾器可能會當機
