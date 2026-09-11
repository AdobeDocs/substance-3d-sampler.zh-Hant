---
helpx_url: 'https://helpx.adobe.com/tw/substance-3d-sampler/getting-started/system-requirements.html'
breadcrumb-title: ''
description: 檢視 Substance 3D Sampler 的系統需求，確保您的硬體與軟體符合相容標準。
helpx_creative_field: ''
helpx_description: Sampler > Getting Started > System requirements
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 系統需求
user-guide-description: ''
user-guide-title: ''
source-git-commit: cd61972eaf1567863dc8c3549a1c90c84ffee825
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---


# 支援系統

以下是該應用程式所支援的硬體與系統清單：

>[!WARNING]
>
> 以下 Nvidia 驅動程式在執行 Sampler 時已知會導致不穩定：
>
> * 610.47
>
> 我們建議避免使用這些版本——理想情況下，使用較新的版本，若無更新版本，則使用先前版本。

## 窗戶

|  | 最低限度 | 推薦 | 最佳 |
| --- | --- | --- | --- |
| **作業系統** | Windows 11 64 位元版本 23H2 | Windows 11 64 位元版本 24H1 | Windows 11 64 位元版本 24H2 |
| **中央處理器** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 超級 NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080、NVIDIA Quadro RTX A4000、AMD Radeon RX 6800 XT、AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090、NVIDIA Quadro RTX 5000、Ada 世代 AMD Radeon RX 7900、XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 GB | 16 GB | 24 GB |
| **記憶體** | 16 GB | 32 GB | 64 GB |
| **儲存** | SSD 有 30 GB 可用空間 | SSD 有 50 GB 可用空間 | SSD 有 70 GB 可用空間 |

### macOS

|  | 最低限度 | 推薦 | 最佳 |
| --- | --- | --- | --- |
| **作業系統** | macOS 13 Ventura | macOS 14 Sonoma | macOS 26 Tahoe |
| **中央處理器** | 蘋果 M1 | 蘋果 M2 Pro | Apple M4 Pro |
| **GPU** | 蘋果 M1 | 蘋果 M2 Pro | Apple M4 Pro |
| **記憶體** | 24 GB | 32 GB | 64 GB |
| **儲存** | SSD 有 30 GB 可用空間 | SSD 有 50 GB 可用空間 | SSD 有 70 GB 可用空間 |

### Linux

| 企業號 | 蒸汽 |
| --- | --- |
| RHEL 8 <br>RHEL 9 | Ubuntu 22.04 |

>[!NOTE]
>
> 如果你的系統符合上述系統需求但效能仍然不穩定，Sampler 可能用錯了 GPU。
>
> 如果你使用的是 NVIDIA GPU，請 [依照本頁](../technical-support/configuration/nvidia-driver-settings.md)說明更改 GPU 取樣器所使用的 GPU 範例。

## 一般建議

* 在舒適環境下工作時，我們建議使用解析度大於1百萬畫素且寬度超過1280像素的螢幕。
* 許多 Substance 應用程式依賴 OpenSSL 1.1.1 來相容 RHEL8/9。 對於使用較新版本 OpenSSL 的系統，你需要手動提供。

## 不支援的配置

**窗戶**

* 不支援虛擬機。
* Windows Server 不支援。

**麥克**

* 僅支援官方蘋果配置。
* 目前不支援 eGPU，且可能存在穩定性問題。

**Linux**

* Linux 上的 Mesa 驅動程式不被支援。

**任何平台**

* 整合式 GPU 不支援 x86-64（Intel、AMD）CPU 的配置。
* 不支援將 Sampler 與第三方軟體結合，後者攔截 Sampler 對圖形驅動程式的呼叫。 此類軟體包括：
  * 後製注入器，例如可套用色彩分級、攝影機效果等的重著色器......
  * 螢幕上的疊加層，例如自訂準星、GPU 效能指標、影片串流的皮膚......

## 最低 GPU 驅動程式版本

以下是應用程式正常運行所需的最低 GPU 驅動版本清單。 隨著新版本發布，此列表可能會有所變動。

要下載新驅動程式請參考： [GPU 驅動程式過](https://experienceleague.adobe.com/zh-hant/docs/substance-3d-painter/using/technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers)時。

| 作業系統 | NVIDIA | AMD | 英特爾 |
| --- | --- | --- | --- |
| **窗戶** | GeForce 551.86 Quadro/RTX 538.33 | Radeon 23.8.1 Radeon Pro / FirePro 24.q2 | 31.0.1015590 |
| **Linux** | 525.116.04 或更晚， *或* 535.54.03 或更高 | Radeon 23.20 Pro 23.Q3 | 無支撐 |

>[!NOTE]
>
> 在 Mac OS **上**，GPU 驅動程式是由作業系統本身提供。更新到作業系統最新版本以存取最新的驅動程式。

## 語言

軟體介面提供以下語言：

* 英文
* 德語
* 法語
* 日本
* 韓語
* 中文
* 義大利語
* 葡萄牙語
* 西班牙語
