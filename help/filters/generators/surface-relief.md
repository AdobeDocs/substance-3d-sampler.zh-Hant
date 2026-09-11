---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/generators/surface-relief.html"
breadcrumb-title: ''
description: 使用 Substance 3D Sampler 中的表面浮雕產生器，在材料中創造壓花和浮雕表面圖案。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Surface Relief
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 地表起伏
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# 地表起伏

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-surfacerelief-18-n-d.png)

**收錄於：** 《發電機》

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 說明

使用表面浮雕濾波器來增加你的材質雜訊。 這有助於打破大形狀或增加視覺趣味。

</td>
</tr>
</table>

## 參數

<b>基本參數</b>

* <b>隨機種子</b>：\
  這個隨機種子，而這個過濾器中所有其他隨機參數都是基於它。
* <b>強度</b>：0-1\
  改變噪音的振幅
* <b>模糊強度</b>：0-1\
  模糊的強度與噪音相呼應
* <b>表面瑕疵 </b>：影像/筆刷/貼圖產生器\
  可以用圖片或材質產生器作為表面瑕疵。

<b>噪音參數</b>

* <b>克蘭普</b>：0-1\
  將噪音壓縮到一定範圍
* <b>比分</b>：0-1\
  調整噪音的對比度
* <b>反轉</b>：切換\
  反轉噪音的高度圖

<b>轉換</b>

* <b>瓷磚：</b>1-16\
  與 Basic 參數>的縮放</b>不同<b>，<b>平鋪</b>管理的是噪音的實例數量。
* <b>鏡子</b>：\
  將噪音在一個或兩個軸上鏡像
* <b>偏移</b>：\
  將噪聲重新定位在 X 軸和 Y 軸
* <b>輪替：</b>\
  調整噪音。 旋轉角度會變快，以確保仍可鋪磚。

<b>面具</b>

* <b>使用自訂遮罩</b>：切換\
  啟用以查看自訂遮罩控制項：
  * <b>遮罩</b>：image/brush/Texture Generator\
    匯入圖片作為遮罩，或直接用畫筆在 2D 視圖中 <b>繪畫</b>
  * <b>自訂面具 - 模糊</b>：0-1\
    模糊面具
  * <b>自訂遮罩 - 反轉</b>：切換

<b>進階參數</b>

* <b>身高強度</b>：0-1\
  控制噪音高度圖與底層材質高度圖的混合
* <b>高度 - 更換底座</b>：切換\
  切換是否更換底座高度
* <b>正常強度</b>：0-1\
  調整噪音法線貼圖的強度
* <b>普通 - 更換底座</b>：切換\
  切換是否替換基礎法線貼圖
* <b>法線方向</b>：\
  修改用於正常生成的軸
* <b>法線 - 旋轉方向</b>
* <b>環境遮蔽 - 強度</b>
* <b>環境遮蔽 - 橈骨</b>
