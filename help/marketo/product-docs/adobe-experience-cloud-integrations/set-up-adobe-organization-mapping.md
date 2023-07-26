---
unique-page-id: 42762511
description: 設定Adobe組織對應 — Marketo檔案 — 產品檔案
title: 設定Adobe組織對應
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# 設定Adobe組織對應 {#set-up-adobe-organization-mapping}

為了與Adobe應用程式(例如Audience Manager)、B2B CDP Marketo聯結器、 [!DNL Dynamic Chat]等等。您必須先在Marketo中輸入Adobe IMS組織憑證。

>[!NOTE]
>
>Marketo執行個體的HIPAA就緒部署無法使用此整合。

>[!CAUTION]
>
>對於加入Adobe Business Platform和Identity Management系統的客戶，與訂閱相關聯的組織ID將會填入，且是唯讀欄位。

1. 在Marketo中，按一下 **[!UICONTROL 管理員]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. 在整合底下，按一下 **[!UICONTROL Adobe組織對應]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. 按一下 **[!UICONTROL 編輯]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. 輸入您的Adobe IMS組織ID (瞭解如何找到 [此處](https://experienceleague.adobe.com/docs/control-panel/using/faq.html){target="_blank"})並按一下 **[!UICONTROL 確定]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. 按一下 **[!UICONTROL 確認]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. 按一下 **[!UICONTROL 關閉]**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >基於安全考量，您必須是您要對應之Adobe組織的組織管理員。 否則，動作將會失敗。 此外，Adobe使用者和Marketo使用者在登入時必須使用相同的電子郵件地址。

1. 如果您是 _非_ 已經登入，快顯視窗會出現在新的標籤/視窗中。 登入您的Adobe組織（此動作會驗證組織存取權）。

就是這樣！ 您現在可以 [共用受眾資料](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} to, or [sync an audience](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} 來自Adobe Experience Cloud。
