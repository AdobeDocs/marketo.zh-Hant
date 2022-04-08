---
unique-page-id: 37357050
description: 升級MSI包 — Marketo文檔 — 產品文檔
title: 升級MSI包
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# 升級MSI包 {#upgrading-your-msi-package}

1. 導航到 [此頁面在appexchange中](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target=&quot;_blank&quot;}。

1. 從步驟一頁的右上角登錄到Salesforce實例(連接到Marketo實例的實例可以是沙箱或生產)。 您必須具有管理員權限才能在Salesforce中安裝/升級托管包。

1. 按一下 **立即獲取** 按鈕 系統將要求您選擇要安裝的位置。 您將獲得升級選項，因為您已擁有以前版本的MSI。 根據您在步驟一期間登錄的帳戶選擇選項。

   >[!TIP]
   >
   >建議您在升級生產實例之前在沙盒實例上test此項。

1. 您可以通過選擇「僅安裝管理員」（並稍後提供對特定配置式的MSI訪問）、「為所有用戶安裝」或「為特定配置式安裝」來升級包。 在此示例中，我們選擇「僅管理員」。 選擇後，按一下 **升級**。

   ![](assets/four.png)

>[!NOTE]
>
>建議您僅更新管理員的包，然後 [提供對特定用戶的訪問](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;}，基於購買的MSI座位數。 或者，您可以為MSI用戶建立特定的Salesforce配置檔案，並僅為這些用戶安裝或升級包。
