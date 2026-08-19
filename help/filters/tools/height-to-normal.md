---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/filters/tools/height-to-normal.html"
breadcrumb-title: ''
description: 在 Substance 3D Sampler 中使用 Height to Normal 工具，將高度貼圖轉換成法線貼圖，方便材質製作工作流程。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Height to Normal
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 身高到正常
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# 身高到正常

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-heighttonormal-18-n-d.png)

**收錄於：** 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

根據高度通道產生法線通道資料。

在下方圖片中，你可以看到 **「高度到法線」濾波器的** 運作。

![](../../assets/h2n-in.jpg)

在上圖中，材料沒有正常數據。 只有高度圖可用，並以 2D 視角&#x200B;**顯示**。

![](../../assets/h2n-out.jpg)

使用 **高度到法線濾波器**&#x200B;時，法線資料會從上方圖片所示的高度圖產生。 第二張圖片中，因為產生的法線貼圖，光線在材質上反射得更真實。

</td>
</tr>
</table>

## 參數

**基本參數**

* **使用世界單位**：切換\
  更改參數是否使用真實世界單位來衡量。 這會改變可用的參數。
  * **如果啟用了使用世界單位：**
    * **表面積（公分）：** 0-500\
      以世界單位來設定 UV 空間的大小
    * **身高深度（公分）：** 0-10\
      設定高度圖所代表的距離。 如果高度圖代表的距離很小，那麼高度圖值的差異很大可能會對法線角產生小幅影響。 如果高度圖代表一個大距離，那麼高度圖值的微小差異可以代表法線貼圖上的一個大角度。
  * **若停用使用世界單位：**
    * **強度**：0-3\
      調整法線角度的陡度
* **綜合最低標準：** 0-1\
  將現有的法線貼圖加入這個濾波器的結果中。

**面具**

* **自訂遮罩**：切換\
  啟用或停用自訂遮罩的使用。 啟用後會出現以下參數：
  * **遮罩**：影像/筆刷\
    選擇一張圖片作為遮罩，或用畫筆直接在 2D 視圖中繪製自訂遮罩
  * **自訂面具 - 模糊**：0-1\
    模糊面具
  * **自訂遮罩 - 反轉**：切換\
    反轉遮罩
