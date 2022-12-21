---
unique-page-id: 12983101
description: 將自訂欄位對應至Marketo - Marketo檔案 — 產品檔案
title: 將自訂欄位對應至Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# 將自訂欄位對應至Marketo {#map-custom-fields-to-marketo}

您可能想要依預設收集超過標準Facebook商店的資訊，例如某人使用您線上遞送服務的頻率。 您可以透過 [建立自訂問題](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) 在您的Facebook領先廣告中。

不過， **Marketo不會自動開始收集此資料**. 為了讓Marketo開始擷取自訂欄位值，您 **必須** 將這些自訂欄位對應至Marketo中的欄位。

以下說明如何在「管理員」的LaunchPoint區域中設定此設定。

>[!NOTE]
>
>**需要管理權限**

1. 前往「管理員」區域，然後按一下 **LaunchPoint**. 在「已安裝的服務」下，查找和編輯 **Facebook Lead Ads**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. 按一下 **下一個**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. 保留授權帳戶的原樣 **not** 進行任何變更。 按一下 **下一個**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. 和以前一樣，將選定的頁面保持原樣 — do **not** 進行任何變更。 按一下 **下一個**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. 以下是將自訂Facebook欄位對應至Marketo欄位的位置。 按一下 **新增。**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. 在新列中，輸入Facebook自訂欄位的名稱。

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >只有已儲存至Facebook表單範本的欄位會在此處顯示為選項。

1. 按一下 **Marketo欄位** 欄。 輸入以搜尋您要對應的欄位。 選取欄位後，按一下 **儲存**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >如果Marketo中尚未有欄位可將Facebook欄位對應至，請了解如何 [建立自訂欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>您 **必須** 針對任何新的Facebook欄位完成此程式，以便Marketo收集資料。
