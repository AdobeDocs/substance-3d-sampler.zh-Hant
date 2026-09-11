---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/technical-support/configuration/update-checker.html"
breadcrumb-title: ''
description: 學習如何使用 Substance 3D Sampler 的更新檢查器，隨時掌握新版本和發行公告。
helpx_creative_field: ""
helpx_description: Sampler > Technical Support > Configuration > Update Checker
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 更新檢查器
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---


# 更新檢查器

更新視窗會顯示是否有新版本的物質鍊金術師可用，並顯示[&#128279;](../../release-notes/release-notes.md)最新的發行說明。

若有新版本可下載，啟動 Substance Alchemist 時會自動跳出此視窗。

可透過以下方法避免在啟動時顯示此視窗：

* 在視窗裡使用「不要提醒我直到下一個版本」的設定，暫時跳過視窗的顯示，直到下一個版本。
* 請在編輯偏好設定>>檢查更新中關閉&#x200B;**「檢查更新**」設定
* 使用命令列 **--skip-version-check** 它不會在 Substance Alchemist 啟動時檢查是否有新版本的應用程式可用
* 使用環境變數 **SUBSTANCE\_ALCHEMIST\_SKIP\_CHECK\_FOR\_UPDATES**:Value 0 或 1（1 = 停用更新檢查）

>[!NOTE]
>
> 自 Substance Alchemist 2020.1（2.1） 起支持。
