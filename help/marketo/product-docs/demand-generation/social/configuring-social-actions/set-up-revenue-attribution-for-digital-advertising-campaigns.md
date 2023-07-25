---
unique-page-id: 10098812
description: 設定數位廣告行銷活動的收入歸因 — Marketo檔案 — 產品檔案
title: 設定數位廣告行銷活動的收入歸因
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# 設定數位廣告行銷活動的收入歸因 {#set-up-revenue-attribution-for-digital-advertising-campaigns}

以下說明如何設定數位廣告頻道和行銷活動的收入歸因。 完成設定後，您可以像在其他Marketo程式中一樣，對數位廣告執行首次接觸和多點接觸收入歸因。

在Marketo中設定第一個廣告程式後，您可以複製並更新其他頻道的該程式。 例如，將LinkedIn程式複製至Facebook程式。

透過個別程式，您可以追蹤每個程式的轉換次數，並在Program Analyzer、Opportunity Influence Analyzer和其他Marketo Analytics功能中檢視您的程式。

>[!PREREQUISITES]
>
>* 設定具有狀態值和方案成功的頻道標籤（例如，數位廣告或社交付費和PPC）
>* 建立或編輯表單，以透過人員傳遞查詢字串
>* 請確定您有權存取某些Revenue Cycle Analytics功能，以便針對您的廣告頻道和行銷活動製作報表

## 建立預設計畫 {#create-a-default-program}

有些程式（例如電子郵件）可能會定期執行一段特定時間，預設程式則一律開啟。

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-5.png)

1. 按一下 **新增** 並選取 **新計畫**.

   ![](assets/image2016-3-14-15-52-0.png)

1. 如果您已有程式，您可以 [原地複製](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >每當您復製程式時，請務必取代智慧列示的查詢字串欄位中的名稱。

1. 設定初始方案後，將新方案放在特定的行銷活動資料夾中。

   >[!NOTE]
   >
   >**範例**
   >
   >透過URL傳遞的查詢字串有助於Marketo知道當某人在Marketo中成為某人時，他們點選了哪個廣告行銷活動。
   >
   >您可以建立查詢字串方法，納入您要測量的所有變數。 Marketo使用這些變數將人員新增至您的不同程式。
   >
   >例如，您可以使用管道type_Channel__Asset__Region。 看起來可能像這樣：SP_FB_NewGuide_US。 **注意**：縮寫可節省空間。
   >
   >或者，將其設定為Channel_Adsource_AssetName_Region_UniqueIdNumber。 類似於：Social-Paid_Facebook_NewGuide_NA_123。

## 為新名稱建立Smart Campaign {#create-a-smart-campaign-for-new-names}

1. 在智慧行銷活動中，建立包含兩個觸發器和兩個篩選器的智慧清單，如下所示。

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >兩個觸發器中使用的查詢字串，以及 **擷取名稱的程式** 篩選器是您專屬的。 此處顯示的查詢字串僅供範例使用。 如果您複製欄位，只需取代這些欄位即可。

1. 建立流程步驟以將屬性變更為 **贏取方案** 並將新值設定為您為付費社交行銷活動定義的值。

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. 排程並啟動行銷活動。

## 建立狀態/方案成功的Smart Campaign {#create-a-smart-campaign-for-status-program-success}

您需要第二個智慧型行銷活動來變更人員狀態，以便讓人員取得方案成功並包含在收入歸因計算中。

1. 在 **填寫表單** 觸發程式，在查詢字串中輸入程式名稱。 如果您要復製程式，只需將舊的查詢字串名稱替換為新的查詢字串名稱即可。

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. 建立流程步驟以將狀態變更為與方案成功相關的狀態。

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >上述範例顯示 **已轉換**，但這取決於您的狀態/成功值。

1. 排程並啟動行銷活動。

## 建立您的廣告 {#create-your-ad}

設定方案和行銷活動後，請建立新廣告。

1. 前往管道；例如LinkedIn或Facebook。
1. 建立新廣告。
1. 選取Marketo登陸頁面，作為行銷活動中行動號召的目的地。
1. 將查詢字串新增至URL。

   >[!NOTE]
   >
   >**範例**
   >
   >以下說明如何將您設定的所有資訊新增至實際URL。 專案之間以&amp;號分隔：
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **source** 作為管道識別碼的「個人來源」
   >* **評論** 是為每個方案建立的唯一識別碼
   >* **camp** 是Facebook、LinkedIn或Google中的促銷活動
   >* **kk** 是要擷取的關鍵字或資產名稱
   >
   >**這四個字詞必須全部小寫，且URL中不能有任何空格才能擷取此資訊。**

## 最佳實務 {#best-practices}

使用單一管道標籤來代表所有數位廣告，或者如果您想要與其他行銷管道進行更細微的比較（例如，社交付費、搜尋付費、顯示、重新目標定位），則使用多個管道標籤。

然後，針對您需要的每個報表檢視設定不同的程式。 如果您有10個地區同時啟動「Big Campaign」，而且想要能夠跨地區檢視結果，請使用通用ID作為查詢字串中URL的引數（例如BC）。

如果您想要報告每個地區以及Big Campaign的集體結果，請建立11個方案 — 每個地區一個，Big Campaign一個。 每個程式只會參考查詢字串中的相關字元（例如BC）。

Big Campaign與地區計畫之間有意重疊個人計數，因此您不想報告所有11個計畫的總個人計數，因為有些人同時在Big Campaign和其中一個地區計畫。
