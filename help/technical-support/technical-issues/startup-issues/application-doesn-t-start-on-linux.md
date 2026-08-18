---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/technical-support/technical-issues/startup-issues/application-doesn-t-start-on-linux.html"
breadcrumb-title: ''
description: 了解如何在 Linux 上解決 Substance 3D Sampler 啟動問題，以解決應用程式啟動問題和錯誤訊息。
helpx_creative_field: ""
helpx_description: Sampler > Technical Support > Technical Issues > Startup issues > Application doesnt start on Linux
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 應用程式無法在 Linux 上啟動
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '108'
ht-degree: 0%

---


# 應用程式無法在 Linux 上啟動

應用程式可能無法在 Linux 上啟動，終端機會出現以下錯誤訊息：

```
error while loading shared libraries: libicui18n.so.50
```


這表示 ICU（[International Components for Unicode](http://site.icu-project.org/)）函式庫要麼缺失，要麼安裝版本太新。 應用程式需要版本 50。

要解決這個問題，可以從套件管理器安裝版本 50，或 [手動下載](http://mirror.centos.org/centos/7/os/x86_64/Packages/libicu-50.2-4.el7_7.x86_64.rpm) 缺少的版本，安裝在 **/usr/lib64** 裡。
