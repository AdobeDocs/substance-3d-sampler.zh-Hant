---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/multiangle-to-material.html"
breadcrumb-title: ''
description: 使用 Substance 3D Sampler 中的「多角度到材質」工具，從多個角度拍攝的表面照片中建立材質。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Multiangle To Material
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 多角度到材質
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# 多角度到材質

![](../../assets/sat-multi-angle.png)

**多角度到材質**&#x200B;模板會從2到8張在特定光線條件下拍攝的輸入影像中產生材質。這種光照條件可以用材料掃描器達成。

>[!NOTE]
>
> 你可以在這篇文章](https://www.adobe.com/products/substance3d/magazine/your-smartphone-is-a-material-scanner-vol-ii.html)中找到更多關於如何製作材料掃描[器的資訊。

## 範例

以下是一個由 8 張輸入影像組成的材質範例：

* 前8張是掃描影像，拍攝角度為8個光角度。
* 底部的圖片是模板的輸出（基底顏色、法線、高度、金屬感和粗糙度）。

![](../../assets/scan-801x697.jpg){width="400px"}

## Substance 3D 取樣器配置

有三項要設定和設定，才能確保 PBR 通道能正確擷取：

* 掃描影像的順序
* 第一個輸入光角度
* 下一個輸入光角度

![](../../assets/multiangles-1024x1024.jpg){width="450px"}

### 掃描影像的順序

匯入圖片時，請在圖片匯入圖層中確認這8張圖片是連續的。

例如，0° 處的第一張影像應為 **scan1** ，然後 45° 的影像應為 **scan2** ...接著 315° 的影像應為 **scan8**

![](../../assets/multiangle-image-import.png){width="450px"}

### 第一光與次光角

在多角度到材料層中：

* 設定第一個輸入的光線角度。 如果你的掃描&#x200B;**1是180°，第一個輸入光角=0.5;如果******&#x200B;掃描1是0°，第一個輸入光角度=0
* 設定下一個輸入光角度：它定義影像旋轉的方向。 若 scan1 為 0°，則 scan2 為 45°...值為 **逆時針方向**

![](../../assets/multiangle-multiangle-to-material.png){width="450px"}
