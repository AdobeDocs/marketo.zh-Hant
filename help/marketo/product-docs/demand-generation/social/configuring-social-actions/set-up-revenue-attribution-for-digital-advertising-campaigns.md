---
unique-page-id: 10098812
description: 設定數位廣告促銷活動的收入歸因 — Marketo檔案 — 產品檔案
title: 設定數位廣告促銷活動的收入歸因
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# 設定數位廣告促銷活動的收入歸因 {#set-up-revenue-attribution-for-digital-advertising-campaigns}

以下說明如何為數位廣告頻道和行銷活動設定收入歸因。 設定後，您就可以對數位廣告執行首次接觸和多次接觸的收入歸因，如同其他Marketo計畫。

在Marketo中設定第一個廣告程式後，您可以複製並更新為其他通道。 例如，將LinkedIn程式複製到Facebook程式。

然後，通過單獨的程式，您可以跟蹤每個程式的轉換次數，並在Program Analyzer、Opportunity Influence Analyzer和其他Marketo Analytics功能中查看您的程式。

>[!PREREQUISITES]
>
>* 設定具有狀態值和方案成功（例如數位廣告或Social付費和PPC）的管道標籤
>* 建立或編輯表單以將查詢字串傳遞至人員
>* 請確定您有權存取某些「收入週期分析」功能，以報告您的廣告頻道和促銷活動


## 建立預設程式 {#create-a-default-program}

與某些程式（如電子郵件）不同，預設程式始終處於開啟狀態。

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-5.png)

1. 按一下 **新增** 選取 **新計畫**.

   ![](assets/image2016-3-14-15-52-0.png)

1. 如果已有計畫，您可以 [複製](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >每當復製程式時，請務必替換智慧清單的查詢字串欄位中的名稱。

1. 設定初始方案後，將新方案放置在特定的促銷活動資料夾中。

   >[!NOTE]
   >
   >**範例**
   >
   >透過URL傳遞的查詢字串，可協助Marketo了解在Marketo中成為人員時，訪客點擊了哪個廣告促銷活動。
   >
   >您可以建立查詢字串方法，其中包含您要測量的所有變數。 Marketo使用這些變數將使用者新增至您的不同程式。
   >
   >例如，您可以使用Channel type_Channel__Asset__Region。 這看起來可能像：SP_FB_NewGuide_US。 **附註**:縮寫儲存空間。
   >
   >或者，將其設定為Channel_Adsource_AssetName_Region_UniqueIdNumber。 這看起來可能像：Social-Paid_Facebook_NewGuide_NA_123。

## 為新名稱建立智慧型促銷活動 {#create-a-smart-campaign-for-new-names}

1. 在智慧型行銷活動中，建立包含兩個觸發器和兩個篩選器的智慧型清單，如所示。

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >兩個觸發器和 **捕獲名稱的程式** 篩選器是您專屬的。 此處顯示的查詢字串僅為範例。 如果您複製了欄位，請直接取代這些欄位。

1. 建立流程步驟，將屬性變更為 **贏取計畫** 並將「新值」設為您為付費社交行銷活動定義的值。

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. 排程並啟動促銷活動。

## 建立智慧型促銷活動以取得狀態/方案成功 {#create-a-smart-campaign-for-status-program-success}

您需要第二個智慧型行銷活動來變更人員狀態，讓他們能夠取得方案成功，並納入收入歸因計算中。

1. 在 **填寫表單** 觸發，在查詢字串中輸入程式名稱。 如果要復製程式，只需用新的查詢字串名稱替換舊的查詢字串名稱即可。

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. 建立流程步驟，將狀態更改為與程式成功關聯的狀態。

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >上例顯示 **已轉換**，但這取決於您的狀態/成功值。

1. 排程並啟動促銷活動。

## 建立廣告 {#create-your-ad}

設定方案和行銷活動後，請建立新廣告。

1. 前往頻道；例如LinkedIn或Facebook。
1. 建立新廣告。
1. 選取Marketo登陸頁面，作為促銷活動中「呼叫動作」的目的地。
1. 將查詢字串新增至URL。

   >[!NOTE]
   >
   >**範例**
   >
   >以下說明如何將您設定的所有資訊新增至實際URL。 這些項目以&amp;符號分隔：
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **來源** 是作為管道識別碼的「人員來源」
   >* **註解** 是為每個程式建立的唯一標識符
   >* **營地** 是Facebook、LinkedIn或Google中的促銷活動
   >* **k** 是您要擷取的關鍵字或資產名稱

   >
   >**這四個詞必須全部小寫，URL中不能有空格才能擷取此資訊。**

## 最佳實務 {#best-practices}

使用單一管道標籤來呈現所有數位廣告，或如果您想要與其他行銷管道（例如社交付費、搜尋付費、顯示、重新鎖定）進行更精細的比較，則使用多個管道標籤。

然後，針對您需要的每個報表檢視設定不同的程式。 如果您有10個地區一起啟動「Big Campaign」，且想要能夠跨地區檢視結果，請在查詢字串的URL（例如BC）中使用通用ID作為參數。

如果您想要報告每個地區以及大型活動的集體成果，請建立11個方案 — 每個地區各一個，大型活動各一個。 每個程式僅引用查詢字串（如BC）中的相關字元。

「大行銷活動」和「地區」計畫之間的人數有故意重疊，因此您不想報告所有11個計畫的總人數，因為「大行銷活動」和「地區」計畫中都有一些人。
