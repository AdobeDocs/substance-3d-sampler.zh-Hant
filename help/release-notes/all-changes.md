---
helpx_url: 'https://helpx.adobe.com/tw/substance-3d-sampler/release-notes/all-changes.html'
breadcrumb-title: ''
description: 檢視 Substance 3D Sampler 版本的所有變更與更新，以追蹤功能隨時間的演進與改進。
helpx_description: Sampler > Release Notes > All Changes
title: 所有變動
user-guide-description: ''
user-guide-title: ''
source-git-commit: 275dc218870f111aa99533840a5aea4c3d22f0cf
workflow-type: tm+mt
source-wordcount: '24964'
ht-degree: 0%
---

# 所有變動

本頁彙整了 Substance 3D Sampler 所有的變更，從新功能到錯誤修正。

## 版本 6

### **6.0.4**

*（發行日期：2026年9月24日）*

**變更**
[引擎] 更新物質引擎至 9.6.1

**固定**
[將影像加入浮雕遮罩時，圖層] 崩潰
[安全] 通用修正

### **6.0.3**

*（發布日期：2026年8月24日）*

**修正：**

[Rendering] 還原 NVIDIA 驅動程式故障的臨時解決方法

### **6.0.2**

*（發布日期：2026年6月25日）*

**補充：**

* &lbrack;Assets&rbrack;請檢查 sbsar 版本並提醒使用者引擎太舊無法讀取
* &lbrack;Captis&rbrack; 在偏好設定中新增儲存 captis 光度測量的選項

**修正：**

* &lbrack;2D View&rbrack;若關閉實體尺寸，請勿「以物理比例顯示」
* &lbrack;Analytics&rbrack;缺少分析事件
* &lbrack;Analytics&rbrack;防止 crashpad 在 vk devicelost 上回報當機
* &lbrack;Application&rbrack;退出時不要摧毀 vkdevices，以避免 NVIDIA 驅動程式當機
* &lbrack;Application&rbrack; 修正連結集合監視者退出 + 通道管理器
* &lbrack;Application&rbrack; 防止出口當機
* &lbrack;Content&rbrack;「金屬表面處理」濾網不會影響金屬性
* &lbrack;Content&rbrack; 在動態過濾器中缺少實體大小時，會新增實體大小
* &lbrack;Filters&rbrack; 從隱藏資產列表中移除內容感知填充
* &lbrack;Layers&rbrack;點擊「重置所有設定」不會重置「apply to」下拉選單
* &lbrack;Layers&rbrack; 修正位置小工具的最小與最大調整
* &lbrack;Layers&rbrack; 正確更新過濾器
* &lbrack;Physical Size&rbrack;確保物理尺度在各處都能正常運作 + 讓 Physicalsize 在動態過濾器下變得合理
* &lbrack;Project&rbrack;建立新資產時，確保資產解析度為預設（2k x 2k）
* &lbrack;Project&rbrack;重新開啟現有專案，過去用來開啟舊版本
* &lbrack;Project&rbrack;Sampler 不再提供還原損壞專案的備份
* &lbrack;Rendering&rbrack; 最高解析度為 2k 的渲染材質縮圖
* &lbrack;UI&rbrack;防禦性程式碼，防止使用者速度快於 UI 時當機

### **6.0.1**

*（發行日期：2026年5月21日）*

**補充：**

* &lbrack;Application&rbrack;在開啟包含 3D 物件或環境燈的專案時，提醒使用者
* &lbrack;Captis&rbrack;讓使用者介面適應小螢幕
* &lbrack;Captis&rbrack; 更新Captis UI
* &lbrack;頻道設定&rbrack;在 ASM 中使用 SSS 頻道時，會自動啟用 SSS
* &lbrack;Engine&rbrack;更新物質引擎至版本 9.4.3
* &lbrack;Preset&rbrack;預設開啟「套用預設縮圖值」
* &lbrack;Resources&rbrack;預設顯示「所有函式庫」，而不是在資源面板中顯示「起始資產」
* &lbrack;Scripting&rbrack; 新增 Python 函式以管理圖層的「套用」
* &lbrack;UI&rbrack;資產列表現在是響應式：資產大小會隨容器調整
* &lbrack;UI&rbrack;預設顯示 3D/2D 視圖
* &lbrack;UI&rbrack;從檔案總覽丟棄材質時，顯示材質優化彈窗
* &lbrack;UI&rbrack; 啟用翻轉裝置列按鈕工具提示

**修正：**

* &lbrack;Application&rbrack; 修正色彩空間問題
* &lbrack;Application&rbrack; 修正設定更新器
* &lbrack;Application&rbrack;當掃描通道設為自動時，請啟用它們
* &lbrack;Application&rbrack;主畫面的新專案按鈕不再會刪除同名的先前專案
* &lbrack;Application&rbrack; 防止 macOS 退出時當機
* &lbrack;Application&rbrack; 防止存取無效資產參考的資產
* &lbrack;Application&rbrack; 防止在調整中從 VersionedImage 存取表面時當機
* &lbrack;Application&rbrack; 在刪除關卡時防止當場崩潰
* &lbrack;Captis&rbrack;確保 Captis 在關閉 Sampler 前已斷開
* &lbrack;Captis&rbrack;防止 USB-2 警告重複顯示
* &lbrack;頻道設定&rbrack; 修正 OpenPBR 頻道名稱
* &lbrack;頻道設定&rbrack;更新OpenPBR頻道的長標籤
* &lbrack;內容&rbrack;將所有網格單元從公尺更新到公分以符合 SSS 值
* &lbrack;Export&rbrack; 確保預設值已接入動態過濾器
* &lbrack;Export&rbrack;圖片現在會儲存在工作者執行串中以提升效能
* &lbrack;Filters&rbrack; 內容感知填充在開啟縮放時會當機
* &lbrack;Filters&rbrack; 無法從資產面板開啟動態過濾器的位置
* &lbrack;Filters&rbrack; 修正 AutoTiling 調整步驟中的全部重置
* &lbrack;Filters&rbrack; 還原 在樹狀結構建立時停用使用處理
* &lbrack;Filters&rbrack; 設定升頻參數的正確預設值
* &lbrack;Filters&rbrack;即使產生器位於填充層，也能更新它們
* &lbrack;Layers&rbrack;禁止重新命名輸入層標頭或佔位圖層
* &lbrack;Layers&rbrack; 防止因懸掛指標而導致層插入時崩潰
* &lbrack;Layers&rbrack; 平面圖層名稱中圖片數量錯誤
* &lbrack;Localization&rbrack; 確保切換語言時預設名稱會更新
* &lbrack;在地化&rbrack;資源面板中多重翻譯問題
* &lbrack;Localization&rbrack;快速動作分類在地化問題
* &lbrack;Performance&rbrack;僅在開啟區段進行負載調整
* &lbrack;Preferences&rbrack; 清除偏好快取路徑會重置為先前的值
* &lbrack;Rendering&rbrack;使用路徑追蹤器時的記憶體洩漏
* &lbrack;Rendering&rbrack;在 Vulkan 仍可存取時，防止刪除材質
* &lbrack;Rendering&rbrack;紋理旋轉未從 0-1 轉換為 0-360
* &lbrack;Scripting&rbrack;從 Python 文件中移除不存在的類別
* &lbrack;Scripting&rbrack; 如果沒有選取資產，則 selectAsset 回傳 N
* &lbrack;Tools&rbrack;重置貼圖值現在會停止繪製並清除補丁視圖
* &lbrack;UI&rbrack;在調整內容時，不要關閉屬性面板中的區塊
* &lbrack;UI&rbrack; 懸停時隱藏的顏色調整標籤
* &lbrack;UI&rbrack; 修正資產列表響應式行為
* &lbrack;UI&rbrack; 修正 AssetItem 工具提示中的綁定迴圈
* &lbrack;UI&rbrack; 修正：雙擊選取的預設群組
* &lbrack;UI&rbrack; 固定影像呈現器中的下落區域
* &lbrack;UI&rbrack;修正標籤，裡面有按鈕，適用於所有語言
* &lbrack;UI&rbrack; 頻道列表中日語線路高度固定彈出視窗
* &lbrack;UI&rbrack; Fix onAccepted 訊號長度欄位
* &lbrack;UI&rbrack; 修正左側控制項長的彈出視窗寬度
* &lbrack;UI&rbrack; 修正資產項目中的預覽彈出視窗
* &lbrack;UI&rbrack;修正粗糙/反光挑選器
* &lbrack;UI&rbrack; 修正字串省略號
* &lbrack;UI&rbrack; 修正字串截斷問題
* &lbrack;UI&rbrack; 修正開關調整重置按鈕
* &lbrack;UI&rbrack;當選擇自訂匯出預設時，隱藏材質模型下拉選單
* &lbrack;UI&rbrack; 在匯出彈出視窗中移除通道列表中的解析度
* &lbrack;UI&rbrack; 重置為預設版面會保留投影檢視器的設定
* &lbrack;UI&rbrack;還原「在 Photoshop 編輯」和「在 Illustrator 編輯」選單項目

**已移除：**

* &lbrack;UI&rbrack; 移除影像匯入圖層的「Applied to」區段
* &lbrack;UI&rbrack;首次啟動時移除自動開啟快速動作提示

## 版本 5

### **5.1.3 浮島**

*（發布日期：2026年1月6日）*

**補充：**

* &lbrack;Captis&rbrack;若防火牆禁用 FTP 協定，則顯示警告

**修正：**

* &lbrack;Captis&rbrack;在捕獲過程中中止可能導致錯誤
* &lbrack;Captis&rbrack;擷取結束時下載結果會消耗太多記憶體
* &lbrack;Captis&rbrack;在自動強度後立即執行自動對焦可能導致錯誤
* &lbrack;Captis&rbrack;HDR 結果顯示於摘要面板中
* &lbrack;UI&rbrack;在某些情況下，MacOS 的資料夾對話框不會選擇正確的資料夾

### **5.1.2 漂流島**

*（發布日期：2025年11月20日）*

**補充：**

* &lbrack;Application&rbrack;偵測顯示裝置遺失，警告使用者並優雅地退出
* &lbrack;Layers&rbrack;圖層扁平時的訊息傳遞改善
* &lbrack;Layers&rbrack;改進的圖片匯入與扁平圖層縮圖
* &lbrack;Onboarding&rbrack;主畫面更新學習內容
* &lbrack;Project&rbrack; 恢復崩潰前最後儲存的會話狀態
* &lbrack;UI&rbrack; 應用程式圖示更新

**修正：**

* &lbrack;Application&rbrack;在 macOS 上插入材質在圖層堆疊中可能會導致當機
* &lbrack;Application&rbrack;macOS 重負載時可能當機
* &lbrack;Application&rbrack;當視訊記憶體滿時，增加圖層時可能當機
* &lbrack;Application&rbrack;開啟專案時可能當機
* &lbrack;Captis&rbrack;自動對焦在自動強度校正後不久啟動時會失效
* &lbrack;Captis&rbrack;首次捕獲後的可靠性與效能問題
* &lbrack;Captis&rbrack;擷取結束時複製檔案時的延遲與錯誤
* &lbrack;Captis&rbrack;查詢 Captis 裝置資訊時有小記憶體洩漏
* &lbrack;Export&rbrack;多重滑桿暴露參數會產生損壞的 .sbsar 檔案
* &lbrack;Layers&rbrack;自動平鋪模式在切換資產時會重置為預設值
* &lbrack;Layers&rbrack;預設自訂基色顯示為紅色
* &lbrack;Layers&rbrack;部分壓平克隆印章子圖層是可能的，這會導致渲染問題
* &lbrack;Layers&rbrack;渲染過程中調整圖層堆疊時可能會當機
* &lbrack;Layers&rbrack;切換來源通道時，自動平鋪感興趣區域步驟出現意外錯誤
* &lbrack;Project&rbrack;建立新材質時有時縮圖錯誤
* &lbrack;快速動作&rbrack;有些快速動作輸入次數錯誤
* &lbrack;UI&rbrack;動作群組按鈕有不同寬度
* &lbrack;UI&rbrack;文字欄位中的清除按鈕有時會觸發焦點喪失
* &lbrack;UI&rbrack;組合框和文字欄位太大了
* &lbrack;UI&rbrack;圖示與標籤錯位
* &lbrack;UI&rbrack;名稱欄位標籤放置錯誤
* &lbrack;UI&rbrack;快速動作按鈕標籤錯位
* &lbrack;UI&rbrack; 滑桿顯示 0 後方 0

**已移除：**

* &lbrack;生成式 AI &rbrack;生成式 AI 功能移除。 *此功能已從應用程式中移除，服務將於 3 月 5 日起停止在先前版本的 Sampler 中運作。*

### **5.1.1 漂流島**

*（發行日期：2025年9月18日）*

**補充：**

* &lbrack;2D 視圖&rbrack;能在 2D 視圖中放大更多，以呈現高解析度材質
* &lbrack;Captis&rbrack;提醒使用者複製檔案時的問題
* &lbrack;Layers&rbrack;在複製圖層時，在新圖層名稱中使用遞增數字

**修正：**

* &lbrack;2D View&rbrack;在重置 Clone Stamp 的所有屬性後繪製筆觸時，先前建立的筆劃會重新出現
* &lbrack;Application&rbrack;「儲存目前專案？」 彈出視窗使用錯誤的專案名稱
* &lbrack;Application&rbrack;出口崩潰
* &lbrack;Application&rbrack;潛在崩潰
* &lbrack;Application&rbrack;有時會產生錯誤材質的縮圖
* &lbrack;Captis&rbrack;在某些裝置上，執行高解析度掃描時，高度圖呈現黑色
* &lbrack;Captis&rbrack;當未設定擷取名稱且校正進行時，「開始擷取」按鈕不再被禁用
* &lbrack;Export&rbrack;當匯出 .sbsar 檔案時，匯出可能會失敗，使用者不會被通知
* &lbrack;Filters&rbrack;自動平鋪濾波器的進階參數畫面在調整參數時有時會閃爍
* &lbrack;Filters&rbrack;平鋪濾波器的預設參數會在輸出中產生灰色瑕疵
* &lbrack;Filters&rbrack;有時在高解析度輸入下，自動平鋪濾波器的進階設定不會顯示各個圖案點
* &lbrack;Filters&rbrack;自訂大小自動平鋪參數的模式大小預設值錯誤
* &lbrack;Layers&rbrack;偶爾會出現自動平鋪濾鏡的色彩問題，主要出現在紅色材質上
* &lbrack;Layers&rbrack;有時新增圖層會將部分調整重置回預設值
* &lbrack;實體尺寸&rbrack;具有實體大小的資產縮圖高度比例尺錯誤
* &lbrack;UI&rbrack; 無法重新命名暴露參數
* &lbrack;UI&rbrack;頻道啟動按鈕不是方形的
* &lbrack;UI&rbrack;如果滑桿標籤太長，重置按鈕無法使用。
* &lbrack;UI&rbrack; 按下回車鍵或點擊退出不會移除文字欄位的焦點
* &lbrack;UI&rbrack;有時會在實體尺寸面板中出現不想要的工具提示
* &lbrack;UI&rbrack;3D 視圖在建立空專案時顯示的網格不正確
* &lbrack;UI&rbrack;當顯示色彩選擇器輸入時，其標籤在滑鼠懸停時會消失
* &lbrack;UI&rbrack;在暴露參數時，色點有時會被錯誤定位

### **5.1.0 ÎLE FLOTTANTE**

*（發行日期：2025年8月7日）*

**補充：**

* &lbrack;2D 視圖&rbrack;筆刷大小現在會自動調整到目前的材質解析度
* &lbrack;3D 視圖&rbrack;在偏好設定中切換 3D 渲染的原生顯示縮放
* &lbrack;Application&rbrack; 渲染引擎更新
* &lbrack;Captis&rbrack;預覽時新增「make square」選項
* &lbrack;Captis&rbrack;自動物理尺寸偵測
* &lbrack;Captis&rbrack;捕捉新材料將產生新資產
* &lbrack;Captis&rbrack;在下拉選單中將解析度選擇改為每英吋或每公分像素，而非最大面積的像素解析度
* &lbrack;Captis&rbrack;對齊校正的上下文協助
* &lbrack;Captis&rbrack; 產生粗糙度地圖
* &lbrack;Captis&rbrack;如果預設校正檔案遺失，請提醒使用者
* &lbrack;Filters&rbrack;結構材料與掃描自動平鋪濾波器
* &lbrack;濾網&rbrack;新摺痕去除濾器
* &lbrack;Filters&rbrack; 克隆印章過濾器中的新功能
* &lbrack;Filters&rbrack;Equalize 濾波器中的新功能
* &lbrack;Layers&rbrack;能夠將圖層壓平
* &lbrack;Layers&rbrack;右鍵點擊圖層時的右鍵選單，可重新命名、複製、刪除或扁平該圖層
* &lbrack;Onboarding&rbrack;更新歡迎及最新畫面內容
* &lbrack;Performance&rbrack;使用裁切濾鏡時的效能更好
* &lbrack;Performance&rbrack;改善 3D 視圖的記憶體使用率
* &lbrack;Performance&rbrack;更新3D視圖更快
* &lbrack;物理尺寸&rbrack;在處理物質過濾器時啟用「物理尺寸顯示」
* &lbrack;物理尺寸&rbrack;在匯入空堆疊中的影像時，建議一個與影像比例更為一致的解析度
* &lbrack;快速動作&rbrack;三個新的快速掃描處理動作
* &lbrack;Scripting&rbrack; API 以平整圖層
* &lbrack;Scripting&rbrack; 取得每個影像匯入圖層的檔案名稱
* &lbrack;Scripting&rbrack; 新增功能，用於啟用/停用資產的指定通道
* &lbrack;UI&rbrack;重新設計圖示與按鈕，以配合新功能
* &lbrack;UI&rbrack;警告環境光繪製棄用

**修正：**

* &lbrack;2D View&rbrack;選擇「以物理比例顯示」可能無法使用物質過濾器
* &lbrack;3D Capture&rbrack;Svg 檔案會列在檔案選擇器中，但不支援
* &lbrack;3D View&rbrack;著色器設定中的發射強度參數無法運作
* &lbrack;3D View&rbrack;有時建立新資產時網格位置會不正確
* &lbrack;3D View&rbrack;切換到路徑追蹤渲染在不支援的硬體上會當機
* &lbrack;Application&rbrack;應用程式在關閉手動量表彈窗時會當機，但未設定尺寸
* &lbrack;Application&rbrack; 崩潰
* &lbrack;Application&rbrack; 在顯示桌面時（Windows 鍵 + D 鍵快捷鍵）在 Windows 上凍結
* &lbrack;Application&rbrack;切換語言時可能當機
* &lbrack;Captis&rbrack;當預覽資料無效時會當機
* &lbrack;Captis&rbrack;放大後無法完全縮小
* &lbrack;Captis&rbrack;缺少某些精靈步驟的本地化
* &lbrack;Captis&rbrack;使用Captis時可能在出口時當機
* &lbrack;Captis&rbrack;如果裝置缺少校正檔案，掃描就無法運作
* &lbrack;Filters&rbrack; 使用 Clone Stamp 濾波器時，筆刷預覽可能會因材質和筆刷大小而錯誤
* &lbrack;Filters&rbrack; 使用升頻濾波器後輸出大小錯誤
* &lbrack;Filters&rbrack;缺少環境旋轉與風格化濾鏡的圖示
* &lbrack;Filters&rbrack;更新部分濾鏡可能導致錯誤渲染
* &lbrack;Layers&rbrack;混合兩個材質時第一次渲染錯誤
* &lbrack;Layers&rbrack;更新圖層的按鈕顯示「全部更新」，即使只有一次更新
* &lbrack;Layers&rbrack; 在圖層堆疊中匯入影像時的不必要計算
* &lbrack;Performance&rbrack;改進法線貼圖格式處理以縮短渲染時間
* &lbrack;實體尺寸&rbrack;手動測量彈出視窗只有在自動測量後才會生效
* &lbrack;實體尺寸&rbrack;當啟用實體尺寸時，匯出彈窗的匯出解析度錯誤
* &lbrack;快速動作&rbrack;產生的資產名稱缺少本地化
* &lbrack;UI&rbrack;資產預覽在滑鼠懸停時可能不會顯示
* &lbrack;UI&rbrack; 點擊重置為預設值按鈕可能會破壞部分控制功能
* &lbrack;UI&rbrack;切換專案時不會清除錯誤訊息
* &lbrack;UI&rbrack;確保當沒有資產時，視窗和屬性面板的材質名稱是空的
* &lbrack;UI&rbrack; 視角參數的重置為預設值按鈕無法運作
* &lbrack;UI&rbrack; 重置為預設值，按鈕重疊
* &lbrack;UI&rbrack;面板脫離底座時，有些按鈕無法點擊
* &lbrack;UI&rbrack; 貼圖耕耘 V 參數部分隱藏於檢視器設定與 3D 檢視中

**已移除：**

* &lbrack;3D 擷取&rbrack;移除 3D 擷取支援
* &lbrack;Application&rbrack; 移除 macOS x86 支援

### **5.0.3 榛果**

*（發布日期：2025年6月3日）*

**補充：**

* &lbrack;Captis&rbrack;允許將材料命名為與已存在材料相同的名稱
* &lbrack;Captis&rbrack;將錯誤訊息移至彈出視窗而非吐槽
* &lbrack;Filters&rbrack;更新刺繡
* &lbrack;偏好設定&rbrack; 新增檢視器設定與著色器設定中的重置
* &lbrack;UI&rbrack;不要在專案資產上顯示「顯示位置」選單項目

**修正：**

* &lbrack;3D Capture&rbrack;網格後製濾鏡無法輸出預期的地圖
* &lbrack;3D 檢視與rbrack;3D 視圖因著色器快取損壞而無法運作
* &lbrack;3D 視圖&rbrack;當場景Z-up時，地面平面和網格是垂直的
* &lbrack;3D 視圖&rbrack;網格有時會消失
* &lbrack;Application&rbrack;啟動時關閉登入視窗但未登入，有時會讓應用程式當機
* &lbrack;Application&rbrack;當插件設定檔被拒絕存取時會當機
* &lbrack;Application&rbrack;當專案儲存時，目前資料會被取消選取
* &lbrack;Application&rbrack;重置為預設版面時，解析度會設定為 64x64
* &lbrack;Application&rbrack;Sampler 有時在渲染圖層堆疊時會當機
* &lbrack;Export&rbrack;匯出解析度有時會重置為 64x64
* &lbrack;Export&rbrack;有時無法匯出 .sbs/.sbsar 檔案
* &lbrack;Layers&rbrack; 新增基礎材質按鈕在材質為空時不會有任何作用
* &lbrack;Layers&rbrack;材質平鋪在複製材質時會改變
* &lbrack;實體尺寸&rbrack;如果實體尺寸面板在匯入影像前已停靠，自動測量功能無法運作
* &lbrack;腳本&rbrack;自動儲存插件壞掉了
* &lbrack;UI&rbrack;匯出對話框中空距錯誤
* &lbrack;UI&rbrack;調整滑桿動畫不再運作
* &lbrack;UI&rbrack;滑桿在需要時不會自動吸附成整數值
* &lbrack;UI&rbrack;有些下拉選單會被裁切

### **5.0.2 榛果**

*（發布日期：2025年4月22日）*

**修正：**

* &lbrack;Application&rbrack;首頁的返回按鈕壞了
* &lbrack;Application&rbrack;如果磁碟上有損壞的舊版本資料，取樣器有時無法啟動
* &lbrack;Application&rbrack;匯入的影像不會出現在視窗或圖層堆疊中
* &lbrack;Captis&rbrack;Captis IP 位址欄位即使重新啟動 Sampler 仍為空
* &lbrack;Captis&rbrack;即時攝影機預覽僅在應用程式語言設為英文時有效
* &lbrack;Export&rbrack; 匯出時崩潰 &amp; lbrack;Layers&rbrack; 有時在先前儲存的專案中無法上色
* &lbrack;Layers&rbrack;取樣器有時只更新一個通道時會更新所有材質
* &lbrack;Layers&rbrack;升級到 5.0.x 後，無法在圖層堆疊中使用材質混合
* &lbrack;Layers&rbrack;將專案更新為先前的 Image to Material（AI）版本，會使素材全黑
* &lbrack;Layers&rbrack;當嘗試匯入不支援的圖片時，Sampler 會建立一個破損的圖層
* &lbrack;Scripting&rbrack;Python API 的一部分無法在空專案中運作
* &lbrack;UI&rbrack;選單項目有時會溢出檔案選單

### **5.0.1 榛果**

*（發布日期：2025年3月20日）*

**新增內容**

* &lbrack;Application&rbrack;更新顯示卡驅動程式相容清單
* &lbrack;Captis&rbrack;當作業系統政策阻擋 HP Z Captis 使用時，會顯示彈出視窗
* &lbrack;快速動作&rbrack;說明為何工具提示中關閉快速動作
* &lbrack;UI&rbrack; 崩潰報告視窗 UI 樣式
* &lbrack;UI&rbrack;複製到剪貼簿時，請顯示一個祝酒詞表示已完成

**修正：**

* &lbrack;2D View&rbrack;曝光滑桿在球面投影關閉時不會有影響
* &lbrack;2D 視圖&rbrack;在貼圖外繪製會產生中斷筆觸
* &lbrack;2D 視圖&rbrack;曝光按鈕沒有提示。
* &lbrack;2D View&rbrack;在非方形影像側邊縮放時，滑鼠不會跟著滑鼠移動
* &lbrack;3D Capture &rbrack;3D Capture 在 Windows 11 24H2 上無法使用
* &lbrack;3D Capture&rbrack;如果在網格重建階段關閉 Sampler，會當機
* &lbrack;3D View&rbrack;計算時間有時顯示為 0ms
* &lbrack;3D 視圖&rbrack;當投影從正交切換為透視時，視窗會變為灰色
* &lbrack;Application&rbrack;在檢查 GPU 功能時啟動時當機
* &lbrack;Application&rbrack;安裝時當機
* &lbrack;Application&rbrack; 右鍵點擊元資料欄位後退出時當機
* &lbrack;Application&rbrack;從作業系統檔案總管開啟 SBSAR 時，環境燈缺失
* &lbrack;Application&rbrack;在 Sampler 執行時開啟 .sbsar 會改變貼圖平鋪設定
* &lbrack;Captis&rbrack;部分元資料可能無法在擷取步驟間傳輸
* &lbrack;Captis&rbrack;所建立資產的名稱並非中繼資料欄位中輸入的名稱
* &lbrack;內容&rbrack;篩選器更新範例專案提示，但已更新
* &lbrack;Filters&rbrack;Normal/高度調整濾波器沒有圖示
* &lbrack;Layers&rbrack; 無法更改圖片匯入圖層中的圖片
* &lbrack;Layers&rbrack; 使用升頻濾波器時會當機
* &lbrack;Layers&rbrack;將專案更新為舊影像時，材質會變成全黑
* &lbrack;Rendering&rbrack;在建立資產後立即調整圖層堆疊會破壞渲染
* &lbrack;腳本&rbrack;當專案中沒有資產時，自動儲存插件會崩潰
* &lbrack;Tools&rbrack;筆刷工具列中缺少筆刷大小值
* &lbrack;UI&rbrack;更改應用程式語言不會更新主畫面中的部分標籤
* &lbrack;UI&rbrack;在滑桿文字欄位按 Esc 或 Enter 不會失去焦點
* &lbrack;UI&rbrack;在屬性面板中，重置全部按鈕與資產名稱標籤重疊
* &lbrack;UI&rbrack;對接與拆卸面板時的問題
* &lbrack;UI&rbrack;在覆蓋面板中捲動也會在底層視窗中捲動
* &lbrack;UI&rbrack;在主畫面的「近期專案」區塊切換到清單視圖無法使用
* &lbrack;UI&rbrack;視窗顯示模式按鈕圖示總是顯示 2D/3D

### **5.0.0 榛果**

*（發行日期：2025年2月20日）*

**新增內容**

* &lbrack;Onboarding&rbrack;新首頁，提供快速學習內容、範例專案、快速行動及近期專案存取。
* &lbrack;Onboarding&rbrack;快速開始使用新的快速操作功能，可從首頁及專屬面板存取
* &lbrack;Onboarding&rbrack; &lbrack;內容&rbrack;快速動作是預先定義的工作流程，會填充最常用的圖層堆疊
* &lbrack;Onboarding&rbrack;可透過新的快速啟動選單、快速動作或自訂專案建立新專案
* &lbrack;Onboarding&rbrack;可透過專用按鈕直接從首頁建立空專案
* &lbrack;3D View&rbrack;新型先進光柵化器與路徑追蹤器帶來新的渲染能力（如塗層、光澤、半透明、次表面散射等特性）及Substance生態系統的視覺一致性
* &lbrack;3D 視圖&rbrack;檢視器設定現在可直接在 3D 視圖中存取
* &lbrack;3D View&rbrack;可將渲染快照儲存在剪貼簿或檔案中
* &lbrack;3D View&rbrack;顯示格子以視覺化場景原點
* &lbrack;3D View&rbrack;啟用地面平面捕捉陰影與反射
* &lbrack;3D View&rbrack;控制你的地面平面的反射性和不透明度
* &lbrack;3D Capture&rbrack;地面位置網格
* &lbrack;Application&rbrack;啟動應用程式時檢查硬體相容性
* &lbrack;Application&rbrack;當機報告視窗現在會在當機發生後立即開啟
* &lbrack;Content&rbrack; 開啟範例專案以便輕鬆開始
* &lbrack;Export&rbrack; 以 USD 檔案匯出 Adobe Standard 材質著色器
* &lbrack;生成式 AI&rbrack;在影像轉材質工作流程中使用影像作為輸入時，請檢查「Do not infer」標籤
* &lbrack;Project&rbrack;縮圖會儲存在專案檔案中，以便更快開啟專案
* &lbrack;Project&rbrack;在偏好設定中設定在專案檔案中儲存快取資料，並有不同模式（無快取、輕快取、完整快取）
* &lbrack;腳本&rbrack; &lbrack;破壞變更&rbrack;Qt 遷移至 Qt6.15 - 影響現有插件的相容性
* &lbrack;Scripting&rbrack;預設插件和腳本資料夾現在都在 Documents 資料夾裡
* &lbrack;腳本&rbrack;新增插件介面，讓主取樣器面板視覺一致
* &lbrack;腳本&rbrack; 存取 2 個插件範例以發現取樣器插件的功能
* &lbrack;Scripting&rbrack; 新 open_3d_catpure（） 函式
* &lbrack;Scripting&rbrack;插入圖層時，控制該圖層是插入目標位置的上方還是下方

**修正：**

* &lbrack;3D Capture&rbrack;若無法在 macOS 啟動物件擷取，則當機
* &lbrack;Application&rbrack;出口崩潰
* &lbrack;Application&rbrack;在新增資產到專案面板時，會在出口掛機
* &lbrack;Application&rbrack;除非你按下 Enter 鍵，否則無法重新命名專案資產
* &lbrack;Application&rbrack;取消與重做選單項目未被禁用，但本應關閉
* &lbrack;Assets&rbrack;無法從資產面板的「所有函式庫」區塊刪除資產
* &lbrack;內容&rbrack;地圖集建立器 - 若有不透明度地圖，請使用現有的不透明度地圖
* &lbrack;Content&rbrack; Color ID Blend - 修正底色中的顏色選擇問題
* &lbrack;Layers&rbrack;使用產生元時避免無謂計算
* &lbrack;Layers&rbrack;調整產生器可能會導致觸發過多計算
* &lbrack;效能&rbrack;改善 GPU 記憶體管理
* &lbrack;Performance&rbrack;重啟應用程式時不得使用 Render cache
* &lbrack;Resources&rbrack; 唯讀檔案在資產面板中無法顯示
* &lbrack;Scripting&rbrack; 允許在新增一層後重複使用一層
* &lbrack;腳本&rbrack;在同一腳本中多次更改層堆疊結構可能會失敗

**已移除：**

* &lbrack;Application&rbrack;移除對 .dng 和 .nef 影像檔的支援

## 版本 4

### **4.5.2 格呂耶爾**

*（發行日期：2024年11月7日）*

**修正：**

* &lbrack;內容&rbrack;裁切、刺繡與高度混合濾鏡

### **4.5.1 格呂耶爾**

*（發行日期：2024年7月30日）*

**修正：**

* &lbrack;Layers&rbrack; 灰階遮罩無法上色，會影響像是 Clone Stamp、Paint Warp、Content Aware Fill 等工具

### **4.5.0 GRUYERE**

*（發行日期：2024年7月18日）*

**新增內容**

* &lbrack;互通性&rbrack;將素材傳送至 UE5、Blender、Maya、3DsMax Unity
* &lbrack;Content&rbrack;新的材質產生器類別 - 漸層
* &lbrack;Content&rbrack; HDRI 工具 - 新的環境旋轉過濾器

**修正：**

* &lbrack;Exposed Parameters&rbrack;暴露 .sbsar 輸入值無法運作
* &lbrack;圖層&rbrack;底色在灰階影像下會變成紅色
* &lbrack;Rendering&rbrack; 色彩通道中使用的灰階影像色彩空間錯誤
* &lbrack;Scripting&rbrack;使用匯出預設有時無法匯出預期的頻道
* &lbrack;Content&rbrack; Dirt - 在 Image to Material 上套用 Dirt 濾鏡會產生黑色法線
* &lbrack;內容&rbrack;壓印 - 浮雕濾波器中圖案的縮放在 0 與 1 之間並非線性
* &lbrack;內容&rbrack;讓它變成瓷磚 - 改善法線和高度一致性

### **4.4.1 火鍋**

*（發行日期：2024年6月6日）*

**修正：**

* &lbrack;內容&rbrack;缺少髒污過濾器
* &lbrack;生成式 AI&rbrack;使用影像轉貼圖時有時會發生網路錯誤

### **4.4.0 火鍋**

*（發行日期：2024年5月23日）*

**補充：**

* &lbrack;Application&rbrack;3D 擷取快取現存於獨立子資料夾中
* &lbrack;生成式 AI&rbrack;影像轉紋理（測試版）
* &lbrack;生成式 AI&rbrack;文字轉模式（測試版）
* &lbrack;生成式 AI&rbrack;文字轉紋理（測試版）
* &lbrack;Scripting&rbrack;資產現在擁有「資源」屬性
* &lbrack;Scripting&rbrack;圖層現在擁有「output_usages」屬性

**修正：**

* &lbrack;Application&rbrack; 開啟損壞專案檔案時當機
* &lbrack;Application&rbrack;當專案包含損壞資產時會當機
* &lbrack;Application&rbrack; 在 Windows 拔除螢幕時當機
* &lbrack;Application&rbrack;Windows 工作列中應用程式圖示錯誤
* &lbrack;Application&rbrack;主設定檔損壞可能導致檔案被刪除
* &lbrack;Application&rbrack; 面板會出現在彈出視窗前方
* &lbrack;內容&rbrack;材質產生器的縮圖會模糊
* &lbrack;Export&rbrack;從匯入影像產生的不透明度通道在匯出 .sbs/.sbsar 時會中斷
* &lbrack;Filters&rbrack;升頻可能會根據輸入層數當機
* &lbrack;生成式 AI&rbrack;當服務收到意外結果時可能發生當機
* &lbrack;Scripting&rbrack; 從環境變數自動載入插件時會當機
* &lbrack;Scripting&rbrack;指派 API 輸出使用時可能當機

### **4.3.3 EMPANADA**

*（發行日期：2024年3月26日）*

**補充：**

* &lbrack;3D Capture&rbrack;後製過程中新增的先進自動紫外線參數
* &lbrack;Filters&rbrack; 穿孔濾波器：可反轉並改變自訂圖案大小的能力

**修正：**

* &lbrack;3D 擷取&rbrack;macOS 上的底色可能會錯誤
* &lbrack;3D 擷取&rbrack;處理新版本時會當機
* &lbrack;3D Capture&rbrack;後製處理步驟在 macOS 上可能會當機
* &lbrack;3D Capture&rbrack;網格轉換圖層可能導致錯誤渲染
* &lbrack;Application&rbrack; 在啟動取樣器時，當上一個實例仍在匯出時當機
* &lbrack;Application&rbrack; Sampler 第一次啟動時會短暫無反應
* &lbrack;Export&rbrack;各向異性角度映射不會匯出
* &lbrack;Filters&rbrack;將布織法加入圖層堆疊可能會導致當機
* &lbrack;Filters&rbrack;將 Emboss 加入圖層堆疊可能會導致當機
* &lbrack;Filters&rbrack;內容感知填充在使用 32 位元影像時會當機
* &lbrack;Filters&rbrack; Emboss：下方圖層的不透明度並未完全覆寫
* &lbrack;Filters&rbrack; Fill：混合模式在 Designer 和 Painter 中無法使用
* &lbrack;過濾器&rbrack;刺繡：自動選色壞掉了
* &lbrack;偏好設定&rbrack; 防止設定不支援的 3D 擷取快取路徑
* &lbrack;偏好設定&rbrack;正常格式偏好不適用
* &lbrack;腳本&rbrack;Asset.export_material的通道參數以大小寫區分

### **4.3.2 EMPANADA**

*（發行日期：2024年2月22日）*

**修正：**

* &lbrack;Application&rbrack; 在 Windows 的網路共享中儲存專案會損壞專案檔案

### **4.3.1 EMPANADA**

*（發行日期：2024年2月15日）*

**修正：**

* &lbrack;3D Capture&rbrack;當影像檔案無法存取時，當批次產生遮罩時會當機
* &lbrack;Export&rbrack;用 Crop 或相對於輸入政策層匯出材料，結果無效
* &lbrack;Layers&rbrack;渲染圖層堆疊時罕見崩潰
* &lbrack;Filters&rbrack; 刺繡 - 修正 MacOS 材質輸入時的問題
* &lbrack;Filters&rbrack; 風格化 - 支援材質產生器
* &lbrack;Filters&rbrack; 模式 - 修正參數命名
* &lbrack;Localization&rbrack; 「另存為...」 在硬體資訊視窗的說明選單裡，顯示為未本地化

### **4.3.0 EMPANADA**

*（發行日期：2024年1月25日）*

**新增內容**

* &lbrack;Assets&rbrack; 新資產類型：材質產生器
* &lbrack;資產&rbrack;入門資產中包含的新材料
* &lbrack;Assets&rbrack;屬性面板中新增的影像參數資產選擇器
* &lbrack;Assets&rbrack;將材質產生器從資產面板拖放到屬性面板的圖片選擇器
* &lbrack;Assets&rbrack;從作業系統檔案總管拖放材質產生器
* &lbrack;Assets&rbrack; 過濾器可透過影像輸入的使用者標籤建議擬合產生器
* &lbrack;Assets&rbrack;材質產生器可以透過使用者標籤定義應該推薦的濾鏡
* &lbrack;內容&rbrack;新視角裁切濾鏡
* &lbrack;內容&rbrack;新風格化過濾器
* &lbrack;內容&rbrack;填充過濾器上的混合模式
* &lbrack;內容&rbrack;更新刺繡濾鏡
* &lbrack;內容&rbrack; 更新的塗裝包裝濾鏡
* &lbrack;內容&rbrack;更新所有濾鏡以支援材質產生器
* &lbrack;Layers&rbrack;在將材質產生器加入圖層堆疊時，能夠選擇其輸出通道
* &lbrack;Layers&rbrack; 能輕鬆列出並套用貼圖產生器上的預設設定
* &lbrack;Layers&rbrack; 在圖片選擇器中顯示材質產生器預覽
* &lbrack;Layers&rbrack;紋理產生器參數可以被暴露並匯出
* &lbrack;Layers&rbrack; 在用材質匯入建立範本匯入單一圖片時，指派基底顏色的使用方式
* &lbrack;Layers&rbrack; 在屬性面板中嘗試拖放不相容檔案時的反饋
* &lbrack;Layers&rbrack; 從匯入影像的 alpha 通道產生不透明度通道
* &lbrack;Layers&rbrack;影像轉材質（AI）在更改類別時計算速度更快
* &lbrack;Layers&rbrack;使用建立範本後，選擇最相關的圖層
* &lbrack;Layers&rbrack;現在可以在進階參數群組中用滑桿調整位置小工具
* &lbrack;Export&rbrack;在隊列中顯示百分比，而非原始數字
* &lbrack;互通性&rbrack;不透明度通道現在在傳送給 Painter 時被識別為 alpha 通道
* &lbrack;Application&rbrack;新增顯示與儲存硬體資訊的對話框
* &lbrack;Application&rbrack;新增偏好，為每個專案更改預設高度比例
* &lbrack;Application&rbrack;改善舊資產的顯示方式
* &lbrack;Scripting&rbrack; 新 asset.documentResolution（） 及 asset.setDocumentResolution（） 函式
* &lbrack;Scripting&rbrack; 新 select_asset（） 函式
* &lbrack;腳本&rbrack; Python 材質產生器API
* &lbrack;Scripting&rbrack; get_project_assets（） 現在回傳 3D 物件
* &lbrack;UI&rbrack;資產縮圖大小可在資產面板中更改
* &lbrack;UI&rbrack;更新視窗顯示圖示

**修正：**

* &lbrack;2D 視圖&rbrack;滑鼠滾輪的縮放被阻擋在 244%
* &lbrack;Application&rbrack;初始化圖形 API 時當機
* &lbrack;Application&rbrack;如果專案名稱包含 # 字元，則當機
* &lbrack;Application&rbrack;開啟舊專案時可能當機
* &lbrack;Application&rbrack;重新開啟目前專案可能會導致當機
* &lbrack;Application&rbrack;有些專案變更未被登錄，若未儲存，關閉專案時會無預警遺失
* &lbrack;Export&rbrack; .sbs/.sbsar 在使用多個同名檔案時匯出問題
* &lbrack;Export&rbrack;匯出灰階影像的色彩空間錯誤 .sbs/.sbsar 檔案
* &lbrack;Filters&rbrack;不透明度混合行為問題
* &lbrack;Layers&rbrack;.svg檔案有時不會以正確解析度呈現
* &lbrack;Performance&rbrack;有些專案存檔在磁碟上是不必要的
* &lbrack;Project&rbrack;匯入舊專案不會載入相關的預設
* &lbrack;Scripting&rbrack; 無法取得第一層插入的參數
* &lbrack;UI&rbrack;當滑鼠滑鼠移到資產時，預覽彈出視窗可能會出現在錯誤的位置或畫面
* &lbrack;UI&rbrack;未接駁的面板在歡迎畫面上方可見且可用

### **4.2.2 多拉燒**

*（發行日期：2023年12月5日）*

**補充：**

* &lbrack;3D 擷取 &rbrack;現在 Windows 上的 3D 擷取速度快了 5% 到 10%
* &lbrack;3D 擷取&rbrack;在減量前改善網格清理
* &lbrack;Engine&rbrack;更新 Substance Engine 至 9.0.3 版本
* &lbrack;Layers&rbrack;內容感知填充：上游更新、各種使用案例修正及 Linux 支援

**修正：**

* &lbrack;3D Capture&rbrack;對齊後點擊「返回」再點擊「Next」不會更新點雲
* &lbrack;3D 擷取&rbrack;加入專案後顯示有孔的網格
* &lbrack;Application&rbrack;在3D擷取後退出全螢幕模式時會當機
* &lbrack;Application&rbrack;用製作的影像檔案當機
* &lbrack;Application&rbrack;如果在「所有函式庫」中退出取樣器時，重啟時資產面板會變空
* &lbrack;Application&rbrack; 匯出資料時的記憶體洩漏
* &lbrack;Application&rbrack;開啟包含先前取樣器版本的專案存檔可能會導致當機
* &lbrack;Application&rbrack;當無法轉換 3D 網格時，潛在的當機
* &lbrack;Application&rbrack;在 Sampler 執行時開啟 .sbsar 時發生靜默當機
* &lbrack;Export&rbrack;匯出 .sbs/.sbsar 檔案並自訂使用時會當機
* &lbrack;Export&rbrack;匯出的法線貼圖無論使用者設定如何，都永遠是 DirectX
* &lbrack;Export&rbrack;在 macOS 上將 3D 物件匯出成 FBX 檔案無法運作
* &lbrack;Export&rbrack;將帶有刺繡濾波器的圖層堆疊匯出為 .sbs/.sbsar 檔案時的不一致
* &lbrack;Export&rbrack;有時匯出 .sbs/.sbsar 檔案無法運作
* &lbrack;Export&rbrack;有時匯出 .sbs/.sbsar 檔案時，圖片的位元深度不對
* &lbrack;Layers&rbrack;將 Splatter 圖層變成隱形則會呈現其第一個子節點
* &lbrack;Layers&rbrack;在亮度/對比圖層載入遮罩時會崩潰
* &lbrack;Layers&rbrack;刪除圖層後會顯示誤導性的錯誤訊息
* &lbrack;Layers&rbrack;降級資產時可能發生崩潰
* &lbrack;Layers&rbrack;有些輸出除非在通道設定面板強制使用，否則不會連接到輸入端
* &lbrack;物理尺寸&rbrack;參考層下拉選單可能會被誤重置
* &lbrack;UI&rbrack; 匯入模板資訊圖示需要更新
* &lbrack;UI&rbrack;視窗快捷鍵提示，每次視窗配置改變時都會出現

### **4.2.1 多拉燒**

*（發行日期：2023年9月21日）*

**新增：**

* &lbrack;Content&rbrack;影像到材質 - 改善法線貼圖中的微細節生成
* &lbrack;內容&rbrack;影像到素材 - 新的愉悅強度參數
* &lbrack;圖層&rbrack;圖片可在影像匯入圖層中加入
* &lbrack;Layers&rbrack;圖片可以在 Image 匯入圖層中移除
* &lbrack;Layers&rbrack; 無效圖層現在可以刪除
* &lbrack;2D View&rbrack;Shift+C 快捷鍵可切換回頻道
* &lbrack;3D 擷取&rbrack;當使用者匯入少於 20 張圖片時，會顯示警告吐司
* &lbrack;Application&rbrack;新增設定預設材質貼圖平鋪值
* &lbrack;Onboarding&rbrack;更新了影像轉材質（AI）及放大的教學介面
* &lbrack;Scripting&rbrack; 3D 擷取 API：當 Capture3dState 設定為對齊時，DatasetInfo 擁有更多資料
* &lbrack;Scripting&rbrack; create_asset（） 的新select_asset論元。 新增功能：wait_for_computation（） 與 clear_render_cache（）

**已修正：**

* &lbrack;Layers&rbrack;當作物區域非常小時崩潰
* &lbrack;Layers&rbrack;新增或調整裁切濾鏡時會崩潰
* &lbrack;Layers&rbrack;將裁切區域設成方形會導致材料輸出解析度錯誤
* &lbrack;Layers&rbrack;當多個層被停用時，輸出有時會消失
* &lbrack;Layers&rbrack;渲染快取可能無法正確失效於影像轉材質（AI）及升頻濾波器
* &lbrack;Layers&rbrack;在警告彈出視窗中選擇「請勿再次顯示此訊息」時，無法新增升頻過濾器
* &lbrack;Layers&rbrack;修改後無法在刺繡濾鏡中還原圖片
* &lbrack;Export&rbrack;當更改法線格式時，匯出的法線貼圖解析度會改變
* &lbrack;Export&rbrack;在匯出環境時移除「\_environment」檔名後綴
* &lbrack;Export&rbrack;當圖層堆疊中有 Warp Transform 圖層時，無法匯出 .sbsar 檔案
* &lbrack;2D View&rbrack;「Fit to screen」在解析度改變時無法運作
* &lbrack;Application&rbrack;在關閉應用程式視窗後，應用程式程序仍可繼續執行
* &lbrack;Application&rbrack;出口崩潰
* &lbrack;Application&rbrack; 切換 GPU 加速神經網路時，渲染快取失效
* &lbrack;Scripting&rbrack; 將外掛命名為現有面板名稱會引起意想不到的行為
* &lbrack;UI&rbrack;點擊有提示的項目會讓提示消失，直到重新啟動
* &lbrack;UI&rbrack;高度比例值在切換資產時可能會改變
* &lbrack;UI&rbrack;組合框中的邊距錯誤

### **4.2 多拉燒**

*（發行日期：2023年9月5日）*

**補充：**

* &lbrack;內容與內容;大幅改進了影像與材質（AI）及 Delighter 濾鏡
* &lbrack;內容&rbrack;新高頻濾波器
* &lbrack;內容&rbrack;裁剪濾波器現在具有動態輸出解析度。
* &lbrack;材料建立範本&rbrack;新增文件大小設定。
* &lbrack;材質創建範本&rbrack;新增「新增裁切」切換按鈕。
* &lbrack;素材建立範本&rbrack;新的「高頻素材」切換功能
* &lbrack;材質建立範本&rbrack;顯示匯入影像大小
* &lbrack;材質建立範本&rbrack;當部分匯入圖片無法使用時，給予回饋
* &lbrack;材質建立範本&rbrack;當影像大小不一致時會警告
* &lbrack;材質製作範本&rbrack;新增警告與工具提示
* &lbrack;Layers&rbrack; 顯示圖層堆疊中各圖層的解析度
* &lbrack;Layers&rbrack;圖層計算解析度現在可以設定為文件大小或輸入大小
* &lbrack;Layers&rbrack; 顯示圖層堆疊中的圖層解析度
* &lbrack;Layers&rbrack;在適用時，將圖層解析策略切換為文件或圖層輸入
* &lbrack;Layers&rbrack;當手動新增升頻濾波器時，提醒使用者並提供一些文件
* &lbrack;Layers&rbrack;在線性升階時提醒使用者，並提出改用升頻濾波器
* &lbrack;Layers&rbrack;計算影像到材質（AI）圖層現在可以更快取消，以改善調整圖層堆疊時的渲染時間
* &lbrack;Layers&rbrack;計算升頻圖層現在可以更快取消，以提升調整圖層堆疊時的渲染時間
* &lbrack;Export&rbrack; 允許覆蓋匯出材質的解析度
* &lbrack;Export&rbrack;出口通道列表現在已排序
* &lbrack;Export&rbrack;在出口通道列表中顯示通道解析度
* &lbrack;Application&rbrack;啟用或停用 GPU 加速神經網路的新偏好
* &lbrack;UI&rbrack;改進解析度下拉選單
* &lbrack;UI&rbrack;網格轉換、網格後製處理與織布濾鏡的新圖示
* &lbrack;UI&rbrack; 將「分享」面板改名為「匯出」
* &lbrack;Scripting&rbrack; 為匯出 API 新增層輸出解析度支援
* &lbrack;Scripting&rbrack;新增裁切、放大及文件大小於影像匯入 API 中
* &lbrack;入門&rbrack;新教學
* &lbrack;Onboarding&rbrack;更新歡迎及最新畫面內容
* &lbrack;Engine&rbrack;更新物質引擎至版本 9.0.1

**修正：**

* &lbrack;3D 擷取&rbrack;改善對齊設定參數中的精度選項命名
* &lbrack;Application&rbrack;匯入 16 維度非倍數的影像可能會導致當機
* &lbrack;Application&rbrack;在專案面板複製資產時會當機
* &lbrack;Application&rbrack;在專案面板切換資產時當機
* &lbrack;內容&rbrack;為雪濾網繪製自訂遮罩無法正常運作
* &lbrack;Exposed Parameters&rbrack;在更換材料時，暴露的參數變更可能會遺失
* &lbrack;互通性&rbrack;從匯出面板傳送材料可能導致當機
* &lbrack;Layers&rbrack;內容感知填充在從單一影像輸入切換到材質輸入時停止計算
* &lbrack;Layers&rbrack;在複製包含材質的環境光後當機
* &lbrack;Layers&rbrack;如果圖片檔案被重新命名，影像匯入層會在屬性面板顯示錯誤的圖片名稱
* &lbrack;Layers&rbrack;有時旋轉器會顯示在非啟用圖層上
* &lbrack;Layers&rbrack;有時更改影像匯入圖層的輸出使用方式無法運作
* &lbrack;Layers&rbrack; 建立範本視窗中的錯字
* &lbrack;UI&rbrack; 3D 視口接入工具提示有焦點問題
* &lbrack;UI&rbrack;若檔名過長，影像名稱可能會溢出
* &lbrack;UI&rbrack;使用橡皮擦時筆刷工具列的小型配置問題
* &lbrack;UI&rbrack;在某些語言中，字串會在檢視器設定面板中被截斷
* &lbrack;UI&rbrack;當視窗工具提示彈出視窗顯示時，按下「空白」會建立一個新專案

### **4.1.2 卡諾利**

*（發行日期：2023年6月20日）*

**修正：**

* &lbrack;Layers&rbrack;調整Substance材質與濾波器時發生記憶體洩漏，導致當機

### **4.1.1 卡諾利**

*（發行日期：2023年6月6日）*

**新增內容**

* &lbrack;Engine&rbrack;更新物質引擎至版本 9.0
* &lbrack;互通性&rbrack;將 3D 物件傳送給 Stager 與 Painter

**修正：**

* &lbrack;3D 擷取&rbrack;應用程式在 3D 擷取渲染器失敗時當機
* &lbrack;3D 擷取&rbrack;影像無法載入時當機
* &lbrack;3D Capture&rbrack;進入網格重建步驟時崩潰
* &lbrack;3D Capture&rbrack;調整包圍框大小時會崩潰
* &lbrack;3D Capture&rbrack;依照慣例匯入遮罩時，遮罩無法正確指派
* &lbrack;3D Capture&rbrack;調整包圍框時的渲染故障
* &lbrack;3D 擷取&rbrack;在 3D 擷取後製過程中，切換版本與切換渲染選項會很慢
* &lbrack;3D Capture &rbrack;在 3D Capture 後製步驟中切換版本有時會出問題
* &lbrack;Application&rbrack;啟動時崩潰
* &lbrack;Application&rbrack;複製重命名素材時的崩潰
* &lbrack;Application&rbrack; 在未包含依賴資料夾時開啟舊有 .alch 專案時會當機
* &lbrack;Application&rbrack;插拔螢幕、電腦進入睡眠或遠端存取時當機
* &lbrack;Application&rbrack;與非持久性資產管理相關的當機與記憶體洩漏
* &lbrack;Export&rbrack;選擇 3D 物件檔案類型的材質格式，嵌入或參考貼圖時應該關閉
* &lbrack;Export&rbrack;如果 3D 物件匯出過程中出錯會當機
* &lbrack;Export&rbrack;匯出 .sbs/.sbsar 檔案時會當機
* &lbrack;Export&rbrack;匯入自訂預設時，標籤相同但檔名不相同，會當機
* &lbrack;Export&rbrack;將環境燈匯出成 .sbs/.sbsar 檔案有時無法運作
* &lbrack;Export&rbrack;Gltf/Glb 匯出時會編碼 base64 中的貼圖
* &lbrack;Export&rbrack;重新聚焦時名稱文字欄位無法運作
* &lbrack;Export&rbrack; Preserve 平鋪在將 Image to Material（AI 驅動）圖層匯出到 .sbs/.sbsar 檔案時無法運作
* &lbrack;Export&rbrack;在匯出 gltf 並替換檔案時，要替換的檔案清單並不正確
* &lbrack;Exposed Parameters&rbrack;隨機種子在匯出的 .sbs/.sbsar 檔案中無法運作
* &lbrack;Layers&rbrack;內容感知填充在第二次新增時有時會當機
* &lbrack;Layers&rbrack;計算層堆疊時的崩潰
* &lbrack;Layers&rbrack;影像轉材質（AI）磁碟快取無法運作
* &lbrack;Layers&rbrack;調整圖層時可能崩潰
* &lbrack;效能&rbrack;記憶體洩漏
* &lbrack;Project&rbrack;儲存專案時的崩潰
* &lbrack;Project&rbrack; 連續匯入同一個專案兩次會重複資產
* &lbrack;UI&rbrack;圓角按鈕僅有圖示的按鈕無法正確呈現

### 4.1.0 卡諾利

*（發行日期：2023年3月28日）*

**補充：**

* &lbrack;內容&rbrack;新刺繡過濾器
* &lbrack;內容&rbrack;新漆面變形濾鏡
* &lbrack;UI&rbrack; 在檔案選單中新增匯出選項
* &lbrack;3D 擷取&rbrack;返回按鈕現在可在對齊步驟中使用
* &lbrack;3D 擷取&rbrack;影像處理 JPEG EXIF 方向
* &lbrack;3D 擷取&rbrack;腳本 - 新dataset_info.camera 屬性
* &lbrack;3D 擷取&rbrack;新增 Linux 支援（見文件）
* &lbrack;3D 擷取&rbrack;驗證匯入影像的讀取權限
* &lbrack;入門&rbrack; 學習 - 2 個新教學（刺繡與油漆變形）
* &lbrack;Onboarding&rbrack;更新內容

**修正：**

* &lbrack;3D Capture&rbrack;切換版本時保持攝影機位置
* &lbrack;3D Capture&rbrack;將物件的所有群組合併為一個
* &lbrack;3D Capture&rbrack;將生成的網格重新命名為原始
* &lbrack;Application&rbrack; 嘗試產生不存在影像縮圖時會當機
* &lbrack;Assets&rbrack;垃圾桶圖示在資產面板中沒有任何作用
* &lbrack;內容&rbrack;更新帶有素材槽的過濾器無法如預期運作
* &lbrack;Export&rbrack;匯出資產時可能會當機，並使用特定篩選條件
* &lbrack;Export&rbrack;SBS/SBSAR 匯出 - 影像匯入圖層優先於影像參數
* &lbrack;Export&rbrack;UE4 匯出預設無法支援 PNG
* &lbrack;Layers&rbrack;當同時從作業系統檔案總管丟棄材質與過濾器時會當機
* &lbrack;Layers&rbrack;拖曳任何 SBSAR 檔案與任何影像檔時會當機
* &lbrack;Layers&rbrack;刺繡不透明度通道可以完全是白色的
* &lbrack;本地化&rbrack;中文可在Linux上預設顯示
* &lbrack;Performance&rbrack;修正了從資產移除圖層時的記憶體問題
* &lbrack;Project&rbrack;儲存時可能當機
* &lbrack;UI&rbrack; 在 Version 選單按鈕上新增缺少的空格
* &lbrack;UI&rbrack; 取消按鈕未正確顯示
* &lbrack;UI&rbrack; 關閉 3D 捕捉後製參數的滑桿動畫
* &lbrack;UI&rbrack;材質建立範本視窗在點擊外部時不會自動關閉
* &lbrack;UI&rbrack;當點擊外部時，過濾器快速存取器會自動關閉

**已知問題：**

* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作
* &lbrack;內容&rbrack;形狀燈光小工具在球面投影模式下無法運作
* &lbrack;互通性&rbrack;送往Stager的排水物資將失去排水控制

### 4.0.2 香蕉

*（發布日期：2023年3月9日）*

**補充：**

* &lbrack;3D 擷取&rbrack;磁碟使用量顯示使用量
* &lbrack;3D 擷取&rbrack;匯入照片是非同步且更快的
* &lbrack;腳本&rbrack;用於撰寫 3D 擷取功能腳本的新類別與函式
* &lbrack;Scripting&rbrack;新的 ExportController 類別，用於在匯出完成、失敗或取消時執行動作
* &lbrack;Scripting&rbrack; 傳遞參數 Python 腳本執行時 --run-script
* &lbrack;UI&rbrack;拖曳資產到圖層面板時的 UI 反饋
* &lbrack;Content&rbrack;色溫濾鏡現在正在材料上工作
* &lbrack;Content&rbrack;Normal to Height 濾波器新增了保留平鋪的選項

**修正：**

* &lbrack;3D Capture&rbrack;資料集對齊步驟中修正影像尺寸
* &lbrack;3D 擷取&rbrack;UV展開後移除重複頂點
* &lbrack;3D 擷取;MacOS - 若有 3D 擷取功能，偵測效果更好
* &lbrack;3D 擷取&rbrack;匯入影像時關閉 3D 擷取視窗時當機
* &lbrack;3D Capture&rbrack;產生新版本時會崩潰
* &lbrack;3D 擷取&rbrack;嘗試在檢視器中載入 3D 物件時會當機
* &lbrack;3D Capture&rbrack;使用非 UTF8 字元的路徑時會崩潰
* &lbrack;3D Capture&rbrack;命中與提示 打字錯誤
* &lbrack;3D Capture&rbrack;網格不再縮放以符合單位立方體
* &lbrack;3D 擷取&rbrack;在渲染時關閉 3D 擷取時防止當機
* &lbrack;3D Capture&rbrack;移除遮罩會讓影像消失
* &lbrack;Application&rbrack;同時匯入兩個資產時會當機
* &lbrack;Application&rbrack;若資產從未備份，開啟專案時備份先前版本的資產
* &lbrack;Application&rbrack; 正確快取烘焙的地圖，即使並非所有地圖都已烘焙
* &lbrack;Application&rbrack;當顯示 3D 物件時，全螢幕會當機。
* &lbrack;Application&rbrack;最後一個資料在儲存專案時會被複製
* &lbrack;Application&rbrack; 防止在烘焙步驟取消網格後處理計算時當機
* &lbrack;Application&rbrack;重新開啟目前專案不會丟棄變更
* &lbrack;Application&rbrack; 停止為 3D 物件產生縮圖
* &lbrack;2D View&rbrack;使用筆刷工具時會崩潰
* &lbrack;內容感知填充 - 計算可能卡住
* &lbrack;內容&rbrack;Atlas Creator 過濾器正在降頻不透明度頻道
* &lbrack;Export&rbrack; 修正：清除失敗的匯出佇列
* &lbrack;Export&rbrack;OBJ 輸出會產生比預期小 100 倍的物件
* &lbrack;Layers&rbrack;以灰階通道匯入的彩色影像現在被視為灰階
* &lbrack;Export&rbrack;FBX 檔案無法匯入第三方應用程式
* &lbrack;Export&rbrack;著色器輸出名稱在 USD 檔案中不正確
* &lbrack;Layers&rbrack;在作業系統檔案總管更改影像名稱時，影像名稱不會更新
* &lbrack;Scripting&rbrack; 在重新載入無效腳本時顯示錯誤訊息
* &lbrack;UI&rbrack;當無法使用時，基礎材質按鈕會被禁用
* &lbrack;UI&rbrack; 在材質建立範本視窗中存取檔案對話框時會當機
* &lbrack;UI&rbrack; 快速存取器即使層面板關閉也能存取
* &lbrack;UI&rbrack;傳送至圖示錯位
* &lbrack;UI&rbrack;點擊 Blend 圖示時，圖示會改變

**已知問題：**

* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作
* &lbrack;內容&rbrack;形狀燈光小工具在球面投影模式下無法運作
* &lbrack;互通性&rbrack;送往Stager的排水物資將失去排水控制

### 4.0.1 香蕉

*（發行日期：2023年2月7日）*

**修正：**

* &lbrack;3D Capture&rbrack;使用遮罩時，貼圖投影可能會被破壞
* &lbrack;3D 擷取&rbrack;你的物件上可能會出現 artefacts
* &lbrack;3D Capture&rbrack;匯出的網格可能非常小

**已知問題：**

* &lbrack;3D Capture&rbrack;FBX 與 OBJ 會將結果匯出縮小解析度
* &lbrack;3D Capture&rbrack;即使你的硬體不相容，MacOS 上也能使用 3D Capture。 請查看文件說明。
* &lbrack;3D Capture&rbrack;網格重建完成時會當機。
* &lbrack;Layers&rbrack;內容感知填充（Content-Aware Fill）如果在下方調整圖層，可能會卡住
* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作
* &lbrack;內容&rbrack;形狀燈光小工具在球面投影模式下無法運作
* &lbrack;互通性&rbrack;送往Stager的排水物資將失去排水控制

### 4.0.0 香蕉

*（發行日期：2023年1月31日）*

**補充：**

* &lbrack;3D 擷取&rbrack;從影像建立 3D 物件
* &lbrack;3D 擷取&rbrack;專用 3D 擷取精靈
* &lbrack;3D Capture&rbrack;在你的資料集中匯入或產生黑白遮罩
* &lbrack;3D 擷取&rbrack;對齊結果 - 以點雲形式查看所有匹配特徵
* &lbrack;3D Capture&rbrack;對齊結果 - 查看並與每張對齊照片相關的相機互動
* &lbrack;3D Capture&rbrack;用邊界框小工具定義重建區域
* &lbrack;3D Capture&rbrack;在所有軸上進行縮放、平移與旋轉，包圍框小工具
* &lbrack;3D Capture&rbrack;定義重建網格的幾何精度
* &lbrack;3D Capture&rbrack;透過建立新版本來優化你的網格和材質
* &lbrack;3D Capture&rbrack;每個版本會自動減至目標面的數字設定
* &lbrack;3D Capture&rbrack;後製步驟會自動展開、重新投影貼圖，然後烘焙高多邊形網格的法線高度與 AO 資訊
* &lbrack;3D 擷取&rbrack;將原始結果或版本加入取樣器專案
* &lbrack;3D Capture&rbrack;新增網格後製圖層，能自動拆解、展開、重新投影底層網格圖層的貼圖，並烘焙細節
* &lbrack;3D Capture&rbrack;新增網格轉換圖層，用於縮放、旋轉或平移底層網格圖層
* &lbrack;出口&rbrack;新出口視窗
* &lbrack;Export&rbrack;根據資產類型（材質、環境光、網格）提供專用設定與介面
* &lbrack;Export&rbrack;將網格匯出為 USD、USDA、USDZ、glTF、glb、obj、fbx、stl
* &lbrack;Export&rbrack;在導出物質檔案時定義材料類型（SBSAR、SBS）
* &lbrack;UI&rbrack; 將快取設定移到偏好設定彈出視窗的新分頁
* &lbrack;Application&rbrack;2D 與 3D 視窗現在可以調整大小、交換並垂直堆疊
* &lbrack;Application&rbrack;新增SAMPLER_RESOURCES_PATH環境變數以新增額外起始資產
* &lbrack;腳本&rbrack;新增SAMPLER_PLUGIN_PATH與SAMPLER_SCRIPT_PATH環境變數以在啟動時匯入外掛與腳本
* &lbrack;腳本&rbrack;新增材質、環境光源及 3D 物件的匯出功能
* &lbrack;Scripting&rbrack;新增識別碼、預設值、最小值與最大值、標籤及枚舉值於參數
* &lbrack;Scripting&rbrack; 新增import_textures功能，可在匯入圖片時輸入自訂使用方式

**修正：**

* &lbrack;Application&rbrack;開啟近期專案並在確認對話框中儲存時當機
* &lbrack;Application&rbrack;檔案對話框阻止開啟 .ssa 檔案
* &lbrack;Application&rbrack;檔案對話框可以出現在 macOS 的背景視窗上
* &lbrack;Application&rbrack;開啟 3.2 專案時可能崩潰
* &lbrack;Application&rbrack;選擇檔案會在顯示警告前關閉檔案對話框
* &lbrack;Exposed Parameters&rbrack; 匯出參數化環境燈無法運作
* &lbrack;Layers&rbrack;圖層堆疊中的「點此瀏覽」連結已無法使用。
* &lbrack;Layers&rbrack;在同一圖層內繪製多張圖片有時無法成功
* &lbrack;Layers&rbrack;在圖層屬性中設定圖片不會更新圖片選擇器的縮圖
* &lbrack;Layers&rbrack; 將取樣器資產作為圖層調整無法運作
* &lbrack;Project&rbrack;開啟專案時更新不需要的資產
* &lbrack;Scripting&rbrack;瀏覽至插件資料夾有時在 Windows 上會失敗
* &lbrack;Scripting&rbrack;在 Python 腳本中使用 &#39;open_project（）&#39; 時會當機
* &lbrack;Scripting&rbrack;API 中缺少 JPEG 匯出功能
* &lbrack;腳本&rbrack;日誌面板並非唯讀
* &lbrack;腳本&rbrack;image_picker參數值不運作
* &lbrack;UI&rbrack;專案面板中缺少環境光源的資產圖示
* &lbrack;UI&rbrack; 偏好設定彈出視窗中的「送至設計器格式」下拉選單可以是空的
* &lbrack;UI&rbrack;有些按鈕的樣式不正確
* &lbrack;UI&rbrack;標籤與按鈕群組小工具中的按鈕重疊
* &lbrack;UI&rbrack;在設定實體尺寸選單中，「工具」的提示位置錯誤
* &lbrack;UI&rbrack;切換語言時，檔案選單會錯位

**已知問題：**

* &lbrack;3D Capture&rbrack;使用遮罩時，貼圖投影可能會被破壞
* &lbrack;3D Capture&rbrack;如果你在網格轉換中的縮放太小，物件上可能會出現小瑕疵
* &lbrack;3D Capture&rbrack;匯出的網格可能非常小。 重置網格轉換的縮放並重新匯出
* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作
* &lbrack;內容&rbrack;形狀燈光小工具在球面投影模式下無法運作
* &lbrack;互通性&rbrack;送往Stager的排水物資將失去排水控制

## 版本 3

### 3.4.1 阿蘭奇尼

*（發行日期：2022年10月6日）*

**補充：**

* &lbrack;入門&rbrack;新歡迎與最新資訊畫面
* &lbrack;Onboarding&rbrack;更新主畫面介面
* &lbrack;Onboarding&rbrack;主畫面新增學習內容
* &lbrack;Scripting&rbrack; 當方法未被識別時，請在日誌面板登錄錯誤
* &lbrack;Scripting&rbrack;新的 ssa.helpers 模組，可列印到日誌面板
* &lbrack;Application&rbrack;Substance 3D Designer 新增的並排按鈕小工具支援

**修正：**

* &lbrack;Export&rbrack;匯出引用遺失圖片的 .sbsar 檔案時會當機
* &lbrack;Export&rbrack;匯出參考損毀影像檔案的資產時會當機
* &lbrack;Export&rbrack;將帶有刺繡圖層的 .sbsar 檔案匯出會產生灰色材質
* &lbrack;Export&rbrack;將材質匯出為 .sbs/sbsar 檔案可以產生完全透明的材質
* &lbrack;Export&rbrack;Normal Format 參數在 .sbs/.sbsar 檔案中未正確暴露
* &lbrack;Export&rbrack;Sbs/sbsar 匯出參考 .svg 檔案的圖層堆疊時會出問題
* &lbrack;Export&rbrack; 變換圖層未正確匯出 / 更新 Enscape - Revit 匯出預設
* &lbrack;Exposed Parameters&rbrack;刪除包含暴露參數的圖層時會當機
* &lbrack;Exposed Parameters&rbrack;更新層堆疊中過時的層可能會導致暴露參數清單損壞
* &lbrack;Exposed Parameters&rbrack;不該匯出的參數反正都會匯出
* &lbrack;Exposed Parameters&rbrack; 刪除圖層時移除混合濾波器並不會解除其參數
* &lbrack;Exposed Parameters&rbrack; 文字參數會破壞 .sbs/.sbsar 匯出
* &lbrack;Layers&rbrack; 將圖層堆疊放入另一層堆疊時會崩潰
* &lbrack;Layers&rbrack;未能載入濾波器時當機
* &lbrack;Layers&rbrack;重置影像欄位時無法重新載入前一張影像
* &lbrack;Layers&rbrack; 無法還原/重做工具變更
* &lbrack;Layers&rbrack; Clone Stamp 圖層在點擊「重設所有設定」後卡住了
* &lbrack;Layers&rbrack;使用任何重置按鈕都會阻止在影像欄位繪製
* &lbrack;Layers&rbrack;重置按鈕不會清除圖片欄位中的繪圖遮罩
* &lbrack;Layers&rbrack;如果使用者已經繪製了東西，影像欄位中的重置按鈕就不會有反應
* &lbrack;Layers&rbrack;使用筆刷工具時，渲染快取無法運作
* &lbrack;Layers&rbrack;刪除的圖層仍可在屬性面板中顯示
* &lbrack;Layers&rbrack; 圖層計算在切換專案資產時可能會停滯
* &lbrack;Project&rbrack;有時 Sampler 無法從磁碟開啟專案
* &lbrack;2D 視圖&rbrack;2D 視圖預設永遠回到 Material Output

**已知問題：**

* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作
* &lbrack;內容&rbrack;形狀燈光小工具在球面投影模式下無法運作
* &lbrack;互通性&rbrack;送往Stager的排水物資將失去排水控制

### 3.4.0 阿蘭奇尼

*（發行日期：2022年9月6日）*

**補充：**

* &lbrack;Exposed Parameters&rbrack;新公開參數面板
* &lbrack;Exposed Parameters&rbrack;參數上的新按鈕懸停在屬性面板中，可以顯示和取消曝光參數
* &lbrack;Exposed Parameters&rbrack;新增了右鍵右鍵選單，可以從屬性面板中顯示與解除參數
* &lbrack;Exposed Parameters&rbrack;公開參數列於Exposed Parameters面板
* &lbrack;曝光參數&rbrack;色彩點與彩色圓盤會在多個位置加入，以便輕鬆辨識暴露參數
* &lbrack;Exposed Parameters&rbrack;參數標籤可在 Exposed Parameters 面板中編輯
* &lbrack;Exposed Parameters&rbrack; 顯示不可匯出參數的警告
* &lbrack;Exposed Parameters&rbrack; 如果將帶有裸露混合參數的圖層移動到隱藏處，會顯示警告
* &lbrack;Exposed Parameters&rbrack;暴露參數會以 SBS 和 SBSAR 格式匯出
* &lbrack;Metadata&rbrack; 支援自訂元資料範本
* &lbrack;Metadata&rbrack;新 CLO 物理屬性 metadata 範本
* &lbrack;Metadata&rbrack; 在滑鼠滑鼠上新增或移除自訂元資料
* &lbrack;Python API&rbrack; New Python API
* &lbrack;Python API&rbrack; API for Asset authoring
* &lbrack;Python API&rbrack; API for Layers management
* &lbrack;Python API&rbrack; API for Parameters management
* &lbrack;Python API&rbrack; API for Project Management
* &lbrack;Python API&rbrack;外掛可以啟用或停用
* &lbrack;Python API&rbrack;Python API 文件可於說明選單中取得
* &lbrack;Scripting&rbrack;偏好設定彈出視窗中的新插件與腳本區塊
* &lbrack;腳本&rbrack;建立並匯入外掛，自訂取樣器介面與你自己的面板
* &lbrack;腳本&rbrack;插件成為取樣器介面的一部分，可以像標準取樣器面板一樣停靠和移動
* &lbrack;Scripting&rbrack;取樣器右側工具列專用的插件按鈕列
* &lbrack;腳本&rbrack; 建立並匯入腳本以執行指定任務清單
* &lbrack;Scripting&rbrack; 透過 Scripts 選單啟動 Python 腳本
* &lbrack;腳本&rbrack;插件與腳本可從偏好設定視窗刪除、重新排序及重新載入
* &lbrack;Scripting&rbrack; 新增 --run-script 命令列參數
* &lbrack;Logs&rbrack;新Logs面板
* &lbrack;Logs&rbrack; 從偏好設定視窗啟用日誌面板
* &lbrack;Logs&rbrack;新增動作列以清除、複製貼上、匯出日誌
* &lbrack;Properties&rbrack;參數上的新按鈕懸停以重置參數值
* &lbrack;Properties&rbrack;新增右鍵右鍵選單，用於參數重設
* &lbrack;內容&rbrack;影像轉材質（AI 驅動）現在可在 MacOS 上運作
* &lbrack;引擎&rbrack;更新Substance引擎至v8.6.0

**修正：**

* &lbrack;Application&rbrack;應用程式在縮圖產生過程中，可能會在退出時當機
* &lbrack;Application&rbrack;應用程式在退出時使用「另存為」可能會當機
* &lbrack;Application&rbrack;應用程式在 MacOS 關機時可能會當機
* &lbrack;Application&rbrack; 開啟顏色對話框儲存時，不會儲存變更
* &lbrack;Export&rbrack;匯出時的命名規則不正確
* &lbrack;Layers&rbrack;將材料丟到過濾器上可能會崩潰
* &lbrack;Layers&rbrack;更新過時的層堆疊可能會更新無關的層堆疊
* &lbrack;Metadata&rbrack;空欄位會被匯出
* &lbrack;Metadata&rbrack;當只有一個元資料項目時，介面允許你嘗試重新排序它
* &lbrack;Project&rbrack;複製材料後，計算永遠不會結束
* &lbrack;Project&rbrack;專案資產在初始專案儲存後會被複製
* &lbrack;Project&rbrack;切換資產時的不必要計算
* &lbrack;Rendering&rbrack;有些圖層堆疊在刪除圖層後無法正常渲染
* &lbrack;Security&rbrack;修正 CVE-2015-20107
* &lbrack;UI&rbrack; 2D 輸出可能會因視窗大小而模糊
* &lbrack;UI&rbrack;資產預覽可以在應用程式失去焦點時保持開啟在最上面
* &lbrack;UI&rbrack;開機畫面圓角呈現方形不透明背景

**已知問題：**

* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作
* &lbrack;內容&rbrack;形狀燈光小工具在球面投影模式下無法運作
* &lbrack;互通性&rbrack;送往Stager的排水物資將失去排水控制

### 3.3.2 櫛瓜

*（發布日期：2022年6月28日）*

**修正：**

* &lbrack;Application&rbrack; 修正開啟專案時可能的當機
* &lbrack;Export&rbrack; 重啟取樣器會破壞匯入的自訂匯出預設列表
* &lbrack;互通性&rbrack;修正從 Designer 傳送的素材被刪除後再從 Designer 重新傳送時的當機
* &lbrack;Project&rbrack;如果最後一個材質或環境燈是專案中的最後一個資產，就無法刪除
* &lbrack;Project&rbrack;右鍵點擊環境燈會顯示「未儲存修改」的星號

**已知問題：**

* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作
* &lbrack;內容&rbrack;形狀燈光小工具在球面投影模式下無法運作
* &lbrack;互通性&rbrack;送往Stager的排水物資將失去排水控制

### 3.3.1 櫛瓜

*（發行日期：2022年6月7日）*

**補充：**

* &lbrack;應用程式&rbrack;原生蘋果矽片（M1）支援
* &lbrack;UI&rbrack;新增快捷鍵，「C」鍵，可在 2D 視圖中切換通道
* &lbrack;工具&rbrack;數值欄位用於在筆刷工具列中編輯灰階色彩值

**修正：**

* &lbrack;Tools&rbrack;在 Windows 上使用 Brush 工具搭配分數 UI 比例（150%）時，可以偏移筆劃
* &lbrack;效能&rbrack;改善記憶體消耗
* &lbrack;物理尺寸&rbrack;啟用此功能時，物理尺寸資訊可能會遺失
* &lbrack;UI&rbrack;滑鼠捲動有時按Alt鍵時無法如預期運作
* &lbrack;Application&rbrack;應用程式在開啟已儲存專案時可能會當機
* &lbrack;Application&rbrack;在材質建立範本視窗中拖放多張圖片並使用材質匯入時會當機
* &lbrack;Application&rbrack;儲存包含自訂過濾器的專案時可能當機
* &lbrack;Application&rbrack;有時切換應用程式時會遺失控制鍵狀態
* &lbrack;Assets&rbrack;重新命名本地資料夾時會崩潰

**已知問題：**

* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作
* &lbrack;內容&rbrack;形狀燈光小工具在球面投影模式下無法運作
* &lbrack;互通性&rbrack;送往Stager的排水物資將失去排水控制

### 3.3.0 櫛瓜

*（發行日期：2022年5月17日）*

**補充：**

* &lbrack;內容&rbrack;新的內容感知填充過濾器（Windows 與 Mac）
* &lbrack;內容感知填充正在處理影像、PBR 材質和環境光源
* &lbrack;Content&rbrack; 將「保留平鋪」參數加入影像至材質（AI 驅動）
* &lbrack;內容&rbrack;透視轉換濾鏡可在四個點之間顯示格子
* &lbrack;互通性&rbrack;將資料傳送至 Adobe Substance 3D Stager
* &lbrack;Tools&rbrack;在調整變形或裁切工具大小時，按 Ctrl 鍵將變形置中
* &lbrack;Tools&rbrack;調整變換或裁切工具時，按 Shift 鍵鎖定正方形比例
* &lbrack;工具&rbrack;複製印章游標提供將要蓋印的預覽
* &lbrack;Tools&rbrack;使用複製印章時，可在橡皮擦游標中預覽原始內容
* &lbrack;Tools&rbrack; Ctrl+Click 會在複製印章圖層建立新印章
* &lbrack;工具&rbrack;連續的複製印章現在被歸類在同一層中
* &lbrack;工具&rbrack;筆刷工具列介面改版
* &lbrack;Tools&rbrack;刷子工具列的位置在工作階段中持續存在
* &lbrack;工具&rbrack;新的按軸線刷子平鋪選項
* &lbrack;Tools&rbrack;上色時將覆蓋層隱藏/顯示在 2D 視圖上
* &lbrack;工具&rbrack;新增快捷鍵「X」鍵，可在刷子與橡皮擦間切換
* &lbrack;Tools&rbrack;新快捷鍵「&lbrack;」「&rbrack;」可更改筆刷大小
* &lbrack;工具&rbrack;新的捷徑，「E」鍵，用來切換橡皮擦
* &lbrack;2D View&rbrack;新球面投影模式，用於建立環境光
* &lbrack;2D View&rbrack;支援球面投影模式的筆刷工具
* &lbrack;2D View&rbrack;位置工具支援球面投影模式
* &lbrack;2D View&rbrack;球面投影模式支援復原/重做
* &lbrack;2D View&rbrack;在球面投影中，設定預設位置為觀看環境中心
* &lbrack;2D View&rbrack;新的曝光控制
* &lbrack;UI&rbrack;在屬性面板中，圖片調整顯示內容來源（圖片或圖層）
* &lbrack;UI&rbrack;改進了圖層/材質輸出的下拉選單背景
* &lbrack;UI&rbrack;解析度資訊在2D視圖中新位置
* &lbrack;UI&rbrack;新增工具提示，包含 3D 視圖導航控制快捷鍵
* &lbrack;UI&rbrack;新工具提示及筆刷控制
* &lbrack;UI&rbrack;新增工具提示，包含投影導航控制快捷鍵
* 複合濾鏡處理變化，用於影像、PBR材質及環境光
* &lbrack;複合過濾器&rbrack;調整順序與複合過濾器中節點的列表順序相符
* &lbrack;複合過濾器&rbrack;同一群組不同節點的調整會在屬性面板合併成一個群組
* &lbrack;Application&rbrack;為每個資產類型設置專用的檢視器設定

**修正：**

* &lbrack;Application&rbrack;應用程式切換到2D視圖時可能會當機
* &lbrack;Application&rbrack;多次匯出時可能的死結或當機
* &lbrack;Application&rbrack;為與 Substance 3D Designer 一致的通道設定預設值
* &lbrack;Application&rbrack; 載入專案不會觸發材料重新計算
* &lbrack;Application&rbrack; 已更新 URL 以提供材質匯入文件
* &lbrack;Content&rbrack;使用複合過濾器時，載入時會要求更新，但不該更新
* &lbrack;內容&rbrack;使用不透明度混合時，高度圖中的細節會消失
* &lbrack;UI&rbrack;在色彩對話框中，可以利用滑桿的文字欄位跳出範圍
* &lbrack;UI&rbrack;使用清單有一個沒用的垂直滾動列

**已知問題：**

* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作
* &lbrack;內容&rbrack;形狀燈光小工具在球面投影模式下無法運作
* &lbrack;互通性&rbrack;送往Stager的排水物資將失去排水控制

### 3.2.1 燒鳥

*（發行日期：2022年3月8日）*

**補充：**

* &lbrack;Export&rbrack; 匯出影像檔案中的 dpi 元資料
* &lbrack;物理尺寸&rbrack;編輯物理尺寸時，保持非正方形材質的比例
* &lbrack;物理大小&rbrack;物理大小元資料在物理大小改變時立即套用
* &lbrack;UI&rbrack; 調整高度比例最大滑桿，使它能在啟用實體尺寸時影響任何材質
* &lbrack;UI&rbrack;資產面板中新增搜尋篩選器工具提示
* &lbrack;UI&rbrack;使用工具提示說明資產面板中按鈕何時被禁用
* &lbrack;內容&rbrack;亮度對比度濾鏡更新

**修正：**

* &lbrack;2D View&rbrack;裁切和變形工具中的 90 度旋轉按鈕無法如預期運作
* &lbrack;2D 檢視&rbrack;裁切小工具有時會遺失
* &lbrack;Application&rbrack;清除影像參數不會重新連接底層。
* &lbrack;Application&rbrack;儲存專案後出口當機
* &lbrack;Application&rbrack;拖放當前素材到資產面板集合時會當機
* &lbrack;Application&rbrack;拖放資產在視窗中可能會當機
* &lbrack;Content&rbrack;普通混合有隨機的種子調整
* &lbrack;Content&rbrack; 雪濾器的正常輸出會根據新鮮和融化雪的參數值而不正確
* &lbrack;Content&rbrack; 拼花過濾器：固定意外接縫
* &lbrack;內容&rbrack; 刺繡過濾器：在金屬地圖中移除線
* &lbrack;內容&rbrack; 地板磚篩選器：修正 x 和 y 磚的計數
* &lbrack;Content&rbrack;磚牆濾波器：輸出標準，高度為16位元
* &lbrack;Export&rbrack;匯出彈出視窗中的預設檔名並非目前的材質名稱
* &lbrack;Export&rbrack;以物理比例匯出並使用出口預設會導致錯誤的尺寸
* &lbrack;Export&rbrack;CLO export 預設中缺少金屬
* &lbrack;Export&rbrack;替換匯出自訂預設時，顯示名稱不會更新
* &lbrack;Layers&rbrack;第一個插入圖層的自訂通道不會被發現
* &lbrack;Layers&rbrack;在更改隱藏圖層微調時會重新評估材質
* &lbrack;Localization&rbrack;工具提示不會在匯出面板中本地化
* &lbrack;物理尺寸&rbrack;停用資產的物理尺寸並不會移除物理比例
* &lbrack;Physical Size&rbrack;高度比例值第一次不能設定在滑桿範圍之外
* &lbrack;Physical Size&rbrack;匯入無實體大小的影像會阻止開啟專案
* &lbrack;物理大小&rbrack;物理大小在缺失時錯誤地設為零
* &lbrack;物理尺寸&rbrack;物理尺寸 物理比例勾選框狀態在首次顯示時不會更新
* &lbrack;UI&rbrack;基礎材質與法線至高度沒有類別
* &lbrack;UI&rbrack;游標在繪製圖像時有時會隱形
* &lbrack;UI&rbrack;如果文字欄位為空，請在編輯選單中停用「全部複製」和「全部剪掉」選項
* &lbrack;UI&rbrack;過濾器名稱有錯誤的字元
* &lbrack;UI&rbrack;實體尺寸鎖定按鈕的樣式不正確
* &lbrack;UI&rbrack;資產面板搜尋欄的關閉按鈕不會清除搜尋字串

**已知問題：**

* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作

### 3.2.0 燒鳥

*（發行日期：2022年1月25日）*

**補充：**

* &lbrack;物理尺寸&rbrack;新的物理尺寸面板
* &lbrack;Physical Size&rbrack; 在材質建立範本視窗中新增物理尺寸選項
* &lbrack;物理尺寸&rbrack; 新增實體尺寸測量工具
* &lbrack;物理尺寸&rbrack; 新增物理尺寸自動測量工具
* &lbrack;物理尺寸&rbrack; 新增物理大小診斷工具
* &lbrack;Physical Size&rbrack; 允許設定物理大小的 z 值
* &lbrack;Physical Size&rbrack;下拉選單小工具，用以設定 2D 視圖縮放的等級
* &lbrack;實體尺寸&rbrack;在縮放等級下拉選單新增的「與物理比例顯示」選項
* &lbrack;物理尺寸&rbrack;在縮放下拉選單中新增的「Fit to Physical size」選項
* &lbrack;物理尺寸&rbrack; 在2D視圖中顯示物理大小
* &lbrack;物理尺寸&rbrack;在3D視窗中顯示物理尺寸
* &lbrack;Physical Size&rbrack;在影像匯入對話框中，若有匯入高度圖，請顯示實體尺寸深度
* &lbrack;物理大小&rbrack; 在資產情境選單中顯示物理大小
* &lbrack;物理尺寸&rbrack;在偏好設定中設定長度單位
* &lbrack;物理尺寸&rbrack;尊重物理比例的匯出紋理
* &lbrack;元資料&rbrack;能夠為使用者自創資產新增自訂元資料
* &lbrack;Export&rbrack; 將自訂元資料匯出為 .sbs（ar） 檔案
* &lbrack;Export&rbrack;將描述、分類、作者及標籤元資料匯出至 .sbs（ar） 檔案
* &lbrack;Export&rbrack; 把實體大小匯出成 .sbs（ar） 檔案
* &lbrack;Export&rbrack; 設定 .sbsar 檔案壓縮設定
* &lbrack;Export&rbrack;將資產縮圖匯出為 .sbs（ar） 檔案
* &lbrack;Export&rbrack;匯出 .sbs（ar） 檔案時設定圖表類型
* &lbrack;Application&rbrack;Realtime Engine 2021 已不再提供
* &lbrack;Application&rbrack;復原/重做現在支援平鋪（U，V）及高度縮放滑桿的變更
* &lbrack;Rendering&rbrack;當作者資產被儲存時產生磁碟快取
* &lbrack;Assets&rbrack; 使用 Ctrl+Click 在資源面板中啟用多種資產類型篩選
* &lbrack;UI&rbrack;能鎖定平鋪（U，V）滑桿
* &lbrack;UI&rbrack;新增一個包含「複製」、「剪切」、「貼上」、「全部複製」和「全部剪掉」的上下文選單
* &lbrack;UI&rbrack;長度單位（公尺、英吋、秒差距等） 標籤與文字欄位支援
* &lbrack;UI&rbrack;使用者可以設定用於顯示數字的十進位精度
* &lbrack;UI&rbrack;在所有相關的小節彈出視窗中使用單位
* &lbrack;Localization&rbrack;預設新資產名稱已在地化
* &lbrack;內容&rbrack;新布織產生器
* &lbrack;內容&rbrack;新頻道切換濾波器
* &lbrack;內容&rbrack;所有相關過濾器現在都知道實體大小
* &lbrack;內容&rbrack;木質塗裝的新圖示
* &lbrack;內容&rbrack;所有過濾器現在都相容於 Adobe Standard Materials（ASM）頻道
* &lbrack;內容&rbrack;過濾器現在可以有「環境」變化

**修正：**

* &lbrack;2D View&rbrack;頻道移除後仍留在列表中
* &lbrack;Application&rbrack;無法複製從作業系統檔案總管載入的資產
* &lbrack;Application&rbrack;出口崩潰
* &lbrack;Application&rbrack;有時點擊「Starter Assets」面板的「Starter Assets」時會當機
* &lbrack;Application&rbrack;刪除材料時的崩潰
* &lbrack;Application&rbrack;環境變數「SUBSTANCE_DISABLE_SPECIFIC_FEATURES」在設定為「0」或「」時仍然有效。
* &lbrack;Application&rbrack;在儲存多個材料的專案時凍結
* &lbrack;Application&rbrack;匯入映像檔可能導致當機
* &lbrack;Application&rbrack;首次推出時缺少一些起始資產
* &lbrack;出口&rbrack;出口資產有時會導致崩盤
* &lbrack;Layers&rbrack;當圖層面板關閉或不可見時，無法匯入圖片
* &lbrack;Layers&rbrack;更改語言會使目前資產重新計算
* &lbrack;Layers&rbrack;更改匯入影像的使用方式不會更新應該使用哪個濾波器變體
* &lbrack;Layers&rbrack;在調整下方圖層時，有時無法計算影像到材質（AI）
* &lbrack;Layers&rbrack;影像轉材質（AI）有時會在不需要時重新計算
* &lbrack;Layers&rbrack;當磁碟上有自訂過濾器更新時，不建議更新
* &lbrack;Layers&rbrack;正常頻道有時會有錯誤的像素格式
* &lbrack;Layers&rbrack;即使不可見，某些圖層仍會被計算
* &lbrack;Layers&rbrack;切換圖層可見性時，2D 視圖工具可能會失效
* &lbrack;Layers&rbrack;使用影像轉材質（AI）時，介面會凍結
* &lbrack;Layers&rbrack;切換 Transform 濾波圖層的可見性會破壞 2D 視圖工具，可能導致當機
* &lbrack;Layers&rbrack;移除圖層堆疊時需重複計算過多
* &lbrack;Layers&rbrack;當複合濾波器包含不尋常或自訂的輸入/輸出時，取樣器不會計算該輸入/輸出
* &lbrack;績效&rbrack;資產面板開啟緩慢
* &lbrack;Performance&rbrack;避免對層堆疊進行不必要的重新計算
* &lbrack;Performance&rbrack;載入專案資產太耗時
* &lbrack;Performance&rbrack;磁碟上的渲染快取不可使用
* &lbrack;Performance&rbrack;層間切換很慢
* &lbrack;性能&rbrack;調整材料或過濾器速度很慢
* &lbrack;Project&rbrack;退出時儲存專案可能導致當機
* &lbrack;Rendering&rbrack;移除影像可能會移除所有輸出
* &lbrack;Rendering&rbrack;在調整時，視窗中顯示的渲染時間是錯誤的
* &lbrack;UI&rbrack;在匯出彈出視窗中無法垂直捲動
* &lbrack;UI&rbrack;當沒有東西可匯出時，可以打開匯出彈窗
* &lbrack;UI&rbrack;有些彈出視窗如果內容溢出，則不會捲動
* &lbrack;UI&rbrack;點擊或開啟選單時不會選取文字欄位
* &lbrack;UI&rbrack;屬性面板中混合模式的名稱有時不正確
* &lbrack;UI&rbrack;檔案選單中的儲存選項有時會顯示灰色
* &lbrack;UI&rbrack;重新命名兩個材料後，文字欄位不會消失
* &lbrack;UI&rbrack;偏好設定彈出視窗中打錯字

**已知問題：**

* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作

### 3.1.2 索科阿特爾

*（發行日期：2021年12月14日）*

**修正：**

* &lbrack;互通性&rbrack;從 Bridge 開啟 Substance 3D 取樣器的 .sbsar 檔案，在 Windows 上可能會失敗
* &lbrack;Layers&rbrack;將唯一層移到自己下方會當機
* &lbrack;UI&rbrack;頻道設定按鈕在切換語言時會消失
* &lbrack;UI&rbrack;儲存專案後，屬性面板中的材質名稱會消失
* &lbrack;Assets&rbrack;點擊「所有函式庫」可能會導致當機

**已知問題：**

* &lbrack;Realtime Engine 2021&rbrack;繁重計算可能導致應用程式當機
* &lbrack;Realtime Engine 2021 會當機，安裝在同時安裝 AMD CPU 和 Nvidia GPU 的 Windows 電腦上
* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作

### 3.1.1 索科阿特爾

*（發行日期：2021年11月24日）*

**補充：**

* &lbrack;互通性&rbrack;將資產（SBS 或 SBSAR）傳送至 Substance 3D Designer
* &lbrack;互通性&rbrack;在偏好設定中設定與 Substance 3D Designer 互通的預設格式
* &lbrack;互通性&rbrack;從 Adobe Bridge 接收多個資產
* &lbrack;UI&rbrack; 新隨機種子小工具
* &lbrack;UI&rbrack;右鍵選單更新
* &lbrack;Assets&rbrack;將圖片從資產面板拖放到屬性面板
* &lbrack;Project&rbrack;資產名稱會被淨化以避免某些特定字元
* &lbrack;品牌設定&rbrack;更新SBSAR檔案圖示
* &lbrack;Engine&rbrack;更新物質引擎版本 8.3.0

**修正：**

* &lbrack;Content&rbrack; 裁切 - 裁切非正方形影像時的保留比例
* &lbrack;內容&rbrack; 轉換 - 使用小工具時水平轉換不會被反轉
* &lbrack;Content&rbrack; Gravel - 修正所有通道的自訂遮罩繪畫
* &lbrack;內容&rbrack;地板磚 - 修正圖案平鋪與重複的問題
* &lbrack;Assets&rbrack;如果未安裝 Adobe Bridge 選項，請將 Adobe Bridge 選項變灰
* &lbrack;色彩選擇器&rbrack;Esc鍵關閉色彩選擇器
* &lbrack;Rendering&rbrack; 修正使用灰階輸入時的散射距離縮放問題
* &lbrack;分享&rbrack;傳送選項僅在 Adobe 授權下提供
* &lbrack;Project&rbrack; 修復記憶體效能問題

**已知問題：**

* &lbrack;Realtime Engine 2021&rbrack;繁重計算可能導致應用程式當機
* &lbrack;Realtime Engine 2021 會當機，安裝在同時安裝 AMD CPU 和 Nvidia GPU 的 Windows 電腦上
* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作

### 3.1.0 索科阿特爾

*（發行日期：2021年9月28日）*

**補充：**

* &lbrack;色彩選擇器&rbrack;全新色彩選擇器使用者介面
* &lbrack;色彩選擇器&rbrack;並排預覽當前與過去的顏色
* &lbrack;Color Picker&rbrack;以十六進位輸入你的顏色
* &lbrack;色彩選擇器與新吸管，附色彩預覽
* &lbrack;Color Picker&rbrack;吸管可以在 Sampler 之外選擇顏色
* &lbrack;色彩選擇器&rbrack;在 RGB 或 HSV 色彩空間中調整你的顏色
* &lbrack;色彩選擇器&rbrack;儲存與管理色色
* &lbrack;互通性&rbrack;在 Illustrator 中從影像匯入圖層或影像參數編輯圖片
* &lbrack;互通性&rbrack;從 Photoshop 中的影像匯入圖層或影像參數編輯圖片
* &lbrack;Widget&rbrack;新作物小工具
* &lbrack;Widget&rbrack;按 Enter 來驗證你的作物
* &lbrack;Widget&rbrack;裁切小工具會讀取圖片大小以符合小工具，並在調整大小時保持比例
* &lbrack;UI&rbrack; New gresycale 滑桿 UI
* &lbrack;Application&rbrack; 在偏好設定中新增正常格式選擇
* &lbrack;Application&rbrack;影像匯入圖層中的正常格式遵循偏好設定中預設的標準格式
* &lbrack;Application&rbrack;在2D視圖中，法線會依照偏好設定的法線格式顯示
* &lbrack;Application&rbrack;normal 格式匯出於偏好設定中。
* &lbrack;Export&rbrack;為 SBS 與 SBSAR 檔案匯出新增正常格式參數
* &lbrack;Export&rbrack;為 SBS 和 SBSAR 檔案匯出新增著色器設定
* &lbrack;Export&rbrack; 設定匯出 SBS 圖表的預設解析度
* &lbrack;複合濾波器&rbrack; 配備 7z 的 SSA 濾波器
* &lbrack;複合過濾器&rbrack; 在複合過濾器中加入類別元資料
* &lbrack;複合濾波器&rbrack;複合濾波器可以嵌入縮圖
* &lbrack;Compound Filters&rbrack; 在取得內容的檔案對話框中新增了 Compound Filters 副檔名（.ssafilter）
* &lbrack;Compound Filters&rbrack; 在資產面板匯入複合過濾器（.ssafilter）
* &lbrack;Engine&rbrack; 更新物質引擎至 v8.2.0

**修正：**

* &lbrack;Application&rbrack;連接的本地資料夾可能會掛掉
* &lbrack;Application&rbrack;出口崩潰
* &lbrack;Application&rbrack;啟動兩個 Sampler 實例時當機
* &lbrack;Content&rbrack;作物過濾器有隨機的種子調整
* &lbrack;內容&rbrack;有些物質材料有時不會升級
* &lbrack;Export&rbrack;匯出新新增的自訂預設時崩潰
* &lbrack;出口&rbrack;出口彈窗中缺少估計包裹大小
* &lbrack;Export&rbrack; 解決匯出 SBS 與 SBSAR 檔案時的記憶體洩漏
* &lbrack;複合濾波器&rbrack;複合濾波器可能有重複輸入
* &lbrack;複合濾波器&rbrack;若濾波器有未被滿足的參考，則崩潰
* &lbrack;複合濾波器&rbrack;在重新排序包含複合濾波器的層堆疊時會崩潰
* &lbrack;複合濾鏡&rbrack;渲染有時會卡住
* &lbrack;影像匯入&rbrack;匯入一張影像會觸發多個渲染
* &lbrack;Layers&rbrack; 在復原/重做時崩潰
* &lbrack;Layers&rbrack;加入基材時崩潰
* &lbrack;Layers&rbrack; 使用無效影像作為環境光時會當機
* &lbrack;Layers&rbrack; 修正插入含多個圖形的過濾器時重複匯入問題
* &lbrack;Layers&rbrack;重新排序圖層並不總是有效
* &lbrack;Project&rbrack;載入未完成專案檔案時當機
* &lbrack;Project&rbrack;開啟損壞專案時當機
* &lbrack;Project&rbrack;有些資產可能會從專案中消失
* &lbrack;Properties&rbrack; 修正缺少濾鏡預設
* &lbrack;UI&rbrack; 角度參數無法設定
* &lbrack;UI&rbrack; 篩選資產面板中的元資料顯示
* &lbrack;UI&rbrack;依類別分組可隱藏篩選器
* &lbrack;UI&rbrack;資產面板中的捲動問題
* &lbrack;UI&rbrack;匯出面板現在有滾動條
* &lbrack;UI&rbrack;某些圖片格式的縮圖在圖片選擇器中不會顯示

**已知問題：**

* &lbrack;Realtime Engine 2021&rbrack;繁重計算可能導致應用程式當機
* &lbrack;Realtime Engine 2021 會當機，安裝在同時安裝 AMD CPU 和 Nvidia GPU 的 Windows 電腦上
* &lbrack;色彩選擇器&rbrack;在第二台螢幕上選擇不同解析度的顏色可能無法運作

### 3.0.1 鬆餅

*（發行日期：2021年7月27日）*

**補充：**

* &lbrack;Brush&rbrack;如果影像輸入支援，請在筆刷工具中啟用顏色
* &lbrack;Brush&rbrack;按住刷子工具中的 Shift 鍵可畫出直線
* &lbrack;Brush&rbrack; 在刷子工具中按住 shift 鍵時，顯示線條預覽
* &lbrack;Brush&rbrack;刷子工具現在支援復原與重做
* &lbrack;2D View&rbrack;圖像輸入時使用預設顏色。
* &lbrack;Layers&rbrack; 在 SBSAR 檔案中讀取 Substance 輸入預設值
* &lbrack;Rendering&rbrack; 允許將高度與法線合併
* &lbrack;Rendering&rbrack;次表面散射支援（MacOS 上無法提供）
* &lbrack;Assets&rbrack;使用 SBSAR 圖形類型來判定資產類型
* &lbrack;資產&rbrack;資產面板中搜尋與資產發現的效能提升
* &lbrack;Assets&rbrack;在資產面板新增了一個「所有函式庫」條目，顯示所有函式庫的所有資產
* &lbrack;Assets&rbrack;使用者現在可以選擇依類別或類型來分組資產
* &lbrack;Import&rbrack;自動偵測各向異性、塗層、光澤及鏡面邊緣色彩紋理，匯入時
* &lbrack;UI&rbrack;將省略面板標題替換成圖示
* &lbrack;UI&rbrack;Textfields 風格更新
* &lbrack;UI&rbrack;環境光源範本建立視窗中的新描述文字
* &lbrack;Application&rbrack;傳送至外部應用程式時，匯出以當前解析度的資產
* &lbrack;Application&rbrack;Material 預設解析度現在為 2048\*2048（macOS 為 1024\*1024）
* &lbrack;內容&rbrack;地板磚過濾器中的新圖案
* &lbrack;內容&rbrack;色彩替換濾鏡中的新雙色模式

**修正：**

* &lbrack;2D 視圖&rbrack;刷子工具的第一筆有時會壞掉
* &lbrack;2D 檢視&rbrack;當刷子工具不可見時，免費資源
* &lbrack;2D View&rbrack;在變換元件中使用右邊的調整大小游標
* &lbrack;2D 視圖&rbrack;若使用者先前在 2D 視圖中平移過，則不會顯示小工具
* &lbrack;Application&rbrack;開啟專案時工作流程故障
* &lbrack;Application&rbrack; 修正應用程式關閉，避免日誌中充斥無用錯誤
* &lbrack;Application&rbrack;重做、刪除並儲存鍵盤快捷鍵在某些作業系統上無法使用
* &lbrack;Application&rbrack; 還原/重做 在匯入圖層更改影像使用是壞掉的
* &lbrack;Export&rbrack;輸出顏色匯出影像名稱錯誤
* &lbrack;Export&rbrack;使用 SBSAR 匯出時，環境為 8 位元
* &lbrack;Export&rbrack; 移除匯出影像檔名中的多餘空格
* &lbrack;Export&rbrack;替換或刪除自訂匯出預設會當機
* &lbrack;Layers&rbrack; 避免輸入計數不匹配時當機
* &lbrack;Layers&rbrack; 插入基礎材質圖層時崩潰
* &lbrack;Layers&rbrack; 濾波器輸入數量被限制為預設值
* &lbrack;Layers&rbrack;重做錯誤地將混合類型改為高度混合
* &lbrack;Layers&rbrack; 移除輸入標頭上方的下落區
* &lbrack;Layers&rbrack; 層入錯誤位置，圍繞輸入標頭
* &lbrack;Layers&rbrack; 重置所有設定按鈕不會重置下拉選單小工具的值
* &lbrack;Layers&rbrack; 在更改圖片匯入圖層時，還原/重做會標記專案為修改，因此要儲存
* &lbrack;Layers&rbrack;使用可能會被混合層停止
* &lbrack;Project&rbrack;載入缺少相依資料夾的舊專案時當機
* &lbrack;Project&rbrack;儲存後使用復原/重做時會當機
* &lbrack;Project&rbrack;打開包含環境光源的 SBSAR 檔案會建立一個材質資產
* &lbrack;Project&rbrack;重新命名材質可觸發縮圖產生
* &lbrack;Project&rbrack;重新命名材質後儲存時，該專案標記為未修改
* &lbrack;Project&rbrack;在重新命名素材後，有些變更不會被儲存
* &lbrack;Rendering&rbrack;在 2020 即時引擎下，環境中可見亮點
* &lbrack;Rendering&rbrack;使用 Real Time Engine 2021 調整大小時當機
* &lbrack;Rendering&rbrack;在高度層級變化時重新計算陰影
* &lbrack;Assets&rbrack;連接資料夾在新增無效檔案時停止索引新資產
* &lbrack;Assets&rbrack;連接包含多個素材的本地資料夾時會當機
* &lbrack;UI&rbrack;2D/3D 視圖按鈕缺少工具提示
* &lbrack;UI&rbrack;資產面板中的所有資產在上市時都會被重點標示
* &lbrack;UI&rbrack;Breadcrumbs 有時會在匯入素材時消失在資產面板中
* &lbrack;UI&rbrack;更改語言不會影響專案面板
* &lbrack;UI&rbrack; 通道設定面板顯示舊有工作流程資訊
* &lbrack;UI&rbrack; 在屬性面板中正確對齊「此項目無設定」字樣，且未調整
* &lbrack;UI&rbrack;元素在歡迎畫面和偏好設定彈出視窗中錯位
* &lbrack;UI&rbrack;面板標題寬度不正確
* &lbrack;UI&rbrack;在屬性面板中，捲動有時會出問題
* &lbrack;UI&rbrack;啟動畫面比例不正確且模糊
* &lbrack;UI&rbrack;全螢幕模式並非全螢幕
* &lbrack;UI&rbrack;即使應用程式在 MacOS 上未啟用，未接駁面板也總是在最上面
* &lbrack;UI&rbrack;更新歡迎畫面橫幅圖片
* &lbrack;Content&rbrack;平鋪濾波器不會處理環境遮蔽通道
* &lbrack;內容與布條;縫線組合與菱形圖案的被子縫問題
* &lbrack;Content&rbrack;Emboss 濾鏡可在 256px x 256px 中運作
* &lbrack;Content&rbrack; 修正當偏移大於 0 時地板磚的磁磚問題

**已知問題：**

* &lbrack;Realtime Engine 2021&rbrack;繁重計算，導致應用程式崩潰
* &lbrack;Realtime Engine 2021 會在同時使用 AMD CPU 和 Nvidia GPU 的 Windows 電腦上當機

### 3.0.0 鬆餅

*（發行日期：2021年6月23日）*

**補充：**

* &lbrack;品牌塑造&rbrack;物質煉金術師變成Adobe Substance 3D取樣器
* &lbrack;品牌與新應用圖示
* &lbrack;UI&rbrack;新使用者體驗與使用者介面
* &lbrack;UI&rbrack;新啟動畫面
* &lbrack;UI&rbrack;面板在介面中既無法對接，也可停靠
* &lbrack;UI&rbrack;在同一欄最多可對接3個面板
* &lbrack;UI&rbrack;在同一面板中最多可擴充 3 個面板（分頁）
* &lbrack;UI&rbrack; 脫離底座面板以在同一或不同螢幕中建立獨立視窗
* &lbrack;UI&rbrack;點擊圖示時，封閉面板會跳出視窗
* &lbrack;UI&rbrack;透過移動面板圖示重新排列左右條
* &lbrack;UI&rbrack;新增工具列，可直接存取特定篩選條件（裁切、變換、透視轉換、複製印記）
* &lbrack;UI&rbrack;左側欄新增「Get Content」按鈕
* &lbrack;UI&rbrack;直接用「取得內容」按鈕匯入你的資產檔案
* &lbrack;UI&rbrack; 直接用「取得內容」按鈕匯入檔案到你的圖層
* &lbrack;UI&rbrack; 直接使用 Adobe Substance 3D 資產網站，使用「取得內容」按鈕
* &lbrack;UI&rbrack;解析度小工具現在可直接在視窗中存取
* &lbrack;UI&rbrack;所有 UI 元素現在都動態載入
* &lbrack;UI&rbrack; 快捷鍵 - 使用「2」來切換 2D 視圖的可見性
* &lbrack;UI&rbrack; 快捷鍵 - 使用「3」來切換 3D 視圖的可見性
* &lbrack;歡迎畫面&rbrack;用新建按鈕一鍵建立專案
* &lbrack;歡迎螢幕&rbrack;新藝術作品橫幅
* &lbrack;Project&rbrack;所有專案現在都關聯到一個唯一的檔案
* &lbrack;Project&rbrack;新專案副檔名 .ssa
* &lbrack;Project&rbrack;「另存為專案」會要求你選擇要儲存專案的位置
* &lbrack;Project&rbrack;結束取樣器會要求你儲存專案（如果沒有儲存）
* &lbrack;Project&rbrack;關閉取樣器會要求你儲存專案，若自上次存檔以來有修改
* &lbrack;Project&rbrack;你的專案名稱會顯示在視窗上方
* &lbrack;Project&rbrack;若專案名稱未被儲存或包含自上次存檔以來的修改，則以斜體加星標示
* &lbrack;Project&rbrack;直接從作業系統檔案總管開啟 .ssa 專案檔案
* &lbrack;Project&rbrack;從作業系統檔案總管開啟 .sbsar 檔案，即可啟動帶有新專案的 Sampler，並準備使用此 .sbsar 檔案
* &lbrack;Project&rbrack;從作業系統檔案總管開啟一個 .alch（舊有的 Substance Alchemist 檔案）
* &lbrack;專案面板&rbrack;新增面板，將包含專案內所有資產
* &lbrack;專案面板&rbrack;使用 + 圖示建立資產（材質或環境燈光）
* &lbrack;專案面板&rbrack;右鍵點擊資產會開啟一個右鍵選單
* &lbrack;專案面板&rbrack;從右鍵右鍵選單中，你可以刪除資產
* &lbrack;專案面板&rbrack;從右鍵右鍵選單，你可以複製資產
* &lbrack;專案面板&rbrack;從右鍵右鍵選單，你可以重新命名資產
* &lbrack;專案面板&rbrack;在資產間切換不會失去修改
* &lbrack;解析度&rbrack;你現在可以為所有資產設定非正方形解析度
* &lbrack;Resolution&rbrack;解析度值依專案中資產儲存
* &lbrack;環境光&rbrack; 在 Substance 3D 取樣器中建立環境光
* &lbrack;環境燈光&rbrack;建立環境燈時，拖放圖片會顯示環境光源建立範本視窗
* &lbrack;Environment Light&rbrack;在 Environment Light Creation 範本中，選擇 Environment Import 以將你的影像指派到 3D 視圖中的環境
* &lbrack;環境光源&rbrack;在環境光源建立範本中，選擇 HDR 合併，從多張不同曝光的 360 度影像中建立環境光
* &lbrack;Environment Light&rbrack;在環境光源建立範本中，選擇「用作點陣圖」以編輯你的圖片，然後再建立環境光源
* &lbrack;Environment Light&rbrack; 在 Image Import 圖層中指派環境使用，直接將影像指派到 3D 視圖中的環境
* &lbrack;環境光照&rbrack;在環境通道的 2D 視圖中，有自動色彩校正功能，使渲染呈現與 3D 視圖相同
* &lbrack;環境光&rbrack;全新專為環境光源創作而設的內容
* &lbrack;資產面板&rbrack;資源面板與過濾器面板合併成一個新的資產面板
* &lbrack;資產面板&rbrack;資產面板現在支援以下素材類型：材質、濾鏡與圖片
* &lbrack;資產面板&rbrack;所有入門資產皆可在入門資產區段存取
* &lbrack;資產面板&rbrack;入門資產區塊為唯讀
* &lbrack;資產面板&rbrack;新增「您的資產」區塊
* &lbrack;Assets Panel&rbrack;「你的資產」區塊是你可以匯入所有資源的地方
* &lbrack;資產面板&rbrack;「你的資產」中的所有資產都會被加入文件中的特定資料夾
* &lbrack;Assets Panel&rbrack; 在資產面板中連接本地資料夾以新增區段
* &lbrack;Assets Panel&rbrack;搜尋會在目前資料夾及其子資料夾中搜尋
* &lbrack;資產面板&rbrack;在資料夾與子資料夾間以麵包屑導航
* &lbrack;Assets Panel&rbrack;依材質、濾鏡或圖片過濾目前資料夾
* &lbrack;資產面板&rbrack;結合多個濾鏡，只取得材質與圖片
* &lbrack;資產面板&rbrack;透過切換格線或列表來改變顯示
* &lbrack;資產面板&rbrack;過濾器以其圖示表示
* &lbrack;資產面板&rbrack;圖片以預覽形式呈現
* &lbrack;Assets Panel&rbrack;增加寬度會改變面板的佈局，並以特定視角在資料夾間導航
* &lbrack;Assets Panel&rbrack;在非唯讀區段，將資產拖放到垃圾桶圖示上刪除
* &lbrack;資產面板&rbrack;右鍵點擊資產即可開啟右鍵選單
* &lbrack;資產面板&rbrack;從右鍵右鍵選單，存取資產元資料（名稱、類別、位置）
* &lbrack;資產面板&rbrack;從右鍵右鍵選單刪除該資產（僅在非唯讀區段可用）
* &lbrack;資產面板&rbrack;從右鍵右鍵選單，瀏覽 Adobe Bridge 中的資產
* &lbrack;Layers Panel&rbrack;新增圖示，直接在圖層上方新增基底材質
* &lbrack;Layers Panel&rbrack;快捷鍵 - Shift + B 會在你的圖層上方新增一個基底材質
* &lbrack;圖層面板&rbrack;圖層現在有縮圖預覽（材質縮圖、濾鏡圖示或圖片預覽）
* &lbrack;屬性面板&rbrack;屬性面板標題的新設計，包含資產名稱與縮圖
* &lbrack;屬性面板&rbrack;濾波器圖層現在支援預設
* &lbrack;屬性面板&rbrack;在影像匯入圖層中，右鍵點擊圖片預覽以在 Photoshop 中編輯圖片
* &lbrack;Adobe Bridge&rbrack;在 Adobe Bridge 中瀏覽您的資產，會在資產所在地啟動 Bridge。
* &lbrack;Adobe Photoshop&rbrack;在 Adobe Photoshop 編輯時，圖片會在 Photoshop 中開啟，準備進行編輯
* &lbrack;Adobe Photoshop&rbrack;每次在 Adobe Photoshop 儲存時，編輯後的圖片都會重新載入 Sampler
* &lbrack;Substance 3D Designer&rbrack;從 Adobe Substance 3D Designer 傳送的資產將直接出現在資產面板的「Your Assets」區塊
* &lbrack;Export&rbrack;直接將素材傳送到 Adobe Substance 3D Painter 和 Adobe Substance 3D Stager
* &lbrack;匯出&rbrack;將材質與環境光源傳送至 Adobe Substance 3D Painter
* &lbrack;Export&rbrack; 將環境燈光傳送至 Adobe Substance 3D Stager
* &lbrack;Rendering&rbrack;新增材質屬性現已支援並以 3D 呈現
* &lbrack;Rendering&rbrack;添加光澤支持（光澤顏色、光澤不透明度與光澤粗糙度）
* &lbrack;渲染&rbrack;添加塗層支援（毛色、毛髮粗糙度、毛色法線、毛皮鏡面水平及毛皮IOR）
* &lbrack;Rendering&rbrack;新增各向異性支援（各向異性水準與各向異性角度）
* &lbrack;Rendering&rbrack; 新增鏡面邊緣色彩支援
* &lbrack;Rendering&rbrack;在通道設定面板中啟用這些新屬性
* &lbrack;Rendering&rbrack;2021 年推出全新 Realtime Engine 渲染器，測試版
* &lbrack;Rendering&rbrack;在檢視器設定面板中切換兩個渲染器版本
* &lbrack;Rendering&rbrack;Realtime Engine （2021） 渲染器支援半透明、吸收及散射材質屬性
* &lbrack;Rendering&rbrack;Realtime Engine （2021） 渲染器引入了一種從環境光線計算陰影的新方法
* &lbrack;渲染&rbrack;即時引擎（2021）渲染器即時計算環境光的輻照度
* &lbrack;著色器設定面板&rbrack;新的著色器設定面板用來調整特定材質著色器的參數
* &lbrack;著色器設定面板與rbrack;新增參數（正常比例、高度比例、高度等級、發射強度、IOR、毛色正常強度及毛皮IOR）
* &lbrack;著色器設定面板&rbrack;Realtime Engine 2021 的特定參數（次表面散射、散射距離、紅移與瑞利散射）
* &lbrack;著色器設定面板&rbrack;設定值會儲存在每個資產上
* &lbrack;檢視器設定面板&rbrack;新增預設環境燈的預覽
* &lbrack;檢視器設定面板&rbrack;新增預設網格預覽
* &lbrack;檢視器設定面板&rbrack;新的環境不透明度參數
* &lbrack;檢視器設定面板&rbrack;新的環境模糊參數（專門針對Realtime Engine 2021渲染器）
* &lbrack;本地化&rbrack;德語與法語新譯本
* &lbrack;內容&rbrack;新的預設入門材料
* &lbrack;內容&rbrack;新的預設環境燈
* &lbrack;內容&rbrack;所有過濾器均已更新、清理與優化
* &lbrack;內容&rbrack;調整過濾器已被拆分成多個過濾器
* &lbrack;內容與rbrack;新的亮度/對比度濾鏡
* &lbrack;內容&rbrack;新色調/飽和濾鏡
* &lbrack;內容&rbrack;新Vibrance濾鏡
* &lbrack;內容&rbrack;新銳化濾鏡
* &lbrack;內容&rbrack;新標準/高度調整
* &lbrack;內容&rbrack;新面板過濾器
* &lbrack;Content&rbrack;新污漬濾波器
* &lbrack;Content&rbrack;新織法過濾器
* &lbrack;Content&rbrack;新 Warp 轉換濾波器
* &lbrack;內容&rbrack;AO濾波器的新高度
* &lbrack;內容&rbrack;新增高度至一般過濾器
* &lbrack;Content&rbrack;色彩替換 - 在新支援的通道（光澤、塗層、各向異性,...）中替換
* &lbrack;內容&rbrack;色彩變化 - 手動模式，精確選擇要更改的顏色
* &lbrack;內容&rbrack; 平鋪 - 可視化接縫切割的選項
* &lbrack;內容&rbrack;瓷磚 - 可以選擇塗漆縫線，切割出完美的瓷磚
* &lbrack;Content&rbrack; Match - 選擇加入材質以匹配其顏色與粗糙度
* &lbrack;Content&rbrack; Match - 現在能讓圖片顏色與另一張圖片相匹配
* &lbrack;內容&rbrack; 環境 左 - 新色溫濾鏡
* &lbrack;Content&rbrack; 環境光 - 新曝光濾鏡
* &lbrack;Content&rbrack; 環境 光 - 新曝光預覽濾鏡
* &lbrack;Content&rbrack; Environment ligth - 新的 Nadir Patch 濾波器
* &lbrack;Content&rbrack; 環境光 - 新 Nadir 萃取過濾器
* &lbrack;Content&rbrack; 環境光 - 新光源濾鏡（球體、線條、形狀、平面）
* &lbrack;Content&rbrack; Environment ligth - 新的全景補丁濾鏡
* &lbrack;Content&rbrack; 環境 左 - 新 Straighten Horizon 濾鏡
* &lbrack;Content&rbrack; Environment ligth - 新的 HDR 合併濾鏡

**已知問題：**

* &lbrack;即時引擎 2021&rbrack;更改版面，導致應用程式崩潰
* &lbrack;Realtime Engine 2021&rbrack;繁重計算，導致應用程式崩潰
* &lbrack;Panels&rbrack;MacOS - 未接駁的面板會放在所有應用程式的前面
* &lbrack;Widgets&rbrack;Transform 和 Positions 的小工具可能會消失。 隱藏和解除隱藏該圖層，讓它們顯現。
* &lbrack;Export&rbrack;環境燈的SBSAR匯出會失去32位元深度的精度
* &lbrack;資產面板&rbrack;資產可在開啟資料夾時被高亮顯示
* &lbrack;Properties Panel&rbrack;重置參數不會重置 combobox 介面
* &lbrack;Localization&rbrack; 改變語言在重建專案面板前不會影響

## 版本 2

### 2.3.2 （2020.3.2） Vermicelli

*（發行日期：2021年2月23日）*

**補充：**

* &lbrack;本地化&rbrack;日本支援

**修正：**

* &lbrack;Layers&rbrack;在刺繡濾鏡中調整材質會失去刺繡圖像

**已知問題：**

* 在高解析度影像上使用影像對材質（AI 驅動）可能較慢
* 內容感知填充濾鏡在高解析度下速度較慢
* 在滑桿中輸入特定evalue時，可以忽略Coma或點
* 不可能儲存兩次完全相同的材質層疊

### 2.3.1 （2020.3.1） Vermicelli

*（發行日期：2020年12月17日）*

**補充：**

* &lbrack;引擎與物質引擎更新
* &lbrack;Application&rbrack; 環境變數以停用特定功能
* &lbrack;Content&rbrack; 替換顏色 - 新的進階分割選項
* &lbrack;內容&rbrack;地板磚——新增圖案與選項
* &lbrack;內容&rbrack; 刺繡 - 濾網全面改造
* &lbrack;Content&rbrack; 調整 - 新增金屬參數 + 不透明度安全轉換修正

**修正：**

* &lbrack;Layers&rbrack; 無法匯入重複相同的自訂濾鏡
* &lbrack;Layers&rbrack;無法使用筆刷工具進行影像輸入
* &lbrack;Export&rbrack;用 Export .jpg 代替 .jpeg
* &lbrack;UI&rbrack;更新：歡迎螢幕圖片來源
* &lbrack;UI&rbrack; 修正選單中的隱形分隔符
* &lbrack;UI&rbrack;單選按鈕被截斷時會顯示提示
* &lbrack;UI&rbrack;打字錯誤：入門材料
* &lbrack;Application&rbrack;資產名稱中的 UTF-8 字元無法使用
* &lbrack;Localization&rbrack;關閉中文區域的斜體字型
* &lbrack;Localization&rbrack;將本地化字串分為兩行
* &lbrack;Localization&rbrack;調整資料夾名稱，如果太長則用省略號取代
* &lbrack;本地化&rbrack;格式號碼與千分隔符
* &lbrack;本地化&rbrack;本地化日期與時間顯示
* &lbrack;Localization&rbrack; 在 Windows 上本地化色彩選擇器
* &lbrack;內容&rbrack; 變換 - 啟用安全變換後，法線會正確旋轉每45°一次
* &lbrack;內容&rbrack; 表面緩和 - 修正 Perlin 分形噪聲（進階噪聲）的鋪磚問題
* &lbrack;Content&rbrack; 磚牆模式 - 16位元高度輸入
* &lbrack;內容&rbrack;材質圖示渲染 - 鏡面反射問題
* &lbrack;內容&rbrack;色彩變化 - 顏色輸入與結果間無色移
* &lbrack;內容&rbrack; 顏色變化 - 效能更新

**已知問題：**

* 在高解析度影像上使用影像對材質（AI 驅動）可能較慢
* 內容感知填充濾鏡在高解析度下速度較慢
* 在滑桿中輸入特定evalue時，可以忽略Coma或點
* 不可能儲存兩次完全相同的材質層疊

### 2.3.0 （2020.3.0） Vermicelli

*（發行日期：2020年10月26日）*

**補充：**

* &lbrack;映像轉材質 &rbrack;支援 NVIDIA RTX 3000 系列
* &lbrack;影像轉材質&rbrack;新參數用來控制幾何細節
* &lbrack;影像轉材料&rbrack;新參數用來控制粗糙度
* &lbrack;影像轉材質&rbrack;新參數用以控制愉悅強度
* &lbrack;縮圖&rbrack;基於Substance Designer的PBR渲染器的新縮圖產生器
* &lbrack;縮圖&rbrack;更新基礎材質和地圖集以嵌入縮圖
* &lbrack;縮圖&rbrack;如果有縮圖，請從 .sbsar 檔案中擷取
* &lbrack;縮圖&rbrack;在偏好設定中更改縮圖品質
* &lbrack;引擎&rbrack;更新為Substance Engine版本8
* &lbrack;本地化&rbrack;中文本地化
* &lbrack;UI&rbrack;實驗性專色選擇器
* &lbrack;內容&rbrack;新環境地圖 - Studio 06
* &lbrack;Content&rbrack; 新增圖集產生器過濾器
* &lbrack;Content&rbrack; 新增 Atlas Splitter filter
* &lbrack;內容&rbrack; 新增棄棄膠質過濾器
* &lbrack;內容&rbrack; 新增指紋過濾器
* &lbrack;內容&rbrack; 新增刮痕過濾器
* &lbrack;內容&rbrack; 新增表面緩解濾波器（取代高度調變濾波器）
* &lbrack;內容&rbrack; 新增變速過濾器
* &lbrack;Content&rbrack; 新增反轉過濾器
* &lbrack;內容&rbrack; 新增著色濾鏡
* &lbrack;內容&rbrack; 新增 替換 色彩調整器
* &lbrack;內容&rbrack; 轉換 - 新增在特定通道上停用轉換的功能
* &lbrack;Content&rbrack; Transform - 在安全變形啟動時加入旋轉
* &lbrack;內容&rbrack; 色彩變化 - 新增分段選項以選擇顏色分配方式

**修正：**

* &lbrack;Layers&rbrack;在執行多次復原/重做動作時，正確更新 UI
* &lbrack;Layers&rbrack; 防止在執行多次復原/重做操作時當機
* &lbrack;Layers&rbrack; 使用 Image to Material（AI 驅動）時當機，log： 裝置序數無效
* &lbrack;Filters&rbrack;提升 NVIDIA 顯示卡對 NVidia 特定功能的偵測
* &lbrack;Application&rbrack;關閉應用程式時崩潰
* &lbrack;Application&rbrack; 修正 MacOS 上的 VRAM 數量偵測
* &lbrack;Export&rbrack;有些匯出預設有時會遺失
* &lbrack;內容與油畫效果 - 固定高高度範圍及高位移振幅
* &lbrack;內容&rbrack;讓它成為圖塊進階 - 匯出時不會有褪色的底色
* &lbrack;內容&rbrack; 讓它成為圖塊進階 - 當 AO 過強時，底色上加白色遮罩
* &lbrack;內容&rbrack; 調整 - 現在可以處理圖片（掃描1，...）

**已知問題：**

* 在高解析度影像上使用影像對材質（AI 驅動）可能較慢
* 內容感知填充濾鏡在高解析度下速度較慢
* 在滑桿中輸入特定evalue時，可以忽略Coma或點
* 不可能儲存兩次完全相同的材質層疊

### 2.2.1 （2020.2.1） Udon

*（發行日期：2020年7月21日）*

**補充：**

* &lbrack;Layers&rbrack;當影像轉材質（AI-Powered）記憶體不足時，應用程式內錯誤訊息

**修正：**

* &lbrack;Layers&rbrack;影像轉材質（AI 驅動）無法支援 Specular/Glossiness 工作流程
* &lbrack;Layers&rbrack;使用影像轉材質（AI驅動）時，視訊記憶體不足時會當機
* &lbrack;Layers&rbrack;磁碟快取在開啟堆疊時不用於顯示
* &lbrack;層數與 brack;Nvidia RTX 8000 偵測
* &lbrack;Layers&rbrack;有時無法將圖層移出 Splatter 輸入
* &lbrack;Layers&rbrack;磁碟快取在插入堆疊時不會使用
* &lbrack;Layers&rbrack;雖然未被使用，但會計算部分通道使用情況
* &lbrack;Layers&rbrack;有時在匯入圖片時會產生空白輸出
* &lbrack;2D 視圖&rbrack;切換到另一層，啟用繪圖模式時，方塊會平移與縮放
* &lbrack;Content&rbrack; Snow - 法線貼圖的 8bit 問題
* &lbrack;Content&rbrack; Pavement Pattern - 法線映射出現 8 位元
* &lbrack;Content&rbrack; Equalizer - 法線映射出現 8 位元
* &lbrack;Content&rbrack; Gravel Generator - 法線映射上的 8 位元
* &lbrack;內容&rbrack;地板磚 - 處理不透明度與鏡面層級
* &lbrack;Content&rbrack; Blender 循環 eeve export preset - 反轉法線貼圖
* &lbrack;內容&rbrack;在影像轉材質（AI 驅動）下，處理巨大圖片的問題
* &lbrack;Application&rbrack;在資料庫錯誤時選擇「備份與重新啟動」時當機
* &lbrack;Application&rbrack;快速點擊同一資產時會當機
* &lbrack;Application&rbrack;退出時罕見當機
* &lbrack;Application&rbrack;在歡迎畫面丟棄檔案時會當機
* &lbrack;Application&rbrack;當環境檔案損壞時當機
* &lbrack;Application&rbrack;快速切換渲染資產時罕見當機
* &lbrack;Application&rbrack;資產正在運算時退出時會凍結
* &lbrack;Application&rbrack;macOS 開機時罕見崩潰
* &lbrack;Application&rbrack;啟動後不久關閉應用程式時會死結
* &lbrack;Rendering&rbrack;3D 視圖有時會閃爍
* &lbrack;UI&rbrack;顏色選擇器和隨機種子小工具並未與其他調整對齊
* &lbrack;Rendering&rbrack;顯示錯誤的計算時間
* &lbrack;Export&rbrack;有些匯出預設有時會遺失

**已知問題：**

* 在高解析度影像上使用影像對材質（AI 驅動）可能較慢
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 內容感知填充濾鏡在高解析度下速度較慢
* 在滑桿中輸入特定evalue時，可以忽略Coma或點
* 不可能儲存兩次完全相同的材質層疊

### 2.2.0 （2020.2.0） Udon

*（發行日期：2020年6月15日）*

**補充：**

* &lbrack;Create&rbrack;全新影像轉材質（AI 驅動）篩選器，適用於 Windows 與 Linux
* &lbrack;Create&rbrack; 將位圖重新命名為 Material to Image 再到 Material（B2M）
* &lbrack;圖片匯入&rbrack;新素材建立範本彈出視窗
* &lbrack;影像匯入&rbrack;新增「新增基礎材質」選項
* &lbrack;圖片匯入&rbrack;能夠在材質建立範本中拖放更多圖片
* &lbrack;影像匯入&rbrack;能夠在材質建立範本中移除圖片
* &lbrack;影像匯入&rbrack;根據檔案名稱自動將通道指派給匯入的點陣圖
* &lbrack;影像匯入&rbrack;能夠反轉法線貼圖
* &lbrack;2D 視圖&rbrack;引入繪畫模式
* &lbrack;2D 視圖&rbrack;繪畫磚塊
* &lbrack;2D 視圖&rbrack;為筆刷顏色設定灰階值
* &lbrack;2D 視圖&rbrack;繪畫時平移與變焦
* &lbrack;2D View&rbrack;X 可將筆刷灰階值反轉的捷徑
* &lbrack;2D View&rbrack; &lbrack; 以及 &rbrack;用來更改筆刷大小的快捷鍵
* &lbrack;2D View&rbrack;Ctrl（或 Cmd）+ 滑鼠滾輪可更改筆刷大小
* &lbrack;2D View&rbrack;現在可以使用 Clone Patch 來修改來源位置
* &lbrack;Layers&rbrack; Shift + 拖放至自動散射圖集
* &lbrack;Layers&rbrack;Alt + 拖放可將材質插入貼紙
* &lbrack;Layers&rbrack;Expose 可輕鬆從 Substance Designer 轉換矩陣
* &lbrack;Layers&rbrack;在非空堆疊中丟棄貼圖會自動分配到正確的通道
* &lbrack;Layers&rbrack;新型層：複合濾波器
* &lbrack;參數&rbrack; 支援 Substance 字串輸入
* &lbrack;UI&rbrack;新增了彈出視窗和選單的陰影效果
* &lbrack;UI&rbrack;新色彩小工具，右鍵可選（清除、複製、貼上）
* &lbrack;UI&rbrack;新影像小工具搭配繪圖工具選項
* &lbrack;UI&rbrack;能夠在影像小工具中繪製匯入的影像
* &lbrack;Rendering&rbrack; 新的預設攝影機位置
* &lbrack;Export&rbrack;Substance 檔案已匯出至 Substance Designer 2020.1.2（10.1.2）
* &lbrack;Performance&rbrack;更好的應用程式啟動時間
* &lbrack;Performance&rbrack;改善非同步任務處理
* &lbrack;效能&rbrack;在增加、移除或移動圖層時，提升圖層堆疊效能
* &lbrack;Performance&rbrack;Image to Material（AI 驅動）在 RTX GPU 上運行更快
* &lbrack;內容&rbrack;新網格：女款T恤、男款T恤、鞋子
* &lbrack;Content&rbrack;新混合模式 - 每個通道混合
* &lbrack;內容&rbrack;不透明度混合高度修正，新增兩個參數（高度位置與高度刻度）
* &lbrack;Content&rbrack; 在 Height Blend 模式中新增高度調整
* &lbrack;內容&rbrack; 在自訂遮罩混合中使用高度資訊選項
* &lbrack;內容&rbrack;新視角校正工具
* &lbrack;內容&rbrack; 模式產生器 - 新增參數以反轉模式
* &lbrack;Content&rbrack; 圖案產生器 - 新增參數 覆蓋材質細節
* &lbrack;Content&rbrack;新貼花濾波器
* &lbrack;Content&rbrack;新苔蘚過濾器
* &lbrack;內容&rbrack;新裂紋過濾器
* &lbrack;Content&rbrack;新的 PBR 驗證過濾器
* &lbrack;內容&rbrack;新地板磁磚過濾器
* &lbrack;內容&rbrack;新拼布縫紉過濾器
* &lbrack;Content&rbrack; Atlas Scatter - 新增自訂遮罩輸入以啟用繪畫選項
* &lbrack;Content&rbrack; Dirt - 新增自訂遮罩輸入以啟用繪畫選項
* &lbrack;Content&rbrack; CLO export preset
* &lbrack;Content&rbrack; VStitcher export 預設
* &lbrack;內容&rbrack; Unity HDRP 預設 匯出 detailMap

**修正：**

* &lbrack;Layers&rbrack;匯入的圖片載入次數過多
* &lbrack;Layers&rbrack;在堆疊底部建立克隆補丁時會崩潰
* &lbrack;Layers&rbrack;在堆疊底部加入材料會使其不穩定
* &lbrack;Layers&rbrack; 影像匯入後的濾鏡運作不正常
* &lbrack;Layers&rbrack;workflow_type值在使用自訂篩選器切換專案間工作流程時不會更新
* &lbrack;Layers&rbrack; 當未選取圖層時，請停用「移除圖層」按鈕
* &lbrack;Layers&rbrack;載入包含克隆補丁的資產時當機
* &lbrack;Layers&rbrack;法線到高度過濾器在 MacOS 上當機
* &lbrack;Application&rbrack;在前後載入環境地圖時會當機
* &lbrack;Application&rbrack;安裝某個繪圖板驅動程式時的效能問題
* &lbrack;Application&rbrack;EXR 32位元檔案匯入為黑色
* &lbrack;Application&rbrack;載入與卸載資產時當機
* &lbrack;Application&rbrack;從探索切換到建立時會當機
* &lbrack;Application&rbrack;目標收集：當儲存材料非來自當前專案時
* &lbrack;Application&rbrack; 修正備份並重新啟動
* &lbrack;影像匯入&rbrack;正確匯入灰階影像
* &lbrack;Content&rbrack;用於新矩陣處理的新過濾器
* &lbrack;內容&rbrack;匯入的自訂篩選器可在快速存取列中看到
* &lbrack;Content&rbrack; 用 Make it tile 進階濾鏡修正色差
* &lbrack;Performance&rbrack;開啟色彩對話框較慢且需重新計算當前層
* &lbrack;UI&rbrack;鍵盤快捷鍵有時無法使用。
* &lbrack;2D 檢視&rbrack;內容感知填充只需無用的第一次點擊即可運作
* &lbrack;Resources&rbrack;本地磁碟中的資料夾在移除後仍會被監控更新
* &lbrack;Resources&rbrack; 從檔案系統刪除連結資料夾並不會移除它
* &lbrack;Export&rbrack;自訂匯出預設中的自訂用法不會被匯出
* &lbrack;Export&rbrack;導出帶有特殊字元的 .sbsar 檔案會失敗

**已知問題：**

* 重複性地重新計算影像到材質（AI 驅動）可能會觸發當機（記憶體不足）
* 重複計算 Delighter 可能會觸發當機（記憶體不足）
* 在高解析度影像上使用影像對材質（AI 驅動）可能較慢
* 在低 VRAM 的 GPU 上使用 Image to Material（AI 驅動）可能會引發當機（記憶體不足）
* 圖片轉材質（AI 驅動）在 PBR 高光/光澤中無法使用
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 內容感知填充濾鏡在高解析度下速度較慢
* 在滑桿中輸入特定evalue時，可以忽略Coma或點
* 不可能儲存兩次完全相同的材質層疊

### 2.1.1 （2020.1.1） Tiramisu

*（發行日期：2020年4月1日）*

**補充：**

* &lbrack;Project&rbrack;匯出與匯入元資料
* &lbrack;Application&rbrack;Ctrl+S 現在可以在 Explore 中儲存預設
* &lbrack;Performance&rbrack;使用渲染快取代替重新計算儲存的素材，解析度最高可達 2k

**修正：**

* &lbrack;UI&rbrack;視窗中的固定計算指標
* &lbrack;UI&rbrack;在滑桿中輸入負值是固定的
* &lbrack;UI&rbrack;組合盒：鍵盤箭頭和滾動條現在都能用了
* &lbrack;UI&rbrack;在 2D 視圖中切換「材質輸出」與「圖層輸入」時，保持所選通道
* &lbrack;Layers&rbrack;修正在 Base Material 新增自訂通道時的當機
* &lbrack;Layers&rbrack;操作圖層時崩潰
* &lbrack;Layers&rbrack;自訂通道不會隨儲存的材質顯示
* &lbrack;Application&rbrack;修正了匯入資產時的罕見崩潰
* &lbrack;Application&rbrack;退出時崩潰
* &lbrack;Application&rbrack;組合盒在切換預設時會顯示正確的數值
* &lbrack;Export&rbrack;將 Enscape 預設名稱改為 Enscape Revit。
* &lbrack;Export&rbrack; 移除匯出預設後，匯入它仍然有效
* &lbrack;出口&rbrack;出口崩盤
* &lbrack;Rendering&rbrack;當基底顏色為 16 位元半浮點格式時，修正渲染
* &lbrack;Project&rbrack; 匯入損壞套件時不會當機
* &lbrack;Project&rbrack;處理 2019.1.4 到 2.x.x 的遷移，當 Create 從未開啟時
* &lbrack;Project&rbrack; 修復匯入同一專案兩次時的崩潰
* &lbrack;Project&rbrack;修正匯入專案時的當機
* &lbrack;Resources&rbrack;先前版本匯入的自訂過濾器可正常運作
* &lbrack;資源&rbrack;同名材料不再互相抹除
* &lbrack;Resources&rbrack;連結本地資料夾時會崩潰
* &lbrack;Resources&rbrack;Starter Materials 使用者建立的資料夾在重新啟動後不會再被移除
* &lbrack;Inspire&rbrack;修正材料/收藏丟棄區，若使用未儲存材料則新增警告訊息

**已知問題：**

* 內容感知填充濾鏡在高解析度下速度較慢
* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 在滑桿中輸入特定evalue時，可以忽略Coma或點

### 2.1.0 （2020.1.0） Tiramisu

*（發行日期：2020年3月12日）*

**補充：**

* &lbrack;Export&rbrack;匯出預設的 selction，用來打包你的材質給渲染器和遊戲引擎
* &lbrack;Export&rbrack;匯出預設為 Unreal Engine 4
* &lbrack;Export&rbrack;匯出預設為 Unity 標準
* &lbrack;Export&rbrack; 匯出預設為 Unity HDRP
* &lbrack;Export&rbrack; 匯出預設為 Blender Cycles/Eevee
* &lbrack;Export&rbrack; 匯出預設為 Arnold 5
* &lbrack;Export&rbrack; 匯出預設為 Corona Renderer
* &lbrack;Export&rbrack; 匯出預設為 Enscape
* &lbrack;Export&rbrack;匯出預設為 Keyshot 9
* &lbrack;Export&rbrack;匯出預設為 Redshift
* &lbrack;Export&rbrack; 匯出預設為 Vray Next
* &lbrack;Export&rbrack; 將預設匯出到 Lens Studio
* &lbrack;Export&rbrack; 匯出預設為 Spark AR Studio
* &lbrack;出口&rbrack;從PBR金屬粗糙度預設為PBR鏡面光澤
* &lbrack;Export&rbrack;新的匯出介面
* &lbrack;Export&rbrack; 記得匯出設定
* &lbrack;Export&rbrack; 匯入並管理你的自訂匯出預設
* &lbrack;Export&rbrack; 刪除並替換你的自訂匯出預設
* &lbrack;Export&rbrack; 重新命名你的自訂匯出預設
* &lbrack;Export&rbrack; 將預設匯出解析度設為目前解析度
* &lbrack;Export&rbrack;將建立子資料夾的選項加入匯出位置
* &lbrack;Export&rbrack; 替換現有檔案前的警告訊息
* &lbrack;應用程式&rbrack;新的版本編號方案
* &lbrack;Application&rbrack;啟動時開啟建立，並更改實驗室順序
* &lbrack;歡迎螢幕&rbrack;新的歡迎橫幅
* &lbrack;專案&rbrack;啟動時開啟最後一個專案
* &lbrack;UI&rbrack;全新組合盒型
* &lbrack;2D 視圖&rbrack;F 快速對焦 2D 視圖
* &lbrack;Filters&rbrack;新增對 alchemist：:p arameterVisibility 標籤的支援，在物質圖中
* &lbrack;Filters&rbrack;根據你的工作流程，做全域調整來管理參數可見性
* &lbrack;Resources&rbrack;新增命令列選項，用以設定檔設定資源與連結資料夾
* &lbrack;版本檢查器&rbrack;版本檢查的配置
* &lbrack;內容&rbrack;新入門教材
* &lbrack;Content&rbrack; Bitmap 轉材質 - 新增定義金屬通道（統一、自訂影像匯入、色彩選擇）的功能
* &lbrack;Content&rbrack; 調整 - 新增 PBR 高光/光澤工作流程的支援
* &lbrack;內容&rbrack;Atlas Scatter - 新參數

**修正：**

* &lbrack;Project&rbrack;匯入同一專案兩次時當機
* &lbrack;Project&rbrack;多次在匯入與開啟專案時修正崩潰
* &lbrack;Application&rbrack;載入未命名材料時當機
* &lbrack;Application&rbrack;重新匯入檔案時辨識缺失檔案
* &lbrack;Application&rbrack; 修正關機時的隨機當機
* &lbrack;Application&rbrack; 修正了在 Create 卸載材料時罕見當機的問題
* &lbrack;Application&rbrack;修正了使用 UI 控制項時的隨機當機
* &lbrack;Application&rbrack; 修正了 Windows 10 上日誌檔案匯出到桌面的問題
* &lbrack;UI&rbrack;在建立時，匯出面板大小不對
* &lbrack;UI&rbrack;一鍵開啟專案
* &lbrack;UI&rbrack;正確設定最小與最大滑桿值
* &lbrack;UI&rbrack; 顯示頻道使用標籤，取代 ID。
* &lbrack;UI&rbrack;點擊材質總是會開啟或關閉調整面板
* &lbrack;UI&rbrack; 修正隱藏圖層顏色
* &lbrack;UI&rbrack;歡迎畫面按鈕的改進
* &lbrack;Layers&rbrack;減少不必要的重新計算
* &lbrack;Layers&rbrack;使用 Clone Patch 時當機
* &lbrack;Layers&rbrack;選擇影像匯入圖層不再觸發計算
* &lbrack;Layers&rbrack;Clone Patch 與 Content Aware Fill 層在選擇時不再重新計算
* &lbrack;Channel settings&rbrack;啟用或停用使用會觸發渲染
* &lbrack;Resources&rbrack; 防止在函式庫中大量點擊堆疊時凍結
* &lbrack;Resources&rbrack;重新加入先前新增的連結資料夾時效能下降
* &lbrack;Resources&rbrack;修正了嘗試開啟已刪除的 .sbsar 檔案時的當機
* &lbrack;性能&rbrack;避免裝載材料以取得其參數
* &lbrack;Performance&rbrack;僅在專案或作者資料中使用時備份資產
* &lbrack;出口&rbrack;出口佇列中的固定材料有時會跳過或以錯誤參數匯出
* &lbrack;2D 視圖&rbrack;恢復平移與縮放
* &lbrack;內容&rbrack;Parquet 圖案會考慮環境遮蔽通道
* &lbrack;Content&rbrack;Paint - 啟用自訂遮罩時顯示遮罩輸入
* &lbrack;Content&rbrack; Stonewall Pattern - 移除法線貼圖中可能出現的條紋效果
* &lbrack;Content&rbrack; 高度調變 - 在 2D 視圖中正確呈現雙基底顏色條目

**已知問題：**

* 內容感知填充濾鏡在高解析度下速度較慢
* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 在滑桿中輸入特定evalue時，可以忽略Coma或點

## 版本 1

### 1.1.4 （2019.1.4） Sesame

*（發行日期：2020年1月30日）*

**補充：**

* &lbrack;Resources&rbrack;清除資源資料夾時的確認提示

**修正：**

* &lbrack;Layers&rbrack; 將圖層移動到上下或上方兩層以上
* &lbrack;建立&rbrack;配置足夠的 VRAM 預算以維持良好效能

**已知問題：**

* 大量資源匯入會大幅拖慢物質煉金術師的進度
* 內容感知填充濾鏡在高解析度下速度較慢
* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 在滑桿中輸入特定evalue時，可以忽略Coma或點
* 在 MacOS 上，法線到高度過濾器可能會當機

### 1.1.3 （2019.1.3） Sesame

*（發行日期：2020年1月28日）*

**補充：**

* &lbrack;工作流程&rbrack;支援多個工作流程
* &lbrack;工作流程&rbrack;支援PBR鏡面光澤工作流程
* &lbrack;工作流程&rbrack;新通道設定面板
* &lbrack;工作流程&rbrack;專案建立時的工作流程選擇
* &lbrack;通道設定&rbrack;啟動/停用特定通道計算
* &lbrack;頻道設定&rbrack;顯示目前素材中可用的自訂頻道列表
* &lbrack;頻道設定&rbrack;必要時自動計算自訂頻道
* &lbrack;通道設定&rbrack;自訂通道的強制/區塊計算
* &lbrack;Layers&rbrack;Atlas Scatter and Splatter 濾波器中材質輸入佔位符的新使用者介面
* &lbrack;Layers&rbrack;影像輸入參數可由底層層輸入
* &lbrack;Layers&rbrack; 當部分圖層過期時會顯示通知
* &lbrack;Layers&rbrack;可透過通知更新至最新版本的舊圖層
* &lbrack;Project&rbrack;專案建立時新增的元資料欄位
* &lbrack;Inspire&rbrack;生成的變體是針對特定專案的
* &lbrack;2D View&rbrack;在圖層輸入、圖層輸出與材質輸出之間切換
* &lbrack;歡迎畫面&rbrack;新增匯入專案（.alch）選項
* &lbrack;偏好設定&rbrack;新增設定快取位置與分析隱私設定的偏好設定視窗
* &lbrack;UI&rbrack; 新 UI 按鈕
* &lbrack;效能&rbrack;整體平行化系統的改進
* &lbrack;性能&rbrack;材料數量的優化計算
* &lbrack;引擎與物質引擎更新
* &lbrack;Framework&rbrack;升級至Qt 5.13
* &lbrack;MacOS&rbrack;macOS Catalina 支援的全球改進
* &lbrack;Content&rbrack; 調整濾波器 - 正常強度與反轉參數

**修正：**

* &lbrack;Layers&rbrack;刪除圖層時取消影像輸入參數
* &lbrack;Layers&rbrack; 修正新增克隆補丁層時的崩潰
* &lbrack;Layers&rbrack; 修正混合圖層時的一些崩潰，堆疊其他圖層的材質，堆疊材質
* &lbrack;出口&rbrack;出口通道選擇現已受到尊重
* &lbrack;Resources&rbrack;在資源面板中導航時不會當機
* &lbrack;Resources&rbrack; 修正匯入損壞 Substance 檔案時的當機
* &lbrack;Resources&rbrack;在載入大型資料夾時減少當機次數
* &lbrack;縮圖&rbrack;縮圖計算不會凍結介面
* &lbrack;影像匯入&rbrack;支援整個應用程式的影像類型統一化
* &lbrack;Preset&rbrack;從 SBSAR 建立預設時，請儲存描述
* &lbrack;Inspire&rbrack; 修正圖片拖放問題
* &lbrack;Application&rbrack; 修正在出口時當機
* &lbrack;Application&rbrack;修正在導出材料時出口當機
* &lbrack;UI&rbrack;修正與改進
* &lbrack;UI&rbrack; 將臨時資產重新命名為「未儲存素材」
* &lbrack;內容&rbrack;全域更新與所有過濾器清潔

**已知問題：**

* 大量資源匯入會大幅拖慢物質煉金術師的進度
* 內容感知填充濾鏡在高解析度下速度較慢
* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 在滑桿中輸入特定evalue時，可以忽略Coma或點
* 在 MacOS 上，法線到高度過濾器可能會當機

### 1.1.2 （2019.1.2） 芝麻

*（發行日期：2019年12月11日）*

**補充：**

* &lbrack;Layers&rbrack;儲存與另存為選項可透過圖層堆疊工具列的介面存取
* &lbrack;Resources&rbrack;資源面板中更清晰的麵包屑，方便瀏覽資料夾
* &lbrack;Resources&rbrack; 保持返回鍵以存取所有上方資料夾
* &lbrack;Resources&rbrack; 新增匯入材料的重載選項，以更新至最新版本
* &lbrack;Layers&rbrack; 可在 Image 匯入圖層中更改影像
* &lbrack;Layers&rbrack;可將影像定義為通道（底色、法線、高度,...） 在 Image 匯入圖層
* &lbrack;內容&rbrack;新圖譜散射濾波器，用以散布來自Substance Source的新圖譜元素
* &lbrack;內容與rbrack;新油畫效果濾鏡
* &lbrack;內容&rbrack;新通道生成濾鏡，可從基底色彩與法線貼圖產生高度、環境遮蔽與粗糙度

**修正：**

* &lbrack;UI&rbrack; 在圖層堆疊工具列中重新啟動工具提示
* &lbrack;UI&rbrack; 修正在滑桿值中輸入兩個小數點時的問題
* &lbrack;Performance&rbrack; 修正快速切換材料時的崩潰
* &lbrack;Export&rbrack;在出口結束前切換到其他材料後，不再當機
* &lbrack;Resources&rbrack;右鍵點擊素材時，右鍵選單會顯示在材質上方
* &lbrack;Layers&rbrack;當圖層堆疊為空時，「點此」連結仍然有效
* &lbrack;Presets&rbrack;當材質在 Alchemist 製作時，請移除調整面板中的儲存按鈕
* &lbrack;調整&rbrack;當該材料在煉金術師中創造時會顯示資訊訊息
* &lbrack;Viewport&rbrack;Specular Level 貼圖的預設值已校正為 0.04
* &lbrack;檔案選單&rbrack;修正並重新命名「儲存」與「儲存為選項」
* &lbrack;Engine&rbrack;更新 Substance 引擎版本，以避免匯入過程中部分 SBSAR 檔案當機。
* &lbrack;內容&rbrack;平鋪濾波器正在環境遮蔽通道上工作
* &lbrack;內容&rbrack;裁切濾波器正在環境遮蔽通道上工作
* &lbrack;Content&rbrack; 水過濾器修改 增益高度映射
* &lbrack;內容&rbrack;在不透明度混合模式下，正確平鋪頂材質
* &lbrack;內容&rbrack;頂部材質的高度在不透明度混合模式下會被保留
* &lbrack;Content&rbrack;可在穿孔濾鏡中新增自訂遮罩、自訂圖案或比例貼圖
* &lbrack;Content&rbrack;高度調變濾波器強制以16位元進行高度與法線映射
* &lbrack;內容&rbrack;調整濾波器強制高度與法線貼圖（16位元）

**已知問題：**

* 大量資源匯入會大幅拖慢物質煉金術師的進度
* 內容感知填充濾鏡在高解析度下速度較慢
* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 在滑桿中輸入特定evalue時，可以忽略Coma或點
* 在 MacOS 上，法線到高度過濾器可能會當機

### 1.1.1 （2019.1.1） Sesame

*（發行日期：2019年11月26日）*

**補充：**

* &lbrack;Blend&rbrack;新不透明度混合模式
* &lbrack;引擎與新物質引擎版本

**修正：**

* &lbrack;Layers&rbrack; 在刪除仍在計算的層時修復崩潰
* &lbrack;Layers&rbrack; 修正移除底層時的崩潰
* &lbrack;Layers&rbrack; 修正材質名稱包含特殊字元時的崩潰
* &lbrack;Layers&rbrack; 停止計算所有使用小工具的過濾器
* &lbrack;Layers&rbrack;使用克隆補丁與內容感知填充過濾器時避免當機
* &lbrack;Layers&rbrack; 修正拖放濾鏡在 splatter 輸入槽時當機的問題
* &lbrack;Resources&rbrack; 修正在 Substance Alchemist 連結本地資料夾或匯入資源時當機的問題
* &lbrack;Collection&rbrack; 修正快速切換材料時的崩潰
* &lbrack;UI&rbrack; 修正當值為空或無效時，視口上的位移滑桿當機
* &lbrack;Inspire&rbrack;修正存取 Inspire 分頁時的當機
* &lbrack;Inspire&rbrack;修正剛儲存的圖層堆疊材質靈感時當機
* &lbrack;性能&rbrack;重物質材料與過濾器（平鋪）計算速度更快
* &lbrack;Help&rbrack; 修正匯出日誌檔案
* &lbrack;內容&rbrack;隨機化過濾器適用於所有頻道
* &lbrack;內容&rbrack;多角度工作流程會考慮所有掃描
* &lbrack;內容&rbrack;AO 混合正確混合
* &lbrack;Content&rbrack;曲率混合正確混合
* &lbrack;內容&rbrack; 色彩識別 混合正確混合
* &lbrack;內容&rbrack;自訂遮罩混合正確混合
* &lbrack;內容&rbrack;修正 調整濾波器以調整粗糙度
* &lbrack;內容&rbrack;修正自訂普通頻道上傳的基礎材質過濾器
* &lbrack;Content&rbrack; 修正壓紋濾波器的自訂匯入模式

**已知問題：**

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 在滑桿中輸入特定值時，可以忽略逗點或點
* 在 MacOS 上，法線到高度過濾器可能會當機

### 1.1.0 （2019.1.0） Sesame

*（發行日期：2019年11月4日）*

**補充：**

* &lbrack;專案&rbrack;專案的建立
* &lbrack;Project&rbrack;引入包含專案資料的 .alch 檔案格式
* &lbrack;Project&rbrack; 匯出包含集合及其資料的 .alch 專案
* &lbrack;Project&rbrack; 匯入 .alch 專案
* &lbrack;專案&rbrack;開放近期專案
* &lbrack;歡迎螢幕;啟動時會顯示歡迎螢幕
* &lbrack;歡迎畫面&rbrack;從歡迎畫面創建專案
* &lbrack;歡迎畫面;在歡迎畫面中查看你所有專案的清單
* &lbrack;歡迎螢幕&rbrack;快速連結可存取文件、關於視窗及授權管理
* &lbrack;檔案選單&rbrack;檔案選單整合
* &lbrack;檔案選單&rbrack;從檔案標籤和圖層堆疊的儲存中存取專案指令
* &lbrack;檔案選單&rbrack;從編輯標籤存取復原與重做指令
* &lbrack;檔案選單&rbrack;先前的說明選單移到了說明標籤下的檔案選單中
* &lbrack;Layers&rbrack;新的層堆疊架構
* &lbrack;Layers&rbrack;圖層堆疊的新使用者介面
* &lbrack;Layers&rbrack;直接在工具列選擇混合模式
* &lbrack;Layers&rbrack;分別存取混合參數與材質參數
* &lbrack;Layers&rbrack; 直接在 Splatter 濾波器的專用輸入中加入材質，並置於圖層堆疊中
* &lbrack;Layers&rbrack;直接在影像匯入圖層中更改掃描順序
* &lbrack;視窗&rbrack;攝影機視野控制
* &lbrack;視窗&rbrack;可在正交相機與透視相機間切換
* &lbrack;Viewport&rbrack;顯示每個通道的解析度與位元深度資訊
* &lbrack;資源&rbrack;基礎材料預設會被開啟
* &lbrack;Cache&rbrack; 找到你的縮圖快取資料夾
* &lbrack;Cache&rbrack; 找到你的渲染快取資料夾
* &lbrack;Panels&rbrack;材料設定面板暫時隱藏
* &lbrack;工作流程&rbrack;視角/光澤暫時停用
* &lbrack;MacOS&rbrack; Catalina OS 版本公證
* &lbrack;內容&rbrack;新版 Delighter 濾波器
* &lbrack;Content&rbrack; 新的影像內容感知填充過濾器
* &lbrack;內容&rbrack;新素材內容感知填充過濾器
* &lbrack;Content&rbrack; 轉換過濾器有安全的轉換選項

**修正：**

* 所有先前與 Create 相關的錯誤，隨著新 UI 和架構版本，今天都失效了
* 工具提示不會隱藏頂欄（3D、2D、2D/3D）中的圖示。
* &lbrack;Content&rbrack;濺射濾波器可接受帶有完整高度圖的 Atlas
* &lbrack;內容&rbrack;轉換濾鏡適用於影像（scan1， scan2,...）

**已知問題：**

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 在滑桿中輸入特定值時，可以忽略逗點或點
* 在 MacOS 上，法線到高度過濾器可能會當機

## 測試版

### 0.8.1-beta 藜麥

*（發行日期：2019年8月19日）*

**補充：**

* 能夠從發射器將物質源資產傳送給物質煉金術師計畫

**修正：**

* &lbrack;Create&rbrack;有些過濾器在快速存取器中列出，但在過濾器面板中卻沒有
* &lbrack;MacOS&rbrack;修正了退出時的一些當機問題

**已知問題：**

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 不建議快速切換 Delighter 舞台
* Tif 影像在 Image 匯入圖層的屬性面板中沒有顯示
* 在滑桿中輸入特定值時，可以忽略逗點或點
* 在 MacOS 上，法線到高度過濾器可能會當機
* 在 MacOS 上退出時仍可能隨機當機

### 0.8.0-beta 藜麥

*（發行日期：2019年8月8日）*

**補充：**

* &lbrack;Resources&rbrack;將你的素材資料夾連接到並鏡像到本地磁碟
* &lbrack;Resources&rbrack;瀏覽你的材料資料夾及其子資料夾
* &lbrack;資源&rbrack;在另一個視窗中移除你的材料資源面板，即可全螢幕查看資源
* &lbrack;Resources&rbrack;新增資源面板配置以支援資料夾及子資料夾導航
* &lbrack;Resources&rbrack;用麵包屑來瀏覽你的資料夾
* &lbrack;Resources&rbrack;強制同步你的本地資料夾，透過點擊即可開啟的同步選項
* &lbrack;Resources&rbrack;用「斷開」選項，透過點擊鍵斷開你的本地資料夾
* &lbrack;Manage&rbrack; 顯示 Substance 檔案的嵌入標籤
* &lbrack;管理&rbrack;新增、編輯及刪除你素材的標籤
* &lbrack;管理&rbrack;評分你的資料
* &lbrack;Layers&rbrack; 支援全景輸出
* &lbrack;Layers&rbrack;你可以在 Image 匯入圖層中刪除 Image 輸入
* &lbrack;Layers&rbrack; 自動選擇新增圖層
* &lbrack;Layers&rbrack;在層刪除後自動選擇下方的圖層
* &lbrack;UX&rbrack;切換到其他實驗室時，保持左側面板的可見性
* &lbrack;UX&rbrack;在匯入非空圖層堆疊的圖片時，請勿建立基底圖層或開啟材質工作流程彈窗
* &lbrack;UI&rbrack;新文字欄位風格
* &lbrack;UI&rbrack;新搜尋框風格
* &lbrack;UI&rbrack;新面板標頭風格
* &lbrack;UI&rbrack;新的忙碌指示器風格
* &lbrack;UI&rbrack;新圖層堆疊背景風格
* &lbrack;UI&rbrack; 使用 Adobe Clean 字型
* &lbrack;UI&rbrack; 移除滴管圖示的顏色輸入參數佔位符
* &lbrack;Performance&rbrack;忙碌指標優化
* &lbrack;Content&rbrack;新模式產生器濾波器
* &lbrack;內容&rbrack;新模糊濾鏡

**修正：**

* &lbrack;Inspire&rbrack;修正使用超過10種顏色時的崩潰
* &lbrack;2D 視圖&rbrack; 修正 2D 視圖頻道列表中的滾動條
* &lbrack;Viewer&rbrack; 修正匯入非 2 次方環境貼圖時的崩潰
* &lbrack;Content&rbrack; 修正 PNG 匯入以支援壓紋與穿孔濾鏡的自訂圖案
* &lbrack;Export&rbrack;修正正常，且每個通道匯出高度為 16 位元
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

### 0.7.0-beta 佩珀

*（發行日期：2019年6月13日）*

**補充：**

* &lbrack;Filters&rbrack;按空白鍵快速存取你的過濾器
* &lbrack;Filters&rbrack;全新專用面板，用來管理、瀏覽及匯入你的濾鏡
* &lbrack;Metadata&rbrack; 右鍵點擊素材以查看其元資料
* &lbrack;Metadata&rbrack;右鍵點擊素材以查看其在磁碟中的位置
* &lbrack;滑桿&rbrack;按 Ctrl 鍵將滑鼠移到滑桿時進行動畫
* &lbrack;滑桿&rbrack;按 P 停止並重新啟動滑桿動畫
* &lbrack;出口&rbrack;SBSAR出口遵循物質來源指引
* &lbrack;License&rbrack;使用環境變數啟動物質煉金術師
* &lbrack;UX&rbrack;檔案對話框會記住最後選擇的檔案路徑
* &lbrack;UX&rbrack;資料夾對話框會記住最後選擇的資料夾路徑
* &lbrack;UI&rbrack; 更新資源面板 UI
* &lbrack;UI&rbrack; 更新搜尋欄 UI
* &lbrack;UI&rbrack; 建立新素材圖示已更新
* &lbrack;Help&rbrack;網址已更新至 substance3d.com 網域
* &lbrack;Mesh&rbrack;現已提供布網
* &lbrack;內容物&rbrack;新腐蝕過濾器
* &lbrack;Content&rbrack;新型氧化過濾器
* &lbrack;內容&rbrack;新苔蘚過濾器
* &lbrack;內容與brack;新塵埃過濾器
* &lbrack;內容&rbrack;新磚牆模式濾波器
* &lbrack;內容&rbrack;新石牆型過濾器
* &lbrack;內容物&rbrack;新木質表面過濾器
* &lbrack;內容物&rbrack;新金屬表面處理過濾器
* &lbrack;內容&rbrack;新雪過濾器
* &lbrack;Content&rbrack;新隨機器過濾器
* &lbrack;Content&rbrack;你現在可以直接在 Base Material 濾鏡中匯入你的材質

**修正：**

* 修復儲存層堆疊時的崩潰
* 可以在環境旋轉滑桿中加入高於 1 的值
* 當混合圖層在不同素材圖層之間來回轉換時，不要失去混合參數
* 在產生同一層堆疊多次變體時，修正重複問題
* 重新開啟材料時，煉金術士會記住你調整過的滑桿範圍（最小值和最大值）

**已知問題：**

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 不建議快速切換 Delighter 舞台
* 自訂環境匯入可能會變成黑色
* Tif 影像在 Image 匯入圖層的屬性面板中沒有顯示
* 在滑桿中輸入特定值時，可以忽略逗點或點
* 在 MacOS 上，法線到高度過濾器可能會當機

### 0.6.1-beta 橘色

*（發行日期：2019年6月13日）*

**補充：**

* &lbrack;引擎&rbrack;物質引擎更新以相容最新 Substance Designer 版本
* &lbrack;License&rbrack;首次安裝時更新授權資料夾
* &lbrack;Layers&rbrack;隨時在你的圖層堆疊中重新載入以更新你的自訂過濾器

**修正：**

* &lbrack;資料相容性&rbrack;防止升級時資料損壞的修正

**已知問題：**

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 不建議快速切換 Delighter 舞台
* 自訂環境匯入可能會變成黑色
* Tif 影像在 Image 匯入圖層的屬性面板中沒有顯示
* 在滑桿中輸入特定值時，可以忽略逗點或點

### 0.6.0-beta 橘色

*（發行日期：2019年4月18日）*

**補充：**

* &lbrack;Metadata&rbrack;在專用分頁中查看並填寫材料的元資料
* &lbrack;Collection&rbrack;直接從搜尋結果建立集合
* &lbrack;Media Publishing&rbrack;匯出一個收藏的板子
* &lbrack;UX&rbrack;按 Ctrl+Z 來還原修改或匯入圖片
* &lbrack;UX&rbrack;按 Ctrl+Shift+Z 重新調整或匯入圖片
* &lbrack;UI&rbrack;新圖示與新風格
* &lbrack;Performance&rbrack;新增 Session 管理器，以更好地處理分頁切換
* &lbrack;Performance&rbrack;影像匯入層的開啟速度加快
* &lbrack;內容&rbrack;新金屬通用材料
* &lbrack;內容&rbrack;新Rust材料
* &lbrack;內容&rbrack;新石通用材料
* &lbrack;內容&rbrack;浮雕濾波器更新
* &lbrack;Content&rbrack; 刺繡濾鏡更新
* &lbrack;內容&rbrack; 顏料濾鏡更新
* &lbrack;內容&rbrack;Delighter 濾波器更新

**修正：**

* &lbrack;Content&rbrack;水過濾器在 Specular/Glossiness 工作流程中運作
* 修正啟動彈窗中的灰階無線電按鈕
* 接受包含逗號字元的檔案
* 修正彈出視窗中小字型問題
* 修正因部分 NVIDIA 顯卡 FXAA 參數衝突而導致透明度介面問題
* 在滑桿中entenping值後，移除欄位的焦點
* 將最少的 VRAM 分配給 Delighter，以減少當機
* 修正調整應用程式視窗大小時的視窗凍結問題
* 在評估時刪除圖層堆疊時，已修正當機

**已知問題：**

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* 不建議快速切換 Delighter 舞台
* 自訂環境匯入可能會變成黑色
* Tif 影像在 Image 匯入圖層的屬性面板中沒有顯示
* 在滑桿中輸入特定值時，可以忽略逗點或點

### 0.5.4-beta Nacho

*（發行日期：2019年3月26日）*

**修正：**

* &lbrack;Stack&rbrack;移除濺射層時的崩潰
* &lbrack;Data&rbrack;當應用程式當機時，資產資料庫會損壞
* &lbrack;Data&rbrack;當資產資料庫損壞時，物質煉金術師無法啟動
* 匯入物質材料時隨機當機

**已知問題：**

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* Delighter 階段的快速可見度切換會影響效能
* 自訂環境匯入可能會變成黑色
* Tif 影像在 Image 匯入圖層的屬性面板中沒有顯示
* 在滑桿中輸入特定值時，可以忽略逗點或點
* 預設儲存的收藏可以是空的

### 0.5.3-beta Nacho

*（發行日期：2019年3月19日）*

**補充：**

* 在資源面板中依材料名稱搜尋
* &lbrack;UI&rbrack; Clone 工具 新 UI 附有筆刷大小視覺化功能
* &lbrack;UI&rbrack; 選擇並刪除隱藏階段
* &lbrack;UI&rbrack;新文字欄位介面
* &lbrack;幫助&rbrack;存取物質來源、物質分享及物質學院網站
* &lbrack;內容&rbrack;新增預設材料，包含產生器和地圖集
* &lbrack;內容&rbrack; 點陣圖至材質更新
* &lbrack;內容&rbrack;泥土更新
* &lbrack;內容&rbrack;Rust更新
* &lbrack;內容&rbrack;新壓紋濾波器
* &lbrack;內容&rbrack;新刺繡過濾器
* &lbrack;內容&rbrack;新侵蝕過濾器
* &lbrack;內容與rbrack;新碎石發電機
* &lbrack;內容&rbrack;新顏料濾鏡
* &lbrack;內容&rbrack;新款Parquet Pattern濾波器
* &lbrack;內容&rbrack;新路面圖案過濾器
* &lbrack;Content&rbrack;新穿孔濾波器
* &lbrack;內容&rbrack;新濺射濾鏡
* &lbrack;內容&rbrack;新紡織品磨損過濾器
* &lbrack;Content&rbrack;新轉換濾波器

**修正：**

* &lbrack;Viewport&rbrack; 球體網格，X上鋪設 x2 平鋪
* &lbrack;Viewport&rbrack;載入自家環境時崩潰
* &lbrack;Viewport&rbrack;環境地圖現在也使用曝光值
* &lbrack;Viewport&rbrack;F快捷鍵不會重置攝影機角度
* &lbrack;出口&rbrack;SBS出口與最新Substance Designer合作 2018.3.3
* &lbrack;出口&rbrack;SBSAR出口遵循與物質來源材料相同的指導方針
* &lbrack;UI&rbrack;滾動條可以拖曳
* 支援在資料夾與檔案路徑上使用特殊字元
* 縮圖會在你儲存素材時重新生成

**已知問題：**

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* Delighter 階段的快速可見度切換會影響效能
* 自訂環境匯入可能會變成黑色
* Tif 影像在 Image 匯入圖層的屬性面板中沒有顯示
* 在滑桿中輸入特定值時，可以忽略逗點或點
* 預設儲存的收藏可以是空的

### 0.5.2-beta Nacho

*（發行日期：2019年3月7日）*

**補充：**

* 高規格GPU的偵測與使用

**修正：**

* 旋轉參數有一個真正的滑桿小工具
* 修正拖放材質時藍色色線的可見性
* 當材質掉落到第一層以下時，修正材質混合問題
* 只有在沒有設定自訂影像路徑時才接入影像輸入

**已知問題：**

* 檔案路徑中的特殊字元會阻止儲存素材
* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* Delighter 階段的快速可見度切換會影響效能
* 載入自己環境時會當機

### 0.5.1-beta Nacho

*（發行日期：2019年3月4日）*

**修正：**

* 修正當機報告、錯誤回報與授權彈窗

**已知問題：**

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* Delighter 階段的快速可見度切換會影響效能
* 載入自己環境時會當機

### 0.5.0-beta Nacho

*（發行日期：2019年2月28日）*

**補充：**

* &lbrack;層疊疊&rbrack;層重排序
* &lbrack;Layer stack&rbrack; 刪除隱藏圖層
* &lbrack;疊加 stack&rbrack;直接匯入你選擇的位置的材質
* &lbrack;Layer stack&rbrack;材料輸入作為新的濾波器參數類型
* &lbrack;性能&rbrack;Substance Engine 預算是動態的，以提升效能
* &lbrack;效能&rbrack;更好的 OpenGL 效能，特別是在 MacOS 上
* &lbrack;Data&rbrack;新版本發布後更快的資料升級
* &lbrack;內容&rbrack;AI Delighter 可在 Windows 7 和 Windows 8 上取得
* &lbrack;內容&rbrack;RTX GPU 上的 AI Delighter

**修正：**

* 修復關閉應用程式時可能發生的當機問題
* 匯出彈出視窗在匯出大型收藏時會開啟得更快

**已知問題：**

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* Delighter 階段的快速可見度切換會影響效能
* 載入自己環境時會當機

### 0.4.0-beta 瑪芬

*（發行日期：2019年1月17日）*

**補充：**

* &lbrack;Export&rbrack;物質檔案庫（sbsar） 匯出您的收藏
* &lbrack;Export&rbrack;Substance 檔案（sbs）匯出你的收藏
* &lbrack;Export&rbrack;匯出佇列可見於匯出面板
* &lbrack;Export&rbrack;出口前命名你的收藏或資料
* &lbrack;Data&rbrack; 按 Ctrl+Shift+S 儲存為你的素材
* &lbrack;Data&rbrack; 按 Ctrl+S 儲存你的素材
* &lbrack;資料與資料在各版本間相容
* &lbrack;Data&rbrack;更新你的材質層堆疊並使用最新的過濾器
* &lbrack;Data&rbrack; 匯入自訂濾波器的熱重載
* &lbrack;UI&rbrack;在視窗運算時的視覺回饋
* &lbrack;UI&rbrack;新按鈕樣式
* &lbrack;UI&rbrack; 儲存彈出視窗顯示活躍收藏名稱
* &lbrack;UI&rbrack; 修改影像的原始影像 匯入圖層
* &lbrack;內容&rbrack;現已支援自訂使用方式
* &lbrack;Content&rbrack;支援更多影像格式於影像輸入參數中
* &lbrack;Content&rbrack;新平鋪過濾器，名為 Make It Tile Advanced
* &lbrack;內容&rbrack;水過濾器更新

**修正：**

* Bitmap to Material 處理 Specular/Glossiness 的工作流程

**已知問題：**

* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* Delighter 不支援 RTX 顯示卡
* Delighter 階段的快速可見度切換會影響效能

### 0.3.1-beta 千層麵

*（發行日期：2018年12月17日）*

**修正：**

* 產生一個色彩變化，包含 10 個顏色擷取的崩潰
* 用儲存的圖層產生顏色變化，堆疊會崩潰
* 物質煉金術師版本更新彈窗上有錯誤連結

**已知問題：**

* 點陣圖轉材質無法處理高光/粗糙度的工作流程
* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* Delighter 階段的快速可見度切換會影響效能

### 0.3.0-beta 千層麵

*（發行日期：2018年12月12日）*

**補充：**

* &lbrack;出口&rbrack;新出口彈窗
* &lbrack;Export&rbrack; 匯出整個收藏
* &lbrack;Export&rbrack; 以你選擇的格式匯出點陣圖
* &lbrack;Export&rbrack; 以你選擇的解析度匯出點陣圖
* &lbrack;Export&rbrack; 只匯出你選擇的頻道
* &lbrack;Export&rbrack; 預覽你的出口估計大小
* &lbrack;匯出&rbrack;匯出前預覽磁碟可用大小
* &lbrack;UX&rbrack;集合上的操作可透過右鍵點擊存取
* &lbrack;UX&rbrack;允許在 Inspire 中重置圖片或資產
* &lbrack;UX&rbrack;物質煉金術師被最大化推出
* &lbrack;Assets&rbrack;新的方式儲存素材，以保持它們在下一版本中持續存在
* &lbrack;Help&rbrack;可透過說明選單存取線上文件
* &lbrack;性能&rbrack;用物質煉金術師製作的複雜材料，顏色變化更快
* &lbrack;Performance&rbrack; 減少切換實驗室時的記憶體洩漏
* &lbrack;Content&rbrack;用來診斷材料的物理尺寸
* &lbrack;內容&rbrack;更新義大利威尼斯馬賽克瓷磚材料
* &lbrack;內容&rbrack;更新苔蘚濺血事件

**修正：**

* 儲存材料時不再使用預設名稱
* 儲存材料並重新開啟物質煉金術師後，過濾器參數會消失
* &lbrack;內容&rbrack;從下方和頂部修正AO與曲率混合邏輯

**已知問題：**

* 用舊版本製作的教材不會在新版本中提供。
* 點陣圖轉材質無法處理高光/粗糙度的工作流程
* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* Delighter 階段的快速可見度切換會影響效能

### 0.2.0-beta Kiwi

*（發行日期：2018年11月9日）*

**補充：**

* 檢視器設定會從一個會話儲存到另一個
* 材質設定會從一個會話儲存到另一個
* 快速載入屬性面板
* &lbrack;Log&rbrack; 透過說明選單匯出日誌檔案
* &lbrack;UI&rbrack;新滑桿風格
* &lbrack;UI&rbrack;預設與調整面板已合併
* &lbrack;UI&rbrack;新縮圖風格
* 位移、平鋪與陰影設定可直接在視窗中存取
* &lbrack;內容&rbrack;新預設材料
* &lbrack;內容&rbrack;苔蘚濺射更新
* &lbrack;Framework&rbrack;更新物質引擎框架

**修正：**

* 切換實驗室會刪除你的層堆疊是固定的
* 視窗中顯示的載入時間值是正確的
* Material 工作流程預設通道已正確初始化
* 停用自訂網格匯入
* 位圖匯出
* &lbrack;MacOS&rbrack;關閉物質煉金術士可能需要「強制退出」

**已知問題：**

* 用舊版本製作的教材不會在新版本中提供。
* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* Delighter 階段的快速可見度切換會影響效能

### 0.1.1-beta Jam

*（發行日期：2018年10月24日）*

**補充：**

* BaseColor Delighter 現已上市
* 透過說明選單存取物質鍊金術士相關資訊
* 當《物質鍊金術師》新版本推出時，請收到通知
* 這個控制台在 Windows 上已經看不到了
* 新縮圖風格
* &lbrack;MacOS&rbrack;物質煉金術師可全螢幕設定
* &lbrack;Filter&rbrack; 匯入自訂遮罩以管理兩個材質間的混合
* &lbrack;過濾器&rbrack;控制苔蘚秤
* &lbrack;Filter&rbrack;克隆補丁更新

**修正：**

* 在參數列表的輸入中新增影像，更新輸出
* 匯入自訂濾鏡不會新增黑色環境遮蔽和黑色不透明度

**已知問題：**

* 用舊版本製作的教材不會在新版本中提供。
* &lbrack;MacOS&rbrack;關閉物質煉金術士可能需要「強制退出」
* 不建議在同一材料中使用多個 Delighters（甜點）
* Delighter 在較舊的 NVIDIA 驅動程式（低於 400.x）時會當機
* Delighter 階段的快速可見度切換會影響效能
* 材料匯出可能會當機

### 0.1.0-beta 冰淇淋

*（發行日期：2018年10月17日）*

**補充：**

* 材質混合，包含四種混合類型（高度混合、樣本混合、曲率混合、AO 混合）
* 引入快取機制以優化層堆疊重算
* 如果 Inspire 的材質出現在視窗中，會自動選擇
* 一般格式集中在材質設定面板中
* 裁切與平鋪小工具控制項（-90xB0，+90xB0，請將方形,...） 清潔
* 新雪過濾器

**修正：**

* 面板介面清理
* 視窗在調整視窗和面板大小時閃爍
* 儲存時圖層堆疊不會重新計算
* 介面中的資產命名使用標籤而非圖形名稱

**已知問題：**

* 透過快速切換圖層可見性來拉伸 Liure（拉長 liure）
* 對焦重置 攝影機角度
