---
unique-page-id: 1147034
description: 新增至SFDC Campaign - Marketo檔案 — 產品檔案
title: 新增至SFDC Campaign
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 新增至SFDC Campaign {#add-to-sfdc-campaign}

此流程步驟可用於Marketo Engage行銷活動，或作為單一流程步驟，在Salesforce行銷活動中新增人員作為銷售機會。 如果Salesforce中尚未存在潛在客戶，則會自動將其同步並新增至具有指定狀態的促銷活動。

>[!NOTE]
>
>僅在與Salesforce整合時可用。

![](assets/add-to-sfdc-campaign-1.png)

## 使用量 {#usage}

1. 尋找並選取您要新增銷售機會的Salesforce行銷活動。

   ![](assets/add-to-sfdc-campaign-2.png)

   >[!TIP]
   >
   >如果在行銷活動清單中看不到Salesforce行銷活動：
   >
   >  1. 確定已啟用[行銷活動同步處理](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}。
   >  1. 確認您的[Marketo同步使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}是Salesforce中的[行銷使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}。

   >[!TIP]
   >
   >您可以使用Salesforce促銷活動[My Token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}，讓程式複製更容易。

1. 選取在新增潛在客戶時，您想要指派的Salesforce促銷活動成員狀態。

   ![](assets/add-to-sfdc-campaign-3.png)

   >[!CAUTION]
   >
   >如果人員已經是Salesforce促銷活動的主要成員，則將略過這些人員且其狀態不會更新。 您可以改用[在SFDC行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}中變更其狀態。
