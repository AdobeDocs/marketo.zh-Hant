---
unique-page-id: 1147154
description: 將SFDC促銷活動與計畫同步 — Marketo檔案 — 產品檔案
title: 將SFDC促銷活動與計畫同步
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
source-git-commit: 8781c6cf2e64543809fe697e75ae6884969a4e40
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 將SFDC促銷活動與計畫同步 {#sync-an-sfdc-campaign-with-a-program}

Marketo可讓您將方案與Salesforce促銷活動同步，以維護兩個系統中相同的人員清單，包括其狀態。 開始吧！

>[!PREREQUISITES]
>
>您需要 [啟用Salesforce促銷活動同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) 第一個。

>[!CAUTION]
>
>將SFDC促銷活動與Marketo計畫同步時，該計畫的子促銷活動將禁用隱含的SFDC操作（例如，添加到SFDC促銷活動，同步到SFDC）。

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-1.png)

1. 選取您的方案。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 按一下 **計畫操作**，然後選取 **Salesforce促銷活動同步**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. 選擇 **新建** 或選擇現有的Salesforce促銷活動。

   >[!TIP]
   >
   >如果您選取現有的Salesforce促銷活動，請務必 [匹配Salesforce促銷活動和Marketo計畫的方案狀態](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. 輸入新促銷活動的名稱，然後按一下 **儲存**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. 現在，您可以在方案摘要頁面中驗證促銷活動同步詳細資訊。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   太棒了！ 現在，Marketo中的任何計畫狀態變更都會同步至SFDC促銷活動，反之亦然。
