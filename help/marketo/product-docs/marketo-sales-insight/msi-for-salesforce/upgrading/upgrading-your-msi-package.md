---
unique-page-id: 37357050
description: 升級MSI套件 — Marketo檔案 — 產品檔案
title: 升級MSI封裝
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 升級MSI封裝 {#upgrading-your-msi-package}

1. 導覽至 [appexchange中的此頁面](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target="_blank"}.

1. 從步驟一的頁面右上角，登入您的Salesforce執行個體(連線到您的Marketo執行個體的執行個體，可以是沙箱或生產環境)。 您必須擁有管理員許可權，才能在Salesforce中安裝/升級受管理的套件。

1. 按一下 **立即取得** 按鈕。 系統會要求您選擇要安裝的位置。 由於您已經有舊版的MSI，因此您可以選擇升級。 根據您在步驟一期間登入的帳戶選擇選項。

   >[!TIP]
   >
   >建議您在升級生產執行個體之前，在沙箱執行個體上測試此專案。

1. 您可以選擇「僅供管理員安裝」（並在稍後提供特定設定檔的MSI存取權）、「為所有使用者安裝」或「為特定設定檔安裝」來升級套件。 在此範例中，我們選擇「僅限管理員」。 完成選取後，按一下 **升級**.

   ![](assets/four.png)

>[!NOTE]
>
>建議您僅更新管理員的套件，然後 [提供特定使用者的存取權](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"} 根據購買的MSI座位數。 或者，您也可以為MSI使用者建立特定的Salesforce設定檔，並僅為這些使用者安裝或升級套件。
