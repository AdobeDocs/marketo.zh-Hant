---
unique-page-id: 2359418
description: 匯入人員清單 — Marketo檔案 — 產品檔案
title: 匯入人員清單
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
feature: Getting Started
source-git-commit: 1676c9049c61a637faede4751ea49bbcfa018be5
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# 匯入人員清單 {#import-a-list-of-people}

## 任務：將貿易展覽會出席者的試算表清單匯入您的資料庫 {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[設定並新增人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

在本教學課程中，您將瞭解如何從試算表檔案將人員匯入Marketo。

## 步驟1：下載並編輯試算表 {#step-download-and-edit-a-spreadsheet}

1. 若要開始，請將我們的實務試算表檔案([**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"})下載到您的電腦。

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >匯入日期時，請使用此格式： **9/21/20** （月/日/年）。

   >[!NOTE]
   >
   >匯入的任何日期/時間欄位都會視為中央時間。 如果您的日期/時間欄位位於不同的時區，可以使用Excel公式將其轉換為中部時間（美洲/芝加哥）。

1. 新增您自己的名字、姓氏、實際電子郵件地址（以便接收下次任務時將會傳送的培養電子郵件）以及職稱。 將檔案儲存在電腦上。

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >* 請確定電子郵件地址只包含ASCII字元。
   >
   >* Marketo **不**&#x200B;支援包含emoji的電子郵件地址。
   >
   >* 透過CSV匯入`NULL`值，可能會為人員[活動記錄](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"}、_中的數值欄位產生「變更資料值」，即使欄位已經空白_。 如果您有使用「資料值已變更」篩選器或「資料值變更」觸發器的任何[智慧行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target="_blank"}，請務必使用[限制](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"}，以確保在執行匯入時不會不必要地觸發這些限制。

## 步驟2：建立方案 {#step-create-a-program}

1. 前往&#x200B;**[!UICONTROL 行銷活動]**&#x200B;區域。

   ![](assets/import-a-list-of-people-3.png)

1. 選取您的&#x200B;**學習**&#x200B;資料夾，然後在&#x200B;**[!UICONTROL 新增]**&#x200B;下按一下&#x200B;**[!UICONTROL 新增程式]**。

   ![](assets/import-a-list-of-people-4.png)

1. **命名**&#x200B;程式「我的商展程式」並為&#x200B;**[!UICONTROL 程式型別]**&#x200B;選取「事件」。

   ![](assets/import-a-list-of-people-5.png)

1. 選取&#x200B;**[!UICONTROL 頻道]**&#x200B;的&#x200B;**[!UICONTROL 商展]**，然後按一下&#x200B;**[!UICONTROL 建立]**。

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>事件程式會在特定日期發生。 深入瞭解&#x200B;[**活動**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}。

## 步驟3：將試算表匯入Marketo {#step-import-your-spreadsheet-into-marketo}

1. 在&#x200B;**我的商展計畫**&#x200B;中，按一下&#x200B;**[!UICONTROL 新增]**，然後選取&#x200B;**[!UICONTROL 新增本機資產]**。

   ![](assets/import-a-list-of-people-7.png)

1. 選取&#x200B;**[!UICONTROL 清單]**。

   ![](assets/import-a-list-of-people-8.png)

1. **命名**「商展與會者」清單，然後按一下&#x200B;**[!UICONTROL 建立]**。

   ![](assets/import-a-list-of-people-9.png)

1. 在您的&#x200B;**[!UICONTROL 商展與會者]**&#x200B;清單中，按一下&#x200B;**[!UICONTROL 清單動作]**&#x200B;並選取&#x200B;**[!UICONTROL 匯入清單]**。

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >如果您使用自己的CSV檔案，請確定該檔案編碼為UTF-8、UTF-16、Shift-JIS或EUC-JP。

   >[!NOTE]
   >
   >CSV檔案的大小限製為100MB。

1. **[!UICONTROL 瀏覽]**&#x200B;至您電腦上的&#x200B;**tradeshow-attendees.csv**&#x200B;試算表檔案，然後按一下&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >在[清單匯入模式]中，選擇&#x200B;**[!UICONTROL 略過新人員與更新]**&#x200B;表示您不會影響現有的人員記錄或記錄任何活動。 如果您想要在行銷活動中使用的快速預先篩選現有人員的靜態清單，請使用此模式。 選取此模式將：
   >
   > * 略過建立新人員
   > * 略過人員欄位更新
   > * 略過活動記錄

1. 將您的[!UICONTROL 清單資料行]欄位對應到它們各自的Marketo欄位，然後按一下&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >欄標題應始終完全符合欄位（區分大小寫），以獲得最佳自動對應結果。 如果您使用自訂欄位，但未在下拉式清單中看到它們，請返回[建立它們](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}，讓它們成為選項。

   >[!NOTE]
   >
   >如果有任何您不想匯入的欄位，請在Marketo欄位下拉式選單中選取&#x200B;**忽略**。

1. 為&#x200B;**[!UICONTROL 贏取方案]**&#x200B;選取&#x200B;**我的商展方案**，然後按一下&#x200B;**[!UICONTROL 匯入]**。

   ![](assets/import-a-list-of-people-13.png)

1. 等候您的人員匯入，然後關閉匯入進度快顯功能表。

   ![](assets/import-a-list-of-people-14.png)

1. 返回&#x200B;**我的商展方案**，按一下&#x200B;**[!UICONTROL 成員]**&#x200B;標籤。 您會看到剛才匯入的所有人員。

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>您可以透過追蹤計畫會員資格來分析計畫的成功。 深入瞭解&#x200B;[**程式**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}。

## 任務完成 {#mission-complete}

您的商展與會者現在是Marketo計畫的成員！

<br> 

[◄任務4：電子郵件自動回應](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[任務6：滴水、滴水、Nurture ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
