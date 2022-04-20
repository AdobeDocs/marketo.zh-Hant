---
description: 同步來自Adobe Experience Cloud的受眾 — Marketo文檔 — 產品文檔
title: 同步來自Adobe Experience Cloud的受眾
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
source-git-commit: 86451f1027e74479a415a4c6654a2625275d4112
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 同步來自Adobe Experience Cloud的受眾 {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Marketo實例的HIPAA就緒部署無法使用此整合。

>[!PREREQUISITES]
>
>[設定Adobe組織映射](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-organization-mapping.md)

## 如何同步受眾 {#how-to-sync-an-audience}

1. 在「我的Marketo」中，按一下 **資料庫** 平鋪。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. 按一下 **新建** 下拉並選擇 **從Experience Cloud受眾同步**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. 按一下 **訪問群體庫資料夾** 下拉並選擇所需的原始資料夾。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. 選擇 **受眾名稱**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. 對於目標，可以選擇現有清單，或鍵入新清單的名稱。 在這個例子中，我們正在建立一個新的。 按一下 **同步** 完成。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. 按一下 **確定**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## 常見問題 {#faq}

**Cookie同步如何工作？**

為您的Marketo訂閱啟用cookie同步後，Marketo的munchkin.js將嘗試捕獲和儲存在整合設定期間指定的Adobe IMS組織的AdobeECID，並將這些ECID與相應的Marketocookie標識符匹配。 這使Marketo的匿名用戶配置檔案能夠用AdobeECID豐富。

還需要進一步步驟將匿名用戶配置檔案與使用純文字檔案電子郵件標識的潛在客戶配置檔案相關聯。 這是如何運作的 [此處描述](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md)。

**為什麼Marketo的名單大小與Adobe的名單大小不同？**

如果我們無法將ECIDcookie ID與Marketo的已知人綁定，則用戶也不會同步。

**這是一次性同步嗎？**

您只需啟動一次同步。 之後，記錄將自動同步。 初始同步最多需要24小時；今後，新記錄將在2-3小時內同步。
