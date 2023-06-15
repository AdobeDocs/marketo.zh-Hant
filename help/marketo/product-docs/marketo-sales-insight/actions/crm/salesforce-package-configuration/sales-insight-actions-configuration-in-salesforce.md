---
description: Salesforce中的Sales Insight Actions設定 — Marketo檔案 — 產品檔案
title: Salesforce中的Sales Insight動作設定
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Salesforce中的Sales Insight動作設定 {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [安裝](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) 或 [升級](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Salesforce例項中的Sales Insight Package
>* [在Salesforce Enterprise/Unlimited中設定Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

## 在Salesforce中新增遠端站台 {#add-new-remote-site-in-salesforce}

1. 在Salesforce中，按一下 **設定**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. 搜尋「遠端站台」並選取 **遠端站台設定**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. 按一下 **新增遠端站台**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. 輸入遠端網站名稱（可能類似「MarketoSalesInsight1」）。 輸入遠端站台URL `https://ims-na1.adobelogin.com` 並按一下 **儲存**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. 按一下 **新增遠端站台** 再來一次。

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. 輸入遠端網站名稱（可以類似於「MarketoSalesInsight2」）。 輸入遠端站台URL `https://mkto-sales-connect.adobe.io` 並按一下 **儲存**.

## 在整個CRM中啟用銷售分析動作 {#enabling-sales-insight-actions-across-the-crm}

1. 在Salesforce中，按一下 **Marketo銷售分析設定** 標籤。

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >如果您在頂端列中看不到「Marketo銷售分析設定」，請按一下 **+** 在所有標籤下簽署並尋找它。

1. 選取 **啟用MSI動作** 核取方塊。

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. 輸入API金鑰。

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >如果您沒有可用的API秘密金鑰，可以依照以下步驟找到： [本文](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. 按一下 **儲存** 完成時。

這會自動啟用功能概觀文章中概述的所有MSI Actions功能。

>[!NOTE]
>
>只要取消勾選「啟用MSI動作」核取方塊，即可停用所有MSI動作功能。

## MSI動作控管 {#msi-actions-governance}

1. 您可以停用即將到來的區段中的Sales Campaigns及/或Task索引標籤。 這將適用於銷售機會、聯絡人、客戶和機會面板。

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. 您可以取消勾選「動作」設定下的對應功能，以停用MSI動作。

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>治理設定適用於所有MSI使用者。
