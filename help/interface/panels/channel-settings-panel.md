---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/interface/panels/channel-settings-panel.html"
breadcrumb-title: ''
description: 學習如何使用 Substance 3D Sampler 的通道設定面板來管理材質通道並控制通道可見性。
helpx_creative_field: ""
helpx_description: Sampler > Interface > Panels > Channel Settings panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 頻道設定面板
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# 頻道設定面板

<table>
<tr style="border: 0;">
<td style="border: 0; width: 30%" valign="top">


**通道設定**&#x200B;面板控制你目前素材計算出的通道清單。你可以管理通道可見性、新增或移除素材中的通道，或更改所使用的材質模型。

</td>
<td style="border: 0;" valign="top">

![頻道設定面板。](../../assets/6.0_ChannelSettingsPanel.png)

</td>
</tr>
</table>

## 材質模型

用這個下拉選單選擇用來渲染材質的著色器框架。 通道設定面板&#x200B;**中的**&#x200B;選項會根據所選材質模型而改變。

當你更改材質模型時，新的模型需要重新計算圖層堆疊，並且會提供不同的通道。 取樣器試圖在轉換過程中盡量減少資料遺失;然而，這種變更可能會導致新材質模型在外觀上產生細微差異。

>[!NOTE]
>
> 可以從 Adobe 標準材料（ASM）切換到 OpenPBR，但目前無法從 OpenPBR 轉換到 ASM。


## 素材通道

<table>
<tr style="border: 0;">
<td style="border: 0; width: 30%" valign="top">


此區塊顯示根據工作流程預設計算的頻道列表。

你可以使用 **編輯清單按鈕** 開啟 **頻道選擇** ，並更改你素材計算的頻道。

</td>
<td style="border: 0;" valign="top">

![在標示材質通道區塊的通道設定面板中](../../assets/6.0_ChannelSettingsPanel_MaterialChannels.png){width="200px"}

</td>
</tr>
</table>

>[!NOTE]
>
> 例如，Substance Source 的某些材質不會輸出不透明度或環境遮蔽通道。 即使不透明度通道標示為「已計算中」，如果 Substance 檔案沒有輸出，Sampler 也不會產生它。

### 頻道選擇

頻道選擇視窗可以讓你從素材中新增或移除頻道。

![一張頻道選擇視窗的截圖，選取 Adobe Standard 材質為材質模型。](../../assets/6.0_ChannelSelectionWindow.png)

要將頻道加入你的素材，請選擇一個可用的頻道並使用 **>按鈕**。
要從你的素材中移除頻道，請從**「已選取頻道」列表中**&#x200B;選擇該頻道並使用&lt; button **** .
你可以用 **≫按鈕** 將所有可用頻道加入素材，或用 **≪按鈕**&#x200B;移除所有頻道。

你也可以用預設快速選取你素材的頻道列表。 預設情況下，Sampler 包含多個預設，但你也可以自行建立：

1. 把想要的頻道加入你的素材。
1. 使用 **「另存為預設」按鈕**。
1. 說出你的預設。

>[!NOTE]
>
>儲存預設不會把預設套用到你的素材上。

## 自訂頻道

切換預設未包含在所選工作流程中的額外通道。

<table>
<tr style="border: 0;">
<td style="border: 0; width: 30%" valign="top">

每個自訂頻道都有兩個選項可以用來控制：

1. 使用可見性切換來顯示或隱藏頻道在 2D 視圖中。
2. 使用 **自動按鈕** 切換頻道是否自動計算。
   * 當通道開啟時，如果堆疊上方的某層請求通道，該通道就會被計算出來。
   * 關閉後，通道總是被計算出來。

</td>
<td style="border: 0;" valign="top">

![頻道設定面板中自訂頻道區塊被高亮。](../../assets/6.0_ChannelSettingsPanel_CustomChannels.png){width="200px"}


</td>
</tr>
</table>



