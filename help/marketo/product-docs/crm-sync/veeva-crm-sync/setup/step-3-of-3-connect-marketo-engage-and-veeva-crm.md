---
description: 步驟3之3 — 連線Marketo Engage與 [!DNL Veeva] CRM - Marketo檔案 — 產品檔案
title: 步驟3之3 — 連線Marketo Engage和 [!DNL Veeva] CRM
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 1%

---

# 步驟3之3：連線Marketo Engage和[!DNL Veeva] CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

在本文中，您將設定Marketo Engage以與您設定的[!DNL Veeva] CRM執行個體同步。 **您會在部分快顯視窗中看到[!DNL Salesforce]**，因為[!DNL Veeva] CRM是建置在[!DNL Salesforce]平台上。

>[!PREREQUISITES]
>
>* [步驟3之1：將Marketo欄位新增至 [!DNL Veeva]](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [步驟2之3：建立Marketo的 [!DNL Veeva] 使用者](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>一次只能有一個Marketo執行個體連線至[!DNL Veeva] CRM執行個體。

## 使用OAuth連線至[!DNL Veeva] CRM {#connect-to-veeva-crm-using-oauth}

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。 選取&#x200B;**[!UICONTROL CRM]**&#x200B;並按一下&#x200B;**[!UICONTROL Sync with Veeva]**。

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >在按一下[同步欄位]之前，請務必[隱藏Marketo中不需要的所有欄位](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"}，不讓同步使用者看到。 按一下「同步欄位」後，使用者看見的所有欄位將會在Marketo中永久建立，且無法刪除。

1. 按一下「**[!UICONTROL Login with Veeva]**」。

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >如果您正在將Marketo沙箱同步至[!UICONTROL Sandbox] CRM沙箱，請核取[!DNL Veeva]。

1. 按一下「**[!UICONTROL Confirm Credentials]**」。

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. 將會顯示包含[!DNL Salesforce]登入頁面的快顯視窗。 輸入您的「Marketo同步使用者」認證，然後按一下&#x200B;**[!UICONTROL Log In]**。

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. 輸入您透過電子郵件（由[!DNL Salesforce]傳送）收到的驗證碼，然後按一下&#x200B;**[!UICONTROL Verify]**。

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. 在成功驗證後，存取頁面將會顯示以請求存取。 按一下「**[!UICONTROL Allow]**」。

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. 幾分鐘後，Marketo Engae中將會顯示快顯視窗。 按一下「**[!UICONTROL Confirm Credentials]**」。

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## 開始[!DNL Veeva]同步 {#start-veeva-sync}

1. 按一下&#x200B;**[!UICONTROL Start Veeva Sync]**&#x200B;開始持續性[!DNL Marketo-Veeva] CRM同步處理。

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo不會針對[!DNL Veeva] CRM同步處理或手動輸入潛在客戶時，自動進行重複資料刪除。

1. 按一下「**[!UICONTROL Start Sync]**」。

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>完成初始同步的時間會因資料庫的大小和複雜度而有所不同。

## 驗證同步 {#verify-sync}

Marketo在管理區域中提供[!DNL Veeva] CRM同步的狀態訊息。 您可以按照以下步驟驗證同步是否正常運作。

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**，然後按&#x200B;**[!UICONTROL Veeva]**。

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. 同步狀態會顯示在右上角。 它會顯示下列三個訊息之一：上次同步、同步進行中或失敗。

>[!MORELIKETHIS]
>
>[設定自訂物件](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
