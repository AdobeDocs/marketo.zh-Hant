---
description: Salesforce中的MSI操作配置 — Marketo文檔 — 產品文檔
title: MSI Actions Configuration in Salesforce
hide: true
hidefromtoc: true
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 84e3c4d525c5bde9e3ebd17d2f29ad42578777ff
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Salesforce中的MSI操作配置 {#msi-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [安裝]() 或 [升級]() Salesforce實例中的Sales Insight包安裝/升級到 [MSI操作包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) 在Salesforce實例中。
>* [在Salesforce Enterprise/Unlimited中配置MarketoSales Insight]()


## 在Salesforce中添加新遠程站點 {#add-new-remote-site-in-salesforce}

1. In Salesforce, click **Setup**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. 搜索「遠程站點」並選擇 **遠程站點設定**。
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. 按一下 **新建遠程站點**。

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. 輸入遠程站點名稱（它可能類似於「MarketoSalesInsight」）。 Enter the Remote Site URL (https://ims-na1-stg1.adobelogin.com) and click **Save**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

## 在CRM中啟用MSI操作 {#enabling-msi-actions-across-the-crm}

1. In Salesforce, click the **Marketo Sales Insight Config** tab.

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >If you don&#39;t see &quot;Marketo Sales Insight Config&quot; in your top bar, click the **+** sign and find it under All Tabs.

1. 選擇 **啟用MSI操作** 複選框。

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. 輸入API密鑰。

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >如果您的API密鑰不方便使用，您可以按照中的步驟找到它 [這篇文章](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)。

1. 按一下 **保存** 完成。

This will automatically enable all MSI Actions features outlined in the feature overview article.

>[!NOTE]
>
>You can disable all MSI Actions features by simply unchecking the “Enable MSI Actions” checkbox.

## MSI-Actions治理 {#msi-actions-governance}

1. 您可以禁用「銷售市場活動」和/或「即將到來的」部分中的「任務」標籤。 這將適用於銷售線索、聯繫人、客戶和機會小組。

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. 通過取消檢查「操作」設定下的相應功能，可以禁用MSI操作。

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>Governance settings are applicable to all MSI users.
