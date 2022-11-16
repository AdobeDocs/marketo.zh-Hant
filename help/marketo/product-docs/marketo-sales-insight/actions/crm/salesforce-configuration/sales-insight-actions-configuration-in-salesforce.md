---
description: Salesforce中的Sales Insight Actions設定 — Marketo檔案 — 產品檔案
title: Salesforce中的Sales Insight Actions配置
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 854bbc3642d52e670e0e55e6660ea85661edf904
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Salesforce中的Sales Insight Actions配置 {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [安裝](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) 或 [升級](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Salesforce例項中的Sales Insight Package
>* [在Salesforce Enterprise/Unlimited中設定Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)


## 在Salesforce中添加新遠程站點 {#add-new-remote-site-in-salesforce}

1. 在Salesforce中，按一下 **設定**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. 搜索「遠程站點」並選擇 **遠程站點設定**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. 按一下 **新遠程站點**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. 輸入遠端網站名稱（可以是「MarketoSalesInsight1」之類的名稱）。 輸入遠程站點URL `https://ims-na1.adobelogin.com` 按一下 **儲存**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. 按一下 **新遠程站點** 。

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. 輸入遠端網站名稱（可以是「MarketoSalesInsight2」之類的名稱）。 輸入遠程站點URL `https://mkto-sales-connect.adobe.io` 按一下 **儲存**.

## 在整個CRM中啟用Sales Insight Actions {#enabling-sales-insight-actions-across-the-crm}

1. 在Salesforce中，按一下 **Marketo Sales Insight設定** 標籤。

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >如果頂端列中未顯示「Marketo Sales Insight Config」，請按一下 **+** 在「所有標籤」下簽名並查找它。

1. 選取 **啟用MSI操作** 核取方塊。

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. 輸入API密鑰。

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

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

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. 通過取消檢查「操作」設定下的相應功能，可以禁用MSI操作。

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>控管設定適用於所有MSI用戶。
