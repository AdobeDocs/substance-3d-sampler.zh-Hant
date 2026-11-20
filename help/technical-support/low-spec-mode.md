---
title: 低規格模式
description: 了解低規格模式，當硬體不符合最低系統需求時，Sampler 會啟用此功能。
hold: true
source-git-commit: 59761aab02bff266047813f1714e3f53ddcb805c
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%
---

# 低規格模式

![](../assets/v6.1/6_1-Checked.png)

如果您的硬體不符合 Sampler 的 [最低需求](../getting-started/system-requirements.md)，Sampler 會自動以低規格模式啟動，該模式的行為類似 [效能模式](performance-mode.md) ，且無法更改設定。

## 低規格模式限制

低規格模式會自動開啟 **效能模式** ，所有功能皆關閉，且最高預覽解析度為 2048 × 2048。

低規格模式會停用：

* **位移**
* **陰影**
* **路徑追蹤**

此外，低規格模式可防止匯出超過 2048px × 2048px。

![](../assets/low-spec-mode-export-message.png)

*此訊息會在低&#x200B;**規格模式下**&#x200B;顯示&#x200B;**於匯出視窗**&#x200B;中，以提供額外資訊。*

## 我要怎麼判斷低規格模式是否啟用？

當您啟動 Sampler 時，如果您的硬體未達到最低需求，系統會顯示視窗，指出哪些需求未達標，並提供您繼續啟動 Sampler 的選項。

下方圖片展示了一台顯示顯示記憶體少於 8GB 的機器範例。

![](../assets/low-device-specs-popup.png)

如果您選擇「 **無論如何**&#x200B;啟動」，取樣器將以 **低規格模式**&#x200B;啟動。 如果你在上方訊息中勾選了不顯示並啟動的方框，之後的啟動時仍會看到以下橫幅。

![](../assets/low-spec-mode-banner.png)

最後，在啟用低規格模式&#x200B;**時**，無法關閉效能模式或調整效能模式設定。

![](../assets/performance-mode-locked.png)
