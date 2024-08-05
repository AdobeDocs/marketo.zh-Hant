---
unique-page-id: 10098812
description: 設定數位Advertising行銷活動的收入歸因 — Marketo檔案 — 產品檔案
title: 設定數位Advertising行銷活動的收入歸因
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# 設定數位Advertising行銷活動的收入歸因 {#set-up-revenue-attribution-for-digital-advertising-campaigns}

以下說明如何為數位廣告渠道和營銷活動設定收入 歸因。 完成設定後，您可以像在其他Marketo程式中一樣，對數位廣告執行首次接觸和多點接觸收入歸因。

>[!IMPORTANT]
>
>自2024年7月31日起，我們開始淘汰此功能的程式。 您將無法建立新資產。 現有資產將持續運作至2025年1月31日。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

在Marketo中設定第一個廣告程式後，您可以複製並更新其他頻道的該程式。 例如，將LinkedIn程式複製至Facebook程式。

透過個別程式，您就可以追蹤每個程式的轉換次數，並在Program Analyzer、Opportunity Influence Analyzer和其他Marketo Analytics功能中檢視您的程式。

>[!PREREQUISITES]
>
>* 設定具狀態值和方案成功的通道 標記 （例如，數字廣告或付費和 PPC Social）
>* 建立或編輯表單以將查詢字串傳遞給該人員
>* 請確定您有權存取部分Revenue Cycle Analytics功能，以便報告您的廣告頻道和行銷活動

## 建立預設計畫 {#create-a-default-program}

與某些程式（例如電子郵件）可能定期在特定時段執行不同，預設程式會一直開啟。

1. 前往 **營銷活動**。

   ![](assets/login-marketing-activities-5.png)

1. 按一下&#x200B;**新然後選擇**&#x200B;新程式&#x200B;****。

   ![](assets/image2016-3-14-15-52-0.png)

1. 如果已有方案，則可以 [克隆它](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md)。

   >[!TIP]
   >
   >每當您複製方案時，請務必替換智能清單查詢字串字段中的名稱。

1. 設定初始方案后，將新方案放置在特定的行銷活動資料夾中。

   >[!NOTE]
   >
   >**範例**
   >
   >透過URL傳遞的查詢字串有助於Marketo知道某個人在Marketo中成為人員後所點選的廣告行銷活動。
   >
   >您可以建立查詢字串方法，納入您要測量的所有變數。 Marketo使用這些變數將人員新增至您的不同程式。
   >
   >例如，您可以使用管道type_Channel__Asset__Region。 這可能看起來按讚：SP_FB_NewGuide_US。 **注意**：縮寫可節省空間。
   >
   >或者，將其設置為 Channel_Adsource_AssetName_Region_UniqueIdNumber。 這可能類似於：Social-Paid_Facebook_NewGuide_NA_123。

## 為新名稱建立智慧型行銷活動 {#create-a-smart-campaign-for-new-names}

1. 在智慧行銷活動中，建立包含兩個觸發器和兩個篩選器的智慧清單，如下所示。

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >兩個觸發程式和&#x200B;**擷取名稱的程式**&#x200B;篩選器中使用的查詢字串是您獨有的。 此處顯示的查詢字串僅為範例。 如果您複製欄位，只需取代這些欄位即可。

1. 建立流程步驟以將屬性變更為&#x200B;**贏取方案**，並將新值設定為您為付費社交行銷活動定義的值。

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. 排程并啟用行銷活動。

## 建立狀態/方案成功的Smart Campaign {#create-a-smart-campaign-for-status-program-success}

您需要第二個智慧型行銷活動來變更人員的狀態，以便他們能夠實現方案成功並包含在收入歸因計算中。

1. 在&#x200B;**填寫表單**&#x200B;觸發器中，在查詢字串中輸入程式名稱。 如果您要復製程式，只需將舊的查詢字串名稱取代為新名稱即可。

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. 建立流程步驟以將狀態變更為與方案成功相關聯的狀態。

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >上面的範例顯示 **「已轉換」，**&#x200B;但這取決於您的狀態/成功值。

1. 排程并啟用行銷活動。

## 建立您的廣告 {#create-your-ad}

設定好方案和促銷活動后，建立新廣告。

1. 去通道;例如，LinkedIn或臉書。
1. 建立新廣告。
1. 選取Marketo登陸頁面，作為行銷活動中行動號召的目的地。
1. 將查詢字串新增至URL。

   >[!NOTE]
   >
   >**範例**
   >
   >下面介紹了如何將您設置的所有資訊添加到實際URL中。 項目之間以 &amp; 符號 （&amp;） 分隔：
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **來源**&#x200B;是作為管道識別碼使用的Person Source
   >* **註解**&#x200B;是為每個方案建立的唯一識別碼
   >* **camp**&#x200B;是Facebook、LinkedIn或Google中的行銷活動
   >* **kk**&#x200B;是您要擷取的關鍵字或資產名稱
   >
   >**這四個字詞必須全部小寫，且URL中不能有任何空格可供擷取此資訊。**

## 最佳實務 {#best-practices}

使用單個通道 標記來表示所有數字廣告，或者如果您希望與其他行銷管道（例如，Social付費、Search付費、展示廣告、重定向）進行更精細的比較，請使用多個通道標籤。

然後，為您需要的每個報告 視圖設置不同的程序。 如果您有 10 個區域同時啟動“大Campaign”，並希望能夠跨區域視圖結果，請使用通用 ID 作為查詢字串中URL（例如 BC）中的參數。

如果您想報告每個區域和大Campaign的集體結果，請創建 11 個程序 - 每個區域一個，一個用於大Campaign。 每個方案僅引用查詢字串中的相關字元（例如 BC）。

Big Campaign 和 區域 計劃之間的人員數量有意重疊，因此您不想報告所有 11 個計劃的總人數，因為有些人同時在 Big Campaign 和其中一個區域計劃中。
