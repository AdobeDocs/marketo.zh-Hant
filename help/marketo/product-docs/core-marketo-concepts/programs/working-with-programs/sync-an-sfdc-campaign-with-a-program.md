---
unique-page-id: 1147154
description: 將SFDC促銷活動與程式同步 — Marketo檔案 — 產品檔案
title: 將SFDC促銷活動與程式同步
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 將SFDC促銷活動與程式同步 {#sync-an-sfdc-campaign-with-a-program}

Marketo可讓您將方案與Salesforce行銷活動同步，以維護兩個系統中的相同人員清單，包括其狀態。 讓我們開始吧！

>[!PREREQUISITES]
>
>您將需要 [啟用Salesforce促銷活動同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) 第一。

>[!CAUTION]
>
>將SFDC促銷活動與Marketo方案同步時，針對方案的子促銷活動，隱含的SFDC動作（例如，新增至SFDC促銷活動、同步至SFDC）將會停用。

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-1.png)

1. 選取您的程式。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 按一下 **程式動作**，然後選取 **Salesforce Campaign同步**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. 選取 **新建** 或選擇現有的Salesforce行銷活動。

   >[!TIP]
   >
   >如果您選取現有的Salesforce行銷活動，請確定 [比對Salesforce行銷活動和Marketo方案的方案狀態](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. 輸入新行銷活動的名稱，然後按一下 **儲存**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. 現在您可以在方案摘要頁面中驗證Campaign同步處理詳細資料。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   太好了！ 現在，Marketo中的任何方案狀態變更都會同步至SFDC行銷活動，反之亦然。
