---
unique-page-id: 1147034
description: 新增至SFDC Campaign - Marketo檔案 — 產品檔案
title: 添加到SFDC促銷活動
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# 添加到SFDC促銷活動 {#add-to-sfdc-campaign}

>[!NOTE]
>
>僅在與Salesforce整合時可用。

## 總覽 {#overview}

此流程步驟可用於Marketo促銷活動，或作為單一流程步驟，將人員新增為Salesforce促銷活動中的銷售機會。 如果Salesforce中尚未存在銷售機會，則會自動將其同步至具有指定狀態的促銷活動。

![](assets/image2014-9-22-15-3a43-3a36.png)

## 使用情況 {#usage}

1. 尋找並選取您要新增銷售機會的Salesforce促銷活動。

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >如果您在促銷活動清單中看不到Salesforce促銷活動：
   >
   >  1. 請確定 [促銷活動同步已啟用](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >  1. 確認您的 [Marketo同步使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 是 [行銷使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) 在Salesforce。


   >[!TIP]
   >
   >您可以使用Salesforce促銷活動 [我的代號](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) 使程式克隆更容易。

1. 選擇添加銷售線索時要分配給銷售線索的Salesforce促銷活動成員狀態。

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >如果人員已是Salesforce促銷活動的主要成員，則會略過該人員，且其狀態不會更新。 您可以使用 [在SFDC活動中更改其狀態](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md) 。
