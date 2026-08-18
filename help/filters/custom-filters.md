---
helpx_url: 'https://helpx.adobe.com/substance-3d-sampler/filters/custom-filters.html'
breadcrumb-title: ''
description: 學習如何在 Substance 3D Sampler 中使用自訂濾鏡，擴展 Substance Designer 濾鏡和自訂效果的功能。
helpx_creative_field: ''
helpx_description: Sampler > Filters > Custom Filters
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 自訂過濾器
user-guide-description: ''
user-guide-title: ''
source-git-commit: dc832dc546735437051226f4e1e731b55147b3ea
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---


# 自訂過濾器

## Substance 自訂過濾器

你可以透過 *圖層堆疊動作中的匯入* 按鈕，匯入用 Adobe Substance 3D Designer 製作的濾鏡。

### 建立物質過濾器

濾鏡必須在 Designer 中以特定方式建立，匯入 Sampler 後才能正常運作。

濾波器的輸入與輸出節點必須定義識別碼或使用方式。

>[!NOTE]
>
> **可以使用使用量**&#x200B;或&#x200B;**識別碼**（使用權優先權）。

#### 格式

將你的過濾器匯出為 Substance Archive 檔案（.SBSAR）

>[!NOTE]
>
> 你可以在 Sampler 裡直接暴露濾波器參數來控制濾波器。 點此查看操作指南[&#128279;](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/manage-parameters/exposing-a-parameter)

#### 建立濾鏡來修改圖片

![](../assets/image-template.png)

| 圖片名稱 | 使用情況 |
| --- | --- |
| *掃描1* | **掃描1** |
| *掃描2* | **掃描2** |
| *...* | **...** |

#### 建立一個濾波器來修改頻道

![](../assets/material-template.png)

| 頻道名稱 | 使用情況 |
| --- | --- |
| *底色* | **底色** |
| *彌漫* | **彌漫性** |
| *鏡面鏡面* | **鏡面** |
| *鏡面層級* | **高階級** |
| *金屬* | **金屬感** |
| *粗糙度* | **粗糙度** |
| *光澤* | **光澤感** |
| *正常* | **正常** |
| *高度* | **高度** |
| *環境遮蔽* | **環境遮蔽** |
| *不透明度* | **不透明度** |

>[!IMPORTANT]
>
> 在為 Sampler 建立自訂篩選器時，你需要在 Substance 圖表中加入以下使用者資料：
>
> 煉金術士：：類型=過濾器;

>[!IMPORTANT]
>
> 如果你的套件中有一個圖來處理影像（scan1 到 scanX），另一個圖用來處理材質（PBR 通道），Sampler 能根據濾波器在圖層堆疊中插入的位置選擇正確的圖。
>
> 在你的「圖片」圖中，加入以下使用者資料：
>
> * 煉金術士：：類型=過濾器;煉金術士：:variation:：類型=多重
>
> 在你的「材質」圖表上，加入以下使用者資料：
>
> * 煉金術士：：類型=過濾器;煉金術士：:variation:：類型=材料

### 具體參數

特定參數由應用程式全域管理。 這是一種在自訂篩選器中使用應用程式、專案和圖層堆疊的全域參數的方法。

#### 標準格式

對應用程式的正常格式控制。 在取樣器中設定為 DirectX

**參數識別碼**：normalformat、normal_format、$normalformat、$normal_format

#### 輸入計數

當你想修改影像（從 scan1 改成 scanX）時，可以透過 Image Count **參數來計算圖層堆疊**&#x200B;中的圖片數量。

* **參數識別碼**：input_count
* **參數類型**：整數

#### 材料輸入

如果你想在圖層堆疊中顯示一個材質槽，比如圖譜散布或濺射：

* 新增一組輸入節點（Base Color、Normal 等）
* 背景的所有輸入節點（圖層堆疊中最底層材質）都應該在 Group **Material1 中**
* 如果你想要多個材質槽，第一個想加的材料的所有輸入節點都應該放在 Group **Material2** 等欄位裡。
* 新增材料輸入參數：
  * **參數識別碼**：material_input
  * **參數類型**：整數

#### 工作流程類型

如果你想根據專案的工作流程（PBR Metalic/Roughness 或 PBR Specular/Glossiness）顯示或隱藏某些參數，可以使用工作流程類型參數

**參數識別碼**：workflow_type

**參數類型**：integer1，下拉選單

選項：

* 0：PBR 金屬質感/粗糙度
* 1：PBR 高光/光澤

![](../assets/workflow-type.jpg){width="300px"}
