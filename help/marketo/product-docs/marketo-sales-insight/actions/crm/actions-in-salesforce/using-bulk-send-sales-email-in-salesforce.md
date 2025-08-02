---
description: 在Salesforce中使用大量傳送銷售電子郵件 — Marketo檔案 — 產品檔案
title: 在Salesforce中使用大量傳送銷售電子郵件
exl-id: 4886109d-c2b8-4186-922b-8a15cf1e742e
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---

# 在Salesforce中使用大量傳送銷售電子郵件 {#using-bulk-send-sales-email-in-salesforce}

瞭解如何在Salesforce中傳送大量電子郵件，以使用銷售動作協助擴展您的傳出通訊。

>[!NOTE]
>
>Salesforce強制限制200筆可一次選取的記錄。

>[!PREREQUISITES]
>
>請確定您已將[最新Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}安裝至您的Salesforce執行個體，並在Salesforce的連絡人和潛在客戶清單檢視上設定了[動作按鈕](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/add-action-buttons-to-salesforce-list-view.md){target="_blank"}。

## 在Salesforce Lightning中傳送大量電子郵件 {#sending-bulk-email-in-salesforce-lightning}

1. 在Salesforce中，按一下&#x200B;**銷售機會/聯絡人**&#x200B;索引標籤，以瀏覽至「銷售機會/聯絡人」首頁。

   ![](assets/using-bulk-send-sales-email-in-salesforce-1.png)

1. 在「檢視」下拉式清單中，選取您要以電子郵件傳送的潛在客戶/聯絡人檢視。

   >[!TIP]
   >
   >您可以按一下右側的齒輪圖示並選取&#x200B;**新增**，以建立新的檢視。 當您為檢視提供新名稱並儲存後，可以按一下右側的篩選圖示，以協助篩選至您要傳送電子郵件的潛在客戶/聯絡人集合。

1. 選擇所需的潛在客戶或連絡人清單，然後按一下&#x200B;**傳送銷售電子郵件**&#x200B;按鈕。

   ![](assets/using-bulk-send-sales-email-in-salesforce-2.png)

1. 系統會將您導覽至「動作撰寫」視窗，並新增您選取的人員。

1. 選取您要插入至「動作」撰寫視窗編輯器中的範本，或撰寫自訂電子郵件。

   >[!TIP]
   >
   >使用[固定類別](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"}讓您更輕鬆地存取您最愛的電子郵件範本。

   **選擇性步驟**：按一下&#x200B;**預覽動態欄位**&#x200B;按鈕，預覽任何動態欄位個人化。

   >[!TIP]
   >
   >如果您想要自訂所有收件者的範本，按一下大量撰寫側邊欄中的所有收件者選項，可讓您同時編輯所有收件者電子郵件。 如果您想要變更特定電子郵件，請在「大量撰寫」側邊欄中按一下收件者名稱或電子郵件。 請注意，如果您在選取「所有收件者」時，對個別電子郵件進行變更，然後進行變更，則對「所有收件者」所做的變更將會覆寫對個別電子郵件所做的變更。

1. 選取&#x200B;**傳送**&#x200B;以立即傳送電子郵件，或選取&#x200B;**設定排程**&#x200B;以設定傳送電子郵件的日期和時間。

   ![](assets/using-bulk-send-sales-email-in-salesforce-3.png)

## 在Salesforce Classic中傳送大量電子郵件 {#sending-bulk-email-in-salesforce-classic}

1. 在Salesforce中，按一下&#x200B;**銷售機會/聯絡人**&#x200B;標籤。

1. 在[檢視]下拉式清單中，選取想要的要傳送電子郵件的潛在客戶/連絡人檢視，然後按一下[執行]。****

   ![](assets/using-bulk-send-sales-email-in-salesforce-4.png)

   >[!TIP]
   >
   >您可以按一下「建立新檢視」並設定可用的篩選器，以縮小您要新增至促銷活動的使用者清單，藉此建立新檢視。

1. 選擇所需的潛在客戶或連絡人清單，然後按一下&#x200B;**傳送銷售電子郵件**&#x200B;按鈕。

   ![](assets/using-bulk-send-sales-email-in-salesforce-5.png)

1. 系統會將您導覽至動作撰寫視窗，其中包含您在撰寫視窗中選取的收件者。

1. 選取您要插入至「動作」撰寫視窗編輯器的範本，或撰寫自訂電子郵件。

   ![](assets/using-bulk-send-sales-email-in-salesforce-6.png)

   >[!TIP]
   >
   >使用[固定類別](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"}讓您更輕鬆地存取您最愛的電子郵件範本。

   **選擇性步驟**：按一下&#x200B;**預覽動態欄位**&#x200B;按鈕，預覽任何動態欄位個人化。

   >[!TIP]
   >
   >如果您想要自訂所有收件者的範本，按一下大量撰寫側邊欄中的所有收件者選項，可讓您同時編輯所有收件者電子郵件。 如果您想要變更特定電子郵件，請在「大量撰寫」側邊欄中按一下收件者名稱或電子郵件。 請注意，如果您在選取「所有收件者」時，對個別電子郵件進行變更，然後進行變更，則對「所有收件者」所做的變更將會覆寫對個別電子郵件所做的變更。

1. 選取&#x200B;**傳送**&#x200B;以立即傳送電子郵件，或選取&#x200B;**設定排程**&#x200B;以設定傳送電子郵件的日期和時間。
