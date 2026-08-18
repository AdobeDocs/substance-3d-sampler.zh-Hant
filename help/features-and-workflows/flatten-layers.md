---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/features-and-workflows/flatten-layers.html"
breadcrumb-title: ''
description: 學習如何在 Substance 3D Sampler 中將圖層壓平，以提升效能並簡化圖層堆疊，同時了解其影響。
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 平整層
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---


# 平整層

平整圖層是提升效能並簡化圖層堆疊的有效方法，但同時也要注意平整圖層對專案的影響。

## 「平整圖層」按鈕是做什麼的？

扁平圖層會將目前選取的圖層下方的所有圖層合併成單一圖層。 所產生的扁平圖層外觀與原始圖層相同，但你無法再對原始圖層進行調整。

### 為什麼要壓平層次？

每當你在圖層堆疊中更改圖層時，Sampler 需要重新計算該圖層及其上方所有圖層的輸出。 每多一層需要計算，就代表更多的處理時間和記憶體使用。 將多層壓平化可以減少處理這些層所需的時間和記憶體。 例如，取樣器不需要重新計算 10 層，只需處理一層。

此外，平整圖層會讓圖層堆疊更簡單，也更容易導航與理解。

### 什麼時候不該把層壓平？

任何被壓扁的圖層都無法在圖層堆疊中單獨存取，因此你無法更改壓平結果中的參數。 因此，只有當你不再需要修改圖層結果時，才應該進行壓平。

## 扁平化層參數

雖然原始圖層的參數會遺失，但 Flattened 圖層有自己的參數，你可以調整以控制每個產生的通道的使用方式。

對於每個頻道，你可以：

* <b>輸出使用</b>：更改輸出所使用的頻道。 當你平整圖層時，會為每個通道建立並命名一個 TIFF，並自動分配給該通道。
* <b>來自 alpha 通道</b>的不透明度：切換不透明度是否基於 Alpha 通道的結果。
* <b>移除</b>：移除此層的通道。 這對於不包含有用資訊的頻道非常有用。 例如，移除全白不透明度通道是個好主意，這樣可以釋放記憶體而不影響視覺效果。
