---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/technical-support/configuration/retrieving-the-installation-path.html"
breadcrumb-title: ''
description: 學習如何在不同平台上取得 Substance 3D Sampler 的安裝路徑，以便腳本和設定。
helpx_creative_field: ""
helpx_description: Sampler > Technical Support > Configuration > Retrieving the installation path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 取回安裝路徑
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 1%

---


# 取回安裝路徑

本頁彙整了根據版本與平台，如何取得應用程式安裝路徑的資訊。

## 窗戶

### 創意雲端桌面

1. 開啟 Windows 登錄檔編輯器（**regedit**）。
1. 請前往登錄檔鍵：** HKEY\_LOCAL\_MACHINE\Software\Microsoft\Windows\CurrentVersion\App Paths\**
1. 打開名為 **Adobe Substance 3D 的子鍵Sampler.exe**
1. 該金鑰的值包含應用程式執行檔安裝地點的路徑

>[!NOTE]
>
> 此登錄檔金鑰僅從版本 3 開始提供。\
> 對於較舊版本，安裝路徑可從 HKEY\_CURRENT\_USER\Software\Microsoft\Windows\CurrentVersion\ Explorer\FileExt **的檔案關聯**&#x200B;中取得。

### Substance 3D 獨立版

1. 開啟 Windows 登錄檔編輯器（**regedit**）。
1. 請前往登錄檔鍵 **：HKEY\_LOCAL\_MACHINE\ SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall**
1. 找出與你應用程式版本 AppID 相符的子金鑰（見下表）
1. 該密鑰的值包含通往應用程式安裝位置的路徑

| 版本 | AppID |
| --- | --- |
| **1.x（2019.x）至2.x** | {B3506E85-E98F-4D48-A010-BE4DEE27D108} |
| **3.x（或更新版本）** | {ED4A4ABC-9B7D-44B8-984A-C8A994B69CFD} |

### 蒸汽

該應用程式安裝在 **Steam 安裝資料夾的 steamapps/common/** 子資料夾中。

## 麥克

在 Mac 上，該應用程式安裝於以下格式：

| 版本 | 路徑 |
| --- | --- |
| **3.x 或更新版本** | **/應用程式/Adobe Substance 3D Sampler.app** |
| **遺產** | **/應用/實質 Alchemist.app** |

## Linux

在 Linux 上，rpm 套件的安裝路徑如下：

| 版本 | 路徑 |
| --- | --- |
| **3.x 或更新版本** | **/opt/Adobe/Adobe\_Substance\_3D\_Sampler** |
| **遺產** | **/opt/寓言/實質\_Alchemist** |
