---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/generators/brickwall.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的磚牆產生器，為材料製作逼真的磚牆圖案和磚石材質。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Brickwall
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 磚牆
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---


# 磚牆

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-brickwall-18-n-d.png)

**收錄於：** 《發電機》

</td>
<td width="58.30%" style="border: 0;" valign="top">

說明磚牆濾波器會根據其下方的層級產生磚塊圖案。 這對磚牆（顧名思義）和地板或其他使用磚塊的地方都很有用。

下方圖片中，黏土材料經過磚牆濾鏡轉換成磚牆 **。**

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0053-brickwall-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0052-brickwall-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## 參數

**預設音色**

從多個預設中選擇，快速模擬特定風格。

**基本參數**

* **隨機種子**：隨機數\
  此隨機值用於決定此篩選器中其他隨機值。\
  點擊該數字即可獲得新的隨機數值。 當隨機選中後，點擊參數名稱將該值重置為 0。
* **磚塊債券**：\
  根據所選風格將磚塊合併
* **磚塊類型**：\
  選擇磚塊的款式
* **牌塊**：1-25\
  改變 X 軸和 Y 軸的鋪磚量。
* **偏離**&#x200B;比分：0-1\
  修改每排磚塊與前一排的偏移量。
* **使用自訂顏色**：切換\
  根據所選風格將磚塊合併

**混音**

* **混合模式**：\
  改變磚塊的組織方式。 使用 **混合模式會** 產生第二組磚塊，可以獨立於基礎組控制。\
  當 **混合模式** 設為 **無**&#x200B;時，此區塊中不會出現其他參數。
* **磚塊類型2**：\
  選擇第二組磚塊的樣式。
* **身高差錯：** 0-1\
  偏移第二組磚塊的高度

**水泥**

* **水泥色素**：選色器\
  在磚塊之間改變水泥的顏色。
* **水泥粗糙度**：0-1\
  改變磚塊間水泥的粗糙度。
* **水泥間隙**：0-1\
  改變磚塊間水泥的寬度。 改變磚塊大小。
* **水泥等級**：0-1\
  改變水泥的高度
* **水泥失調**：0勝1負\
  調整水泥的平整度。 在高價下，水泥可以高高地疊起。

**年代**

* **磚隊失序**：0勝1負\
  隨機調整每塊磚在三維空間的旋轉。
* **磚碎**：0-1\
  在磚牆上加縫隙
* **布里克埃奇**：0-1\
  損壞並破壞磚塊邊緣
* **磚頭解困**：0-1\
  隨機移除磚塊
* **磚塊顏色變化**：0-1\
  改變磚塊的顏色，讓牆面看起來不那麼均勻
* **磚頭髒：** 0-1\
  在磚塊上加土

**進階參數**

* **高度混合強度**：0-1\
  調整基材高度的混合。 值為 0 則忽略基材高度，僅使用 Brickwall 濾波器參數來產生高度資訊。 值為 1 則會利用底材產生高度資訊。
* **正常強度**：0-1\
  調整 Brickwall 濾波器產生的法線強度。 值為 0 等於沒有法線。
* **環境遮蔽強度**：0-1\
  調整AO的強度。 值為 0 實際上代表沒有環境遮蔽。

使用指南

磚牆過濾器會將底層材料分解成獨立磚塊，然後重新排列。 因此，磚牆過濾器最適合處理硬表面如岩石或金屬——換句話說，這些材料最適合在現實世界中作為磚塊。

磚牆濾鏡很適合用來製作基底材質，然後再在上面疊加其他效果，比如苔蘚、雪或泥土。
