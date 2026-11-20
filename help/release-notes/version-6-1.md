---
description: 檢視 Substance 3D Sampler 6.1 版的發行說明，了解新功能、改進與工作流程強化。
title: 版本 6.1
hold: true
source-git-commit: 99bb504f8dd5c485bf0d208a85cc3825d186c55f
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 0%
---

# 版本 6.1

**Kouign amann** （布列塔尼層層酥皮）

![替代文字](../../help/assets/Sampler_splash_large.jpg)

本次版本引入了效能模式，讓任何人都能關閉可能拖慢工作流程的設定，並自動提升穩定性，保護輕量硬體使用者的安全。

主要新功能包括：

## 效能模式

在 Sampler 中獲得更快速、更靈敏的體驗。 全新 **效能模式** 整合了所有可能拖慢工作流程的設定：解析度限制、陰影、位移品質與路徑追蹤。 關閉不需要的功能，以提升效能與反應速度。

更多資訊 [*請見此處*](https://www.adobe.com/go/substance-3d-sampler-6.1-performance-mode)

![](../assets/v6.1/6_1-Performance_Mode.png)

## 改善對最低規格機器的支援

如果你的硬體規格低於 [最低規格](../getting-started/system-requirements.md)，Sampler 現在會自動調整以維持穩定。 最有可能拖慢進度或導致當機的功能會自動關閉。

更多資訊 [*請見此處*](https://www.adobe.com/go/substance-3d-sampler-6.1-low-specs-mode)

![](../assets/v6.1/6_1-Checked.png)

## V6.1 發行說明

*（發布日期：2026年11月19日）*

## 新增

* &amp;lbrack;應用程式&amp;rbrack; 新增回報最低硬體需求警告的方式
* &amp;lbrack;Captis&amp;rbrack; 新增選項可選擇 4 或 8 種偏振角度
* &amp;lbrack;Captis&amp;rbrack; 新 Captis 快速動作
* &amp;lbrack;匯出&amp;rbrack; 正確向使用者回報匯出失敗
* &amp;lbrack;匯出&amp;rbrack; 更新 Unreal Engine 4 匯出預設（已命名為 Unreal Engine 5）
* &amp;lbrack;效能&amp;rbrack; 從檔案建立資產現在已非同步
* &amp;lbrack;效能&amp;rbrack; 將工作負載從主執行緒移至工作執行緒
* &amp;lbrack;效能&amp;rbrack; 新增效能模式
* &amp;lbrack;專案&amp;rbrack;若專案儲存失敗，提醒使用者
* &amp;lbrack;腳本&amp;rbrack;新增資產generate_thumbnail方法及資源新類型屬性
* &amp;lbrack;腳本&amp;rbrack; 從 Python 模組將 3D 檢視快照渲染到檔案
* &amp;lbrack;UI&amp;rbrack; 點擊放置區的任何位置即可開啟檔案對話框
* &amp;lbrack;UI&amp;rbrack; 左側導覽列捷徑可切換工具（均衡、裁切、平鋪、變形、修復、著色等）
* &amp;lbrack;UI&amp;rbrack; 升級 qt-spectrum 以取得最新圖示

## 已修正

* &amp;lbrack;3D 檢視&amp;rbrack; 修正即時的 UV 偏移與旋轉，移除 OpenPBR 的正常縮放
* &amp;lbrack;3D View&amp;rbrack; 透過確保在刪除視窗時不會發生舞台編輯，以防止當機
* &amp;lbrack;3D 檢視&amp;rbrack; 在變更顯示資產時正確移除位移（高度）資訊
* &amp;lbrack;3D 檢視&amp;rbrack; 刪除網格時正確更新文件
* &amp;lbrack;應用程式&amp;rbrack; 確保在計算動態篩選器除錯資訊時，表面保持活躍
* &amp;lbrack;應用程式&amp;rbrack; 修正 Scene 退出時當機
* &amp;lbrack;應用程式&amp;rbrack; 修正資產資料庫服務關閉時刪除資產時可能發生的當機問題
* &amp;lbrack;應用程式&amp;rbrack; 讓快取除錯資訊執行緒安全以防止當機
* &amp;lbrack;應用程式&amp;rbrack; 在存取節點前測試節點非空值以防止當機
* &amp;lbrack;應用程式&amp;rbrack; 防止因存取空向量的第一個元素而導致當機
* &amp;lbrack;應用程式&amp;rbrack; 防止 invalidateVisibleIfs 中的當機
* &amp;lbrack;應用程式&amp;rbrack; 在資料庫服務關閉期間防止建立資產時發生當機
* &amp;lbrack;應用程式&amp;rbrack; 防止退出時的競賽狀態
* &amp;lbrack;資產&amp;rbrack; 確保資源妥善鎖在正確的鎖後
* &amp;lbrack;Captis&amp;rbrack;手動模式下強度值的錯誤
* &amp;lbrack;Captis&amp;rbrack; 防止使用者選擇超出後端允許的區域
* &amp;lbrack;Channel Settings&amp;rbrack; ASM 中 SpecularColor 的重複出現
* &amp;lbrack;頻道設定&amp;rbrack; 修正由字串建立的使用碼 ID
* &amp;lbrack;內容&amp;rbrack; Atlas Scatter 不透明度問題
* &amp;lbrack;內容&amp;rbrack; 刺繡濾鏡缺少金屬特徵
* &amp;lbrack;內容&amp;rbrack; 修正穿孔濾鏡
* &amp;lbrack;內容&amp;rbrack; 修正類別中的樣式化篩選器及資源面板中的少量修正
* &amp;lbrack;內容&amp;rbrack; 更新填充篩選器
* &amp;lbrack;Creative Cloud&amp;rbrack; 修正 Creative Cloud 中 3D 資產的路徑
* &amp;lbrack;引擎&amp;rbrack; 在作業取消時防止存取引擎資料時發生當機
* &amp;lbrack;Export&amp;rbrack; 新增防禦程式碼以檢查結構樹狀結構是否為空
* &amp;lbrack;Export&amp;rbrack; 防禦程式碼以避免 SBS 生成時的當機
* &amp;lbrack;匯出&amp;rbrack; 啟用輸出自訂使用方式，即使引擎已知這些使用情況
* &amp;lbrack;匯出&amp;rbrack; 修正匯出預設
* &amp;lbrack;匯出&amp;rbrack;法線貼圖以美元原始格式匯出
* &amp;lbrack;匯出&amp;rbrack; 在使用預設匯出時使用輸出標籤而非使用量
* &amp;lbrack;Exposed Parameters&amp;rbrack; 修正動態濾鏡上的暴露參數
* &amp;lbrack;Exposed Parameters&amp;rbrack; 修正當名稱變更時已暴露參數更新的問題
* &amp;lbrack;篩選器&amp;rbrack; 確保動態篩選調整 識別碼在每個平台上的每次執行都完全相同
* &amp;lbrack;篩選器&amp;rbrack; 隱藏自動平鋪地圖選取中不支援的使用方式
* &amp;lbrack;圖層&amp;rbrack; 變更圖層可見性總是會重新建立結構
* &amp;lbrack;圖層&amp;rbrack; 將複製印章壓平覆蓋在某物上時當機
* &amp;lbrack;Layers&amp;rbrack; 直接在堆疊上插入產生器，現在可以正確設定調整與節點名稱
* &amp;lbrack;圖層&amp;rbrack; 插入產生器時使用填充功能，會正確顯示紋理在選取器中
* &amp;lbrack;本地化&amp;rbrack; 修正中文字元對GB18030的符合性
* &amp;lbrack;Project&amp;rbrack; 在複製印章上繪製後儲存時當機
* &amp;lbrack;專案&amp;rbrack; 確保工作階段名稱與專案名稱確實被儲存
* &amp;lbrack;Project&amp;rbrack; 在儲存樹狀結構時防止當機
* &amp;lbrack;專案&amp;rbrack; 從資料庫還原損壞專案的功能已回歸
* &amp;lbrack;快速操作&amp;rbrack; 當堆疊中沒有圖片時，顯示圖片選取彈出視窗
* &amp;lbrack;快速動作&amp;rbrack; 修正快速動作問題;取消快速動作不再會關閉快速啟動
* &amp;lbrack;快速操作&amp;rbrack;匯入材質會要求啟用某些頻道，但不應啟用
* &amp;lbrack;快速操作&amp;rbrack;防止快速動作載入失敗時當機
* &amp;lbrack;快速操作&amp;rbrack; 更新快速動作內容
* &amp;lbrack;Rendering&amp;rbrack; 修正 ASM 材質 combineNormalAndHeight
* &amp;lbrack;Rendering&amp;rbrack; 修正 Vulkan 中可顯示材質的使用方式
* &amp;lbrack;渲染&amp;rbrack; 當唯一使用輸出變更時，將樹標記為髒色
* &amp;lbrack;Rendering&amp;rbrack; 使用正確的參考結構來計算要計算的樹狀節點
* &amp;lbrack;腳本&amp;rbrack;匯出過程中若發生問題，勿卡頓
* &amp;lbrack;腳本&amp;rbrack; 確保 import_images（） 回傳匯入的圖層
* &amp;lbrack;腳本&amp;rbrack;將影像調整設定為影像資產參照失敗
* &amp;lbrack;腳本&amp;rbrack; get_filters（） 不會回傳動態篩選器
* &amp;lbrack;縮圖&amp;rbrack;修正產生縮圖時可能發生的當機問題
* &amp;lbrack;縮圖&amp;rbrack;當版面配置變更時，重新建立縮圖產生器
* &amp;lbrack;UI&amp;rbrack; 變更資產可將高度縮放設定為滑桿最大值
* &amp;lbrack;UI&amp;rbrack; 在材質中繪製會即時更新材質選擇器
* &amp;lbrack;UI&amp;rbrack; 在未最大化模式下進入全螢幕模式時，現在會填滿整個視窗
* &amp;lbrack;UI&amp;rbrack; 修正 Substance 雜誌連結失效
* &amp;lbrack;UI&amp;rbrack; 修正匯出彈出邊界
* &amp;lbrack;UI&amp;rbrack; 修正區段標題大小
* &amp;lbrack;UI&amp;rbrack; 修正字串中的錯字
* &amp;lbrack;UI&amp;rbrack; Linux 檔案對話框現在使用 GTK 外掛
* &amp;lbrack;UI&amp;rbrack; 防止顯示表情符號時當機
* &amp;lbrack;UI&amp;rbrack; 將 .ssa 檔案重新命名為「Adobe Substance 3D Sampler archive」（不含版本或 Beta 版本）
* &amp;lbrack;UI&amp;rbrack; 使用滑鼠時還原可點擊減速
* &amp;lbrack;UI&amp;rbrack; 「建立新材質」對話框中的小修正
