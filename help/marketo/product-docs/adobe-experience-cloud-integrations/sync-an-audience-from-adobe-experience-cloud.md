---
description: 瞭解如何將受眾從Adobe Experience Cloud同步至Marketo Engage。 將對象從對象庫提取到Marketo資料庫，以用於行銷活動和方案。
title: 從 Adobe Experience Cloud 同步客群
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
feature: Integrations
TQID: https://experienceleague.adobe.com/XCskpUNcNae-ikOLXxREb4kePbFs9HRheIihzJqHKoU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 8%

---

# 從 Adobe Experience Cloud 同步客群 {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Marketo執行個體的HIPAA就緒部署無法使用此整合。

>[!PREREQUISITES]
>
>[設定Adobe組織對應](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## 如何同步受眾 {#how-to-sync-an-audience}

1. 在「我的Marketo」中，按一下「**[!UICONTROL Database]**」圖磚。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. 按一下「**[!UICONTROL New]**」下拉式選單，選取「**[!UICONTROL Sync from Experience Cloud Audience]**」。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. 按一下&#x200B;**[!UICONTROL Audience Library Folder]**&#x200B;下拉式清單，然後選取所需的原始資料夾。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. 選取&#x200B;**[!UICONTROL Audience Name]**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. 您可以針對目的地選取現有清單，或輸入新清單的名稱。 在此範例中，正在建立新清單。 完成後請按一下 **[!UICONTROL Sync]**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. 按一下「**[!UICONTROL OK]**」。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## 常見問題集 {#faq}

**Cookie同步如何運作？**

為您的Marketo訂閱啟用Cookie同步後，Marketo的munchkin.js會嘗試針對您在整合設定期間指定的Adobe IMS組織擷取和儲存Adobe ECID，並將這些ECID比對至對應的Marketo Cookie識別碼。 這可讓Marketo的匿名使用者設定檔更加豐富Adobe ECID。

還需要進一步步驟，將匿名使用者設定檔與潛在客戶設定檔建立關聯（使用純文字電子郵件識別）。 [在此說明](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}的運作方式。

**為什麼Marketo中的清單大小與Adobe中的清單大小不同？**

如果ECID Cookie ID無法繫結至Marketo中的已知人員，則人員也不會進行同步處理。

**這是一次性同步嗎？**

您只需要起始同步處理一次。 之後，記錄會自動同步。 初始同步最多可能需要24小時；以後，新記錄將在2-3小時內同步。
