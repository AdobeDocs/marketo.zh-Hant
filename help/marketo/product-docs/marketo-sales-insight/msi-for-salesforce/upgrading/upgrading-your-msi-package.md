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

1. 導覽至 [本頁（在appexchange中）](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target=&quot;_blank&quot;}。

1. 從步驟一頁面右上角登入您的Salesforce執行個體(連線至您Marketo執行個體的執行個體可以是沙箱或生產)。 您必須擁有管理員權限，才能在Salesforce中安裝/升級受管理套件。

1. 按一下 **立即獲取** 按鈕。 系統會要求您選擇要安裝的位置。 您將可以選擇升級，因為您已經擁有了以前版本的MSI。 根據您在步驟一登入的帳戶選擇選項。

   >[!TIP]
   >
   >建議您在升級生產執行個體之前，先在沙箱執行個體上測試此項目。

1. 您可以通過選擇「僅為管理員安裝」（稍後提供對特定配置檔案的MSI訪問）、「為所有用戶安裝」或「為特定配置檔案安裝」來升級包。 在此範例中，我們選擇「僅管理員」。 進行選擇後，按一下 **升級**.

   ![](assets/four.png)

>[!NOTE]
>
>建議您僅更新管理員的套件，然後 [提供特定使用者的存取權](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;}，根據購買的MSI座位數。 或者，您可以為MSI用戶建立特定的Salesforce配置檔案，並僅為這些用戶安裝或升級包。
