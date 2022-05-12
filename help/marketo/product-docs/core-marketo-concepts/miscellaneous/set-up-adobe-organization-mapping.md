---
unique-page-id: 42762511
description: 設定Adobe組織映射 — Marketo文檔 — 產品文檔
title: 設定Adobe組織映射
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: bbe5f4a1502ab79d0081807ea6aab196ae75360a
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# 設定Adobe組織映射 {#set-up-adobe-organization-mapping}

為了與Adobe應用程式(如Audience Manager、B2B CDPMarketo連接器、動態聊天等)同步，您必須首先在Marketo輸入Adobe IMS組織憑據。

>[!NOTE]
>
>Marketo實例的HIPAA就緒部署無法使用此整合。

>[!CAUTION]
>
>對於已掛接到Adobe業務平台和Identity Management系統的客戶，與訂閱關聯的組織ID將已填充，並且是只讀欄位。

1. 在Marketo，按一下 **管理**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. 在整合下，按一下 **Adobe組織映射**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. 按一下 **編輯**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. 輸入Adobe IMS組織ID(瞭解如何查找 [這裡](https://experienceleague.adobe.com/docs/control-panel/using/faq.html)) **確定**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. 按一下 **確認**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. 按一下 **關閉**。

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >出於安全原因，您必須是要映射到的Adobe組織的組織管理員。 如果你沒有，那麼行動將失敗。 此外，Adobe用戶和Marketo用戶登錄時必須使用相同的電子郵件地址。

1. 如果你 _不_ 已登錄，彈出窗口將出現在新的頁籤/窗口中。 登錄到Adobe組織（此操作驗證組織訪問權限）。

就這樣！ 你現在可以 [共用受眾資料](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target=&quot;_blank&quot;到或 [同步受眾](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/sync-an-audience-from-adobe-experience-cloud.md)來自Adobe Experience Cloud的{target=&quot;_blank&quot;}。
