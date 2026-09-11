---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-sampler/features-and-workflows/texture-import.html"
breadcrumb-title: ''
description: 學習如何將材質匯入 Substance 3D Sampler，以便在材質製作工作流程中使用現有的影像檔案。
helpx_creative_field: ""
helpx_description: Sampler > Features and workflows > Texture Import
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 材質匯入
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 2%

---


# 材質匯入

![](../assets/Capture-decran-2025-02-19-162128.png.img.png)

**材質匯入**&#x200B;範本會載入多張圖片，並根據檔名自動將它們連接到正確的輸出通道。

頻道匹配是根據以下所述的特定命名規則進行的。 若有重複或紋理不符，圖片會在介面中標示為重複。

## OpenPBR

取樣器會將以下 OpenPBR 識別碼的檔案與素材中對應的通道進行匹配。

>[!NOTE]
>
> 高度通道識別碼與 ASM 所使用的相同。


| OpenPBR 識別碼 | SBSAR 應用 |
| --- | --- |
| base_weight | 基礎重量 |
| base_color | baseColor |
| base_metalness | 金屬感/金屬感 |
| base_diffuse_roughness | 底底擴散粗糙度 |
| specular_weight | specularWeight（鏡面權重） |
| specular_color | specularColor |
| specular_roughness | 鏡面粗糙度/粗糙度 |
| specular_roughness_anisotropy | specularRoughness各向異性/各向異性水準 |
| specular_ior | specularIOR/IOR |
| transmission_weight | 變速箱重量 |
| transmission_color | 透射顏色/吸收顏色 |
| transmission_depth | 傳輸深度/吸收距離 |
| transmission_scatter | 傳輸散射 |
| transmission_scatter_anisotropy | 傳輸散射各向異性 |
| transmission_dispersion_scale | 傳輸擴散尺度 |
| transmission_dispersion_abbe_number | 傳輸擴散Abbe編號 |
| subsurface_weight | 次表面重量/半透明 |
| subsurface_color | 次表面色彩/散射色彩 |
| subsurface_radius | 次表面半徑/散射距離 |
| subsurface_radius_scale | 次表面半徑縮放/散射距離縮放 |
| subsurface_scatter_anisotropy | 地下散射各向異性 |
| coat_weight | coatWeight/coatOpacity（coat Weight/coatOpacity） |
| coat_color | 毛色 |
| coat_roughness | 毛皮粗糙度 |
| coat_roughness_anisotropy | coat 粗糙度各向異性 |
| coat_ior | 外套 |
| coat_darkening | 毛色變暗 |
| fuzz_weight | 模糊權重/光澤不透明度 |
| fuzz_color | 模糊色/光澤色 |
| fuzz_roughness | 模糊粗糙度/光澤粗糙度 |
| emission_weight | 排放重量 |
| emission_luminance | 發射亮度 |
| emission_color | 發射色/發光 |
| thin_film_weight | 薄膜重量 |
| thin_film_thickness | 薄膜厚度 |
| thin_film_ior | 薄膜 |
| 不透明度 | 不透明度 |
| thin_walled | 薄牆 |
| 正常 | 正常 |
| 切題 | 切題 |
| coat_normal | 毛色正常 |
| coat_tangent | 外套切線 |

## Adobe 標準教材

以下是每個頻道所支援的檔案命名慣例清單：

| **頻道** | **Adobe 標準教材** |
| --- | --- |
| **環境遮蔽** | <ul><li>環境遮蔽</li><li>AO</li><li>阻塞</li><li>ambient_occlusion</li></ul> |
| **底色** | <ul><li>底色</li><li>顏色</li><li>阿貝多</li><li>base_color</li><li>基座/底座</li><li>鞍部</li><li>顏色</li><li>base_colour</li><li>底色</li></ul> |
| **彌漫** | <ul><li>彌漫性</li><li>差異</li></ul> |
| **發射體** | <ul><li>發光/放射</li></ul> |
| **光澤** | <ul><li>光澤感</li><li>唇蜜</li></ul> |
| **高度** | <ul><li>高度</li><li>高度圖</li><li>遷移</li><li>Disp</li></ul> |
| **金屬** | <ul><li>金屬</li><li>MTL</li><li>金屬性</li></ul> |
| **正常** | <ul><li>正常</li><li>NRM</li></ul> |
| **不透明度** | <ul><li>不透明度</li><li>阿爾法</li></ul> |
| **粗糙度** | <ul><li>粗糙度</li><li>粗糙</li></ul> |
| **鏡面鏡面** | <ul><li>鏡面</li><li>規格</li></ul> |
| **鏡面層級** | <ul><li>高階級</li><li>specular_level</li></ul> |

