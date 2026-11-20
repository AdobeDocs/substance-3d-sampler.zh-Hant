---
helpx_url: 'https://helpx.adobe.com/tw/substance-3d-sampler/getting-started/system-requirements.html'
breadcrumb-title: ''
description: 請檢視 Substance 3D Sampler 的系統需求，確保您的硬體與軟體符合相容性標準。
helpx_creative_field: ''
helpx_description: Sampler > Getting Started > System requirements
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 系統需求
user-guide-description: ''
user-guide-title: ''
hold: true
source-git-commit: 8b2438eb381e35c19ab379a5fc14c962fd5b9b0a
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%
---

# 支援系統

以下是該應用程式所支援的硬體與系統清單：

>[!WARNING]
>
> 以下 Nvidia 驅動程式已知在執行 Sampler 時會導致不穩定：
>
> * 610.47
>
> 我們建議避免使用這些版本——理想情況下，使用較新的版本，或若沒有較新版本可用，則使用先前版本。

>[!NOTE]
>
> 如果您的硬體低於最低系統需求，Sampler 將自動以 [低規格模式](../technical-support/low-spec-mode.md)開啟，這會限制部分功能。

>[!TIP]
>
> 如果您想提升 Sampler 的效能，請使用 [效能模式](../technical-support/performance-mode.md) 關閉資源密集型功能。

## Windows

|  | 最低 | 推薦 | 最佳 |
| --- | --- | --- | --- |
| **作業系統** | Windows 11 64 位元版本 23H2 | Windows 11 64 位元版本 24H1 | Windows 11 64 位元版本 24H2 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080、NVIDIA Quadro RTX A4000、AMD Radeon RX 6800 XT、AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090、NVIDIA Quadro RTX 5000、Ada 世代、AMD Radeon RX 7900、XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 GB | 16 GB | 24 GB |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **儲存** | SSD 擁有 30 GB 可用空間 | SSD 配備 50 GB 可用空間 | SSD 配備 70 GB 可用空間 |

### macOS

|  | 最低 | 推薦 | 最佳 |
| --- | --- | --- | --- |
| **作業系統** | macOS 15 Sequoia | macOS 27 Golden Gate | macOS 27 Golden Gate |
| **CPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **GPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **RAM** | 24 GB | 32 GB | 64 GB |
| **儲存** | SSD 擁有 30 GB 可用空間 | SSD 配備 50 GB 可用空間 | SSD 配備 70 GB 可用空間 |

>[!WARNING]
>
> 針對以 [VFX Reference Platform](https://vfxplatform.com/) 為目標打造的管線，Substance 3D Sampler 仍可在 macOS 14 Sonoma 上安裝。 然而，Sampler 不再在低於最低系統需求的作業系統版本上進行測試，因此穩定性並不保證。 建議更新至較新的作業系統版本。

### Linux

| 企業 | 蒸汽 |
| --- | --- |
| RHEL 8 <br>RHEL 9 | Ubuntu 22.04 |

>[!NOTE]
>
> 如果您的系統符合上述系統需求但效能仍然遲緩，Sampler 可能使用了錯誤的 GPU。
>
> 如果您使用的是 NVIDIA GPU，請 [依照本頁](../technical-support/configuration/nvidia-driver-settings.md)說明更改 GPU Sampler 所使用的 GPU。

## 一般建議

* 若需在舒適環境下工作，我們建議使用解析度超過 100 萬像素且寬度超過 1280 像素的螢幕。
* 許多 Substance 應用程式依賴 OpenSSL 1.1.1 來支援 RHEL8/9。 對於使用較新版本 OpenSSL 的系統，您需要手動提供。

## 不支援的配置

**Windows**

* 不支援虛擬機。
* 不支援 Windows Server。

**Mac**

* 僅支援官方 Apple 配置。
* 目前不支援 eGPU，且可能存在穩定性問題。

**Linux**

* Linux 上的 Mesa 驅動程式不被支援。

**任何平台**

* 整合式 GPU 不支援 x86-64（Intel、AMD）CPU 上。
* 不支援將 Sampler 與截取 Sampler 呼叫至圖形驅動程式的第三方軟體搭配使用。 此類軟體包括：
  * 後製注入器，例如可套用色彩分級、攝影機效果等的重著色器......
  * 螢幕上的覆蓋層，例如自訂準星、GPU 效能指標、影片串流介面......

## 最低 GPU 驅動程式版本

以下是應用程式無問題執行所需的最低 GPU 驅動程式版本清單。 隨著新版本釋出，此清單可能會有所變動。

要下載新驅動程式，請參考： [GPU 的驅動程式](https://experienceleague.adobe.com/zh-hant/docs/substance-3d-painter/using/technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers)已過時。

| 作業系統 | NVIDIA | AMD | Intel |
| --- | --- | --- | --- |
| **Windows** | GeForce 551.86 Quadro/RTX 538.33 | Radeon 23.8.1 Radeon Pro / FirePro 24.q2 | 31.0.1015590 |
| **Linux** | 525.116.04 或更新 *版本或* 535.54.03 或更新版本 | Radeon 23.20 Pro 23.Q3 | 未支援 |

>[!NOTE]
>
> 在 Mac OS **上**，GPU 驅動程式由作業系統本身提供。更新至作業系統最新版本以存取最新驅動程式。

## 語言

軟體介面提供以下語言版本：

* 英文
* 德語
* 法語
* 日文
* 韓文
* 中文
* 義大利語
* 葡萄牙語
* 西班牙語