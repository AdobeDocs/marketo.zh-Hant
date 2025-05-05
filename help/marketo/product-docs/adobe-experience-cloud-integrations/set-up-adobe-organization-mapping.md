---
unique-page-id: 42762511
description: 設定Adobe組織對應 — Marketo檔案 — 產品檔案
title: 設定Adobe組織對應
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# 設定Adobe組織對應 {#set-up-adobe-organization-mapping}

若要與Adobe應用程式(例如Audience Manager、B2B CDP Marketo聯結器、[!DNL Dynamic Chat]等)同步，您必須先以Marketo Engage輸入您的Adobe IMS組織認證。

>[!NOTE]
>
>* Marketo執行個體的HIPAA就緒部署無法使用此整合。
>* 為了讓整合發揮作用，Marketo和您的其他Adobe應用程式必須位於相同組織。

>[!IMPORTANT]
>
>對於已上線至Adobe Business Platform和Identity Management System的使用者，將會填入與訂閱相關聯的組織ID，且為唯讀欄位。 因此，本文中的步驟不適用。

1. 在Marketo中，按一下&#x200B;**[!UICONTROL 管理員]**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. 在整合下，按一下&#x200B;**[!UICONTROL Adobe組織對應]**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. 按一下&#x200B;**[!UICONTROL 編輯]**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. 輸入您的Adobe IMS組織ID （瞭解如何在[這裡](https://experienceleague.adobe.com/docs/control-panel/using/faq.html?lang=zh-Hant){target="_blank"}找到該ID），然後按一下&#x200B;**[!UICONTROL 確定]**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. 按一下&#x200B;**[!UICONTROL 確認]**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. 按一下 **[!UICONTROL 關閉]**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >基於安全考量，您必須是您要對應之Adobe組織的組織管理員。 否則，動作將會失敗。 此外，Adobe使用者和Marketo使用者在登入時必須使用相同的電子郵件地址。

1. 如果您&#x200B;_尚未_&#x200B;登入，新的索引標籤/視窗中將會出現快顯視窗。 登入您的Adobe組織（此動作會驗證組織存取權）。

就是這樣！ 您現在可以[與共用對象資料](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"}，或從Adobe Experience Cloud同步對象[&#128279;](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"}。
