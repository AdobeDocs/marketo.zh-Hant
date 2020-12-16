---
unique-page-id: 10098812
description: 設定數位廣告宣傳的收入歸因——行銷檔案——產品檔案
title: 設定數位廣告宣傳的收入歸因
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---


# 設定數位廣告宣傳的收入歸因 {#set-up-revenue-attribution-for-digital-advertising-campaigns}

以下說明如何為數位廣告通道和宣傳活動設定收入歸因。 設定之後，您就可以針對數位廣告進行首次接觸和多點接觸收入歸因，就像在其他Marketo方案中一樣。

在Marketo中設定您的第一個廣告程式後，您可以複製並更新其他頻道。 例如，將LinkedIn程式複製至Facebook程式。

然後，您可以使用個別的程式來追蹤每個程式的轉換次數，並在Program Analyzer、Opportunity Influce Analyzer和其他Marketo Analytics功能中查看您的程式。

>[!PREREQUISITES]
>
>* 設定具有狀態值和方案成功的渠道標籤（例如，數位廣告或Social付費和PPC）
>* 建立或編輯表單，以將查詢字串與人員傳遞
>* 請確定您有權存取某些「收入週期分析」功能，以報告您的廣告通道和促銷活動

>



## 建立預設程式 {#create-a-default-program}

與某些程式（例如電子郵件）不同，預設程式會定期執行一段時間，但一律開啟。

1. 前往行 **銷活動**。

   ![](assets/login-marketing-activities-5.png)

1. 按一下 **新建** ，然後選 **擇新建程式**。

   ![](assets/image2016-3-14-15-52-0.png)

1. 如果已有程式，可以克 [隆](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md)。

   >[!TIP]
   >
   >每當克隆程式時，請務必替換智慧清單的查詢字串欄位中的名稱。

1. 在設定初始程式後，將新程式放入特定的促銷活動資料夾。

   >[!NOTE]
   >
   >**範例**
   >
   >
   >透過URL傳遞的查詢字串可協助Market得知某人在成為Marketo中的人時點選了哪個廣告促銷活動。
   >
   >
   >您可以建立查詢字串方法，其中包含您要測量的所有變數。 Marketo會使用這些變數，將人員新增至不同的程式。
   >
   >
   >例如，您可以使用Channel type_Channel_Asset_Region。 這看起來可能是：SP_FB_NewGuide_US。 **注意**:縮寫儲存空間。
   >
   >
   >或者，將其設為Channel_Adsource_AssetName_Region_UniqueIdNumber。 這看起來可能是：Social-Paid_Facebook_NewGuide_NA_123。

## 建立新名稱的智慧型促銷活動 {#create-a-smart-campaign-for-new-names}

1. 在智慧型促銷活動中，建立包含兩個觸發器和兩個篩選器的智慧型清單，如所示。

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >這兩個觸發器和「捕獲的名稱 **程式」篩選器中使用的查詢字串** 。 此處顯示的查詢字串僅為範例。 如果您已複製欄位，請直接取代這些欄位。

1. 建立流程步驟，將屬性變更為 **贏取方案** ，並將「新值」設定為您為付費社交促銷活動所定義的值。

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. 排程並啟動促銷活動。

## 為狀態／計畫成功建立智慧型促銷活動 {#create-a-smart-campaign-for-status-program-success}

您需要第二個智慧型促銷活動來變更人員狀態，以便他們能夠取得方案成功並納入收入歸因計算。

1. 在「填 **出表單」觸發器** ，在查詢字串中輸入程式名稱。 如果要克隆程式，只需將舊的查詢字串名稱替換為新名稱。

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. 建立流程步驟，將狀態變更為與程式成功相關的步驟。

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >上述範例顯示**Converted, **，但這取決於您的狀態／成功值。

1. 排程並啟動促銷活動。

## 建立您的廣告 {#create-your-ad}

在您設定方案和促銷活動後，請建立新廣告。

1. 前往頻道；例如，LinkedIn或Facebook。
1. 建立新廣告。
1. 選擇行銷人員登陸頁面作為促銷活動中行動呼籲的目的地。
1. 新增查詢字串至URL。

   >[!NOTE]
   >
   >**範例**
   >
   >
   >以下說明如何將您設定的所有資訊新增至實際URL。 項目以&amp;符號分隔：
   >
   >
   >[www.marketo.com?**source**=Social-Paid&amp;**comment**=Social-Paid_Facebook_NewGuide_NA&amp;**camp**=abc&amp;**k=**xyz](http://www.marketo.com?source=Social-Paid&amp;comment=Social-Paid_Facebook_NewGUide_NA&amp;camp=abc&amp;kk+xyz)
   >
   >    
   >    
   >    * **source** 是用作渠道識別碼的人員來源
   >    * **comment** 是為每個程式建立的唯一標識符
   >    * **camp** 是Facebook、LinkedIn或Google中的促銷活動
   >    * **kk** 是您要擷取的關鍵字或資產名稱

   >    
   >    
   >**這4個詞語必須全部為小寫，而且URL中不能有任何空格，才能擷取此資訊。**

## 最佳實務 {#best-practices}

使用單一渠道標籤來代表所有數位廣告，或如果您想要與其他行銷渠道（例如社交付費、搜尋付費、顯示、重新定位）進行更詳細的比較，則使用多個渠道標籤。

然後，針對您需要的每個報表檢視設定不同的程式。 如果您有10個地區同時啟動「大型促銷活動」，並想要能夠跨地區檢視結果，請在查詢字串的URL（例如BC）中使用通用ID做為參數。

如果您想要報告每個地區以及大型促銷活動的集體結果，請建立11個方案——每個地區各一個，大型促銷活動各一個。 每個程式僅引用查詢字串中的相關字元（如BC）。

「大促銷活動」和「地區」計畫之間的人數有意重疊，因此您不想報告所有11個計畫的總人數，因為「大促銷活動」和其中一個地區計畫都有一些人。
