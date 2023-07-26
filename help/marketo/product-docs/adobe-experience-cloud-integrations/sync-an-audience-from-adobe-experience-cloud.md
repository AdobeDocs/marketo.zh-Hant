---
description: 從Adobe Experience Cloud同步受眾 — Marketo檔案 — 產品檔案
title: 從Adobe Experience Cloud同步對象
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
feature: Integrations
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 從Adobe Experience Cloud同步對象 {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Marketo執行個體的HIPAA就緒部署無法使用此整合。

>[!PREREQUISITES]
>
>[設定Adobe組織對應](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## 如何同步受眾 {#how-to-sync-an-audience}

1. 在「我的Marketo」中，按一下 **[!UICONTROL 資料庫]** 圖磚。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. 按一下 **[!UICONTROL 新增]** 下拉式清單並選取 **[!UICONTROL 從Experience Cloud對象同步]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. 按一下 **[!UICONTROL 對象庫資料夾]** 下拉式清單，然後選取所需的原始資料夾。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. 選取 **[!UICONTROL 對象名稱]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. 您可以針對目的地選取現有清單，或輸入新清單的名稱。 在此範例中，我們正在建立新範本。 按一下 **[!UICONTROL 同步]** 完成時。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. 按一下 **[!UICONTROL 確定]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## 常見問題集 {#faq}

**Cookie同步如何運作？**

為您的Marketo訂閱啟用Cookie同步後，Marketo的munchkin.js將嘗試為您在整合設定期間指定的Adobe IMS組織擷取和儲存AdobeECID，並將這些ECID比對至對應的Marketo Cookie識別碼。 這可讓Marketo的匿名使用者設定檔更加豐富AdobeECID。

還需要進一步步驟，將匿名使用者設定檔與潛在客戶設定檔建立關聯（使用純文字電子郵件識別）。 此功能的確切運作方式 [此處說明](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Marketo中的清單大小為何與Adobe中的清單大小不同？**

如果我們無法將ECID Cookie ID繫結至Marketo中的已知人員，人員也不會同步處理。

**這是一次性同步嗎？**

您只需要起始同步處理一次。 之後，記錄會自動同步。 初始同步最多可能需要24小時；以後，新記錄將在2-3小時內同步。
