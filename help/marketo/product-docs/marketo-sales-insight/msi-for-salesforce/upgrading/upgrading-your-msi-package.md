---
unique-page-id: 37357050
description: 升級MSI套件 — Marketo檔案 — 產品檔案
title: 升級MSI封裝
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 升級MSI封裝 {#upgrading-your-msi-package}

>[!IMPORTANT]
>
>由於Salesforce的安全性增強，銷售Insight套件無法再授與標準物件的許可權。 日後，Sales Insight使用者的Salesforce設定檔需要具備下列標準物件的讀取存取權：銷售機會、連絡人、帳戶和機會。 [在此瞭解如何設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#grant-sales-insight-users-profile-access){target="_blank"}。

1. 在appexchange[中導覽至](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target="_blank"}此頁面。

1. 從步驟一的頁面右上角，登入您的[!DNL Salesforce]執行個體(連線到您的Marketo執行個體的執行個體，可以是沙箱或生產環境)。 您必須擁有管理員許可權，才能在[!DNL Salesforce]中安裝/升級Managed套件。

1. 按一下&#x200B;**立即取得**&#x200B;按鈕。 系統會要求您選擇要安裝的位置。 由於您已有舊版MSI，因此可以選擇升級。 根據您在步驟一期間登入的帳戶選擇選項。

   >[!TIP]
   >
   >建議您在升級生產執行個體之前，先在沙箱執行個體上測試此專案。

1. 您可以選擇「僅供管理員安裝」（並在稍後提供特定設定檔的MSI存取權）、「為所有使用者安裝」或「為特定設定檔安裝」來升級套件。 在此範例中，我們選擇「僅限管理員」。 當您選擇完畢後，請按一下[升級]。**&#x200B;**

   ![](assets/four.png)

>[!NOTE]
>
>建議您僅更新管理員的套件，然後[根據購買的MSI座位數提供特定使用者](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}的存取權。 或者，您也可以為MSI使用者建立特定的Salesforce設定檔，並僅為這些使用者安裝或升級套件。
