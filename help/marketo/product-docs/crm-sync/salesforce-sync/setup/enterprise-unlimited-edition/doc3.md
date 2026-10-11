---
description: 瞭解如何在最終的Enterprise或Unlimited步驟中連線Marketo和Salesforce。 擷取同步處理使用者安全性權杖，並在Marketo管理中設定認證。
title: 步驟3之3 — 連線Marketo和Salesforce (Enterprise/Unlimited)
hide: true
hidefromtoc: 'yes'
feature: Salesforce Integration
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 8%
---
# 第 3 步 (共 3 步)：連接 Marketo 和 Salesforce (企業版/無限版) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

在本文中，您將設定Marketo Engage以與已設定的Salesforce執行個體同步。

>[!PREREQUISITES]
>
>* [步驟3之1：將Marketo欄位新增至Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [步驟2之3：建立Marketo (Enterprise/Unlimited)的Salesforce使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}

## 擷取同步處理使用者安全性權杖 {#retrieve-sync-user-security-token}

>[!TIP]
>
>如果您已經有安全性權杖，請直接進入「設定同步使用者認證」和「稱號」進行準備！

1. 以Marketo Sync User登入Salesforce，按一下同步使用者名稱，然後按&#x200B;**[!UICONTROL My Settings]**。
