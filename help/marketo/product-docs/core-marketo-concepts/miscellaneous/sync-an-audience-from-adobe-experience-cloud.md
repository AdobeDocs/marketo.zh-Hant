---
description: 從Adobe Experience Cloud同步觀眾——行銷人員檔案——產品檔案
title: 從Adobe Experience Cloud同步觀眾
translation-type: tm+mt
source-git-commit: 05c2e89222f9316241a3929642998bddb02ff7a5
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---


# 從Adobe Experience Cloud同步觀眾{#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Marketo例項的HIPAA適用部署無法使用此整合。

>[!PREREQUISITES]
>
>[設定Adobe Experience Cloud觀眾分享](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## 如何同步對象{#how-to-sync-an-audience}

1. 在My Marketo中，按一下&#x200B;**Database**&#x200B;表徵圖。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. 按一下「**新增**」下拉式清單，然後選取「從Experience Cloud對象&#x200B;**同步」。**

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. 按一下「**觀眾程式庫資料夾**」下拉式清單，並選取所要的來源資料夾。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. 選取&#x200B;**對象名稱**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. 對於目標，可以選擇現有清單，或鍵入新清單的名稱。 在此範例中，我們正在建立新的範例。 完成時，按一下&#x200B;**Sync**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. 按一下&#x200B;**確定**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## 常見問答{#faq}

**Cookie如何同步？**

當您的Marketo訂閱啟用Cookie同步時，Marketo的munchkin.js會嘗試擷取並儲存您在整合設定期間指定之AdobeIMS組織的AdobeECID，並將這些ECID與對應的Marketo Cookie識別碼相符。 這可讓Marketo的匿名使用者個人檔案更豐富地使用AdobeECID。

需要進一步步驟，將匿名用戶配置檔案與使用純文字檔案電子郵件標識的銷售線索配置檔案關聯。 此處說明[的運作方式。](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md)

**為什麼Marketo中的清單大小與Adobe中的清單大小不同？**

如果我們無法將ECID Cookie ID系結至Marketo中的已知人員，使用者也不會同步。

**這是一次性同步嗎？**

您只需啟動一次同步。 之後，記錄將自動同步。 初始同步最多需要24小時；今後，新記錄將在2-3小時內同步。
