---
description: Salesforce中的MSI操作配置 — Marketo文檔 — 產品文檔
title: Salesforce中的MSI操作配置
hide: true
hidefromtoc: true
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: daff9a98605b8a5c89c538f711fecb5b7a382f84
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Salesforce中的MSI操作配置 {#msi-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>安裝/升級至 [MSI操作包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) 在您的Salesforce例項中。

## 在CRM中啟用MSI操作 {#enabling-msi-actions-across-the-crm}

1. 在Salesforce中，按一下 **Marketo Sales Insight設定** 標籤。

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

   >[!NOTE]
   >
   >如果頂端列中未顯示「Marketo Sales Insight Config」，請按一下 **+** 在「所有標籤」下簽名並查找它。

1. 選取 **啟用MSI操作** 核取方塊。

   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. 輸入API密鑰。

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

   >[!NOTE]
   >
   >如果您的API密鑰不方便，可依照 [這篇文章](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. 按一下 **儲存** 時才能使用。

這將自動啟用功能概述文章中概述的所有MSI操作功能。

>[!NOTE]
>
>只要取消勾選「啟用MSI操作」複選框，即可禁用所有MSI操作功能。

## MSI-Actions控管 {#msi-actions-governance}

1. 您可以在近期區段中停用「銷售促銷活動」和/或「任務」標籤。 這將適用於銷售機會、聯絡人、帳戶和商機面板。

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. 通過取消檢查「操作」設定下的相應功能，可以禁用MSI操作。

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

>[!NOTE]
>
>控管設定適用於所有MSI用戶。
