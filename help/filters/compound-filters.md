---
helpx_url: 'https://helpx.adobe.com/tw/substance-3d-sampler/filters/compound-filters.html'
breadcrumb-title: ''
description: 學習如何在 Substance 3D Sampler 中建立並使用複合濾鏡，將多個濾鏡合併成單一可重複使用的圖層。
helpx_creative_field: ''
helpx_description: Sampler > Filters > Compound Filters
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 複合濾波器
user-guide-description: ''
user-guide-title: ''
source-git-commit: dc832dc546735437051226f4e1e731b55147b3ea
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# 複合濾波器

此功能允許你建立一種新型的過濾器，這些過濾器在介面中以單一圖層表示，並由多個過濾器組成。

>[!NOTE]
>
> 自 Substance 3D Sampler 3.1.0 起支援

## 說明

複合過濾器是一個 **.ssafilter** 檔案，是一個 .7zip 壓縮資料夾，包含以下內容：

* 一個使用 JSON 格式的描述檔案： **myfilter\_name.json**
* 一個&#x200B;**&#x200B;**&#x200B;資源資料夾，內容包括：
  * 濾鏡縮圖：icon.png
  * 外部檔案相依關係

### 描述檔案內容

* 名稱：介面中顯示的複合濾波器標籤
* Id：你化合物過濾器的唯一識別碼
* 類別：當你依類別分組資產時，資產面板中使用的複合過濾器類別
* 版本：遞增數定義複合濾波器的版本。
* 節點：將使用的節點列表
* 連結：不同節點間的連接列表

### 範例

```JSON
{ "SamplerFilter":  
 { 
 "Name": "My filter", 
 "Category": "My filter category", 
 "Id": "my_unique_id", 
 "Version": 2, 
 "Node": [ 
        { 
            "Id": "foo", 
            "InternalFilter": "Foo" 
        }, 
        { 
            "Id": "bar", 
            "File": "bar.sbsar" 
        } 
    ], 
    "Link": [ 
        { 
            "From": { "Node": "FilterInput", "Usage": "baseColor" }, 
            "To": { "Node": "foo", "Usage": "baseColor"} 
        }, 
        { 
            "From": { "Node": "FilterInput", "Usage": "normal" }, 
            "To": { "Node": "foo", "Usage": "normal"} 
        }, 
        { 
            "From": { "Node": "foo", "Usage": "baseColor" }, 
            "To": { "Node": "bar", "Usage": "baseColor"} 
        }, 
        { 
            "From": { "Node": "bar", "Usage": "baseColor" }, 
            "To": { "Node": "FilterOutput", "Usage": "baseColor"} 
        }, 
        { 
            "From": { "Node": "foo", "Usage": "normal" }, 
            "To": { "Node": "FilterOutput", "Usage": "normal"} 
        } 
    ] 
}}
```

## 逐步建立

1. 建立一個新檔案： **my\_new\_filter.json**
1. 請定義其名稱、ID、類別,...
1. 定義你需要的節點清單
1. 如果你需要外部檔案，可以在.json **旁邊建立**&#x200B;資源&#x200B;**資料夾**
1. 把你的檔案加入 **資源** 資料夾
1. 寫出節點間的連結清單
1. 確認你的 JSON 是否有效（沒有打字、漏逗號或缺少括號）
1. 如果你想要縮圖，可以在資源&#x200B;**資料夾裡icon.png**&#x200B;**新增一張圖片**
1. 選擇 **.json** 檔案和 **資源** 資料夾，然後用 7zip 壓縮

## 文件

### 版本

使用版本號可以讓你追蹤不同的版本。 當你打開用舊版本複合過濾器完成的圖層堆疊時，會跳出通知建議你升級到最新版本。

### 節點

節點可指 Substance 3D Sampler 的內部過濾器。 定義一個 **唯一識別碼 Id** ，用於定義節點間的連結，以及內部過濾器 **InternalFilter 的標籤**

```JSON
{ 
  "Id": "step1_identifier", 
  "InternalFilter": "Dirt" 
}
```

節點可以指向 Substance 3D Sampler 中不存在的 SBSAR 檔案。 定義一個用於定義節點間連結的唯一識別碼 **Id** ，以及 SBSAR 檔案的檔案名稱 **File** 。 SBSAR 檔案必須放在 **.alchfilter 檔案旁邊的 resources** 資料夾裡。

```JSON
{ 
  "Id": "step1_identifier", 
  "File": "foo.sbsar" 
}
```

>[!NOTE]
>
> **filterImg** 和 **filterMat** 不能用作節點 ID

### 連結

連結是描述兩個節點如何連結的過程，由兩個元素組成：

* 來源：節點使用的使用情況
* 收件人：節點的使用輸出

每個元素有三個屬性：

* Node：宣告&#x200B;**你想使用的節點的 ID**
  * 設定複合濾波器的輸入，節點 ID 為 **FilterInput**
  * 設定你的複合層輸出，節點 ID 是 **FilterOutput**
* 使用方式：宣告你想使用的使用方式。 有三種選擇：
  * 一次只用一次，並逐個連結聲明（baseColor、normal、height、ambientOcclusion、roughness、metallic、diffuse、specular、glossiness、specularLevel、不透明度、發射、掃描1等）
  * 你也可以指定一個清單 [“baseColor”， “normal”]。 From 清單的第一&#x200B;**項會和 To** 清單的第一&#x200B;**項相**&#x200B;匹配。等等......
  * 使用 **\*** 讓 Substance 3D Sampler 來匹配 From 節點與 To 節點所有相同用途的使用情況（無法將 \*** 與其他連結合併**，但同一節點間可以合併單一連結和列表連結）
* 群組：如果某節點使用次數是多次相同，你可以使用群組屬性來選擇特定的使用方式。 例如：對於混合濾鏡，要取得底部材質 *的 baseColor，使用 Material1* ;若要取得頂部材質的 BaseColor，則使用 *Material2*

```JSON
Link between two nodes  
{ 
  "From": { "Node": "node1","Usage": "baseColor", "Group": ""}, 
  "To": { "Node": "node2", "Usage": "baseColor"} 
} 
 
Link between outputs of layers below of the compound filter and the compound filter: 
{ 
  "From": { "Node": "FilterInput", "Usage": "*" }, 
  "To": { "Node": "node1", "Usage": "*"} 
} 

Link to declare outputs of the compound filter: 
{ 
  "From": { "Node": "node1", "Usage": "*" }, 
  "To": { "Node": "FilterOutput", "Usage": "*"} 
}
```
