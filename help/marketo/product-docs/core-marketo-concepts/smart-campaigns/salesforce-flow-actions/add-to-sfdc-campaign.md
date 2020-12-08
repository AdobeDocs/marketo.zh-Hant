---
unique-page-id: 1147034
description: 添加到SFDC Campaign —— 行銷人員文檔——產品文檔
title: 添加到SFDC促銷活動
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# 添加到SFDC促銷活動 {#add-to-sfdc-campaign}

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>僅在與Salesforce整合時提供。

## 概觀 {#overview}

此流程步驟可用於Marketo促銷活動，或作為單一流程步驟，將人員新增為Salesforce促銷活動中的客源。 如果Salesforce中尚未存在銷售線索，則會自動同步銷售線索，並以指定狀態新增至促銷活動。

![](assets/image2014-9-22-15-3a43-3a36.png)

## 使用狀況 {#usage}

1. 尋找並選取您要新增銷售機會的Salesforce促銷活動。

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >如果您在「促銷活動」清單中看不到Salesforce促銷活動：
   >
   >    
   >    
   >    1. 請確定促銷 [活動同步已啟用](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)。
   >    1. 確認您的 [Marketo Sync使用者是](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) Salesforce [中的Marketing使用者](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) 。


   >[!TIP]
   >
   >您可以使用Salesforce促銷活動 [「我的代號](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) 」，讓程式仿製更輕鬆。

1. 選擇要在新增銷售線索時指派給銷售線索的Salesforce促銷活動成員狀態。

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >如果某人已是Salesforce促銷活動的主要成員，則會略過該人員，且不會更新其狀態。 您可以改 [用更改SFDC促銷活動中的狀態](change-status-in-sfdc-campaign.md) 。

