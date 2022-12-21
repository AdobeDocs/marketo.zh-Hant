---
unique-page-id: 10093188
description: 了解Marketo自訂物件 — Marketo檔案 — 產品檔案
title: 了解Marketo自訂物件
exl-id: f18b1689-c7bc-4da0-8326-7b29733d527d
source-git-commit: 6f17d79344653d1b2c364753d774998e343c9808
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# 了解Marketo自訂物件 {#understanding-marketo-custom-objects}

使用自訂物件來追蹤您企業專屬的量度。

>[!AVAILABILITY]
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請連絡您的銷售代表。

在智慧型行銷活動中使用自訂物件作為篩選和觸發器。 例如：

* **篩選**:僅傳送電子郵件給特定汽車品牌的擁有者
* **觸發**:將自訂物件新增至人員或公司時，傳送電子郵件。

您可以以一對多或多對多關係來設定自訂物件。 例如：

* **一對多**:一個人擁有數輛汽車
* **多對多**:從課程目錄中註冊了多個課程

一對多結構使用單一連結欄位，將自訂物件連結至人員或公司。

多對多自訂物件使用兩個連結欄位，這是中間物件的一部分。 一個連結欄位連接到人員或公司，另一個連接到自定義對象，如課程目錄。 此中間對象可包含其他自定義欄位，如課程級別或考勤日期，這進一步定義了連接的性質。

>[!TIP]
>
>在使用者介面中使用逗號分隔值(CSV)匯入自訂物件，以測試及驗證資料範例。 然後，使用API上傳所有檔案。

>[!CAUTION]
>
>您無法還原自訂物件，因此在刪除自訂物件之前，請務必不再需要它們。

## 存取Marketo自訂物件 {#accessing-marketo-custom-objects}

1. 若要建立或編輯Marketo自訂物件，請按一下 **管理** 然後 **Marketo自訂物件** 連結。

   ![](assets/understanding-marketo-custom-objects-1.png)

1. 「Marketo自訂物件」顯示會在右側列出所有自訂物件，但主格線中只會列出已核准的物件。

   ![](assets/understanding-marketo-custom-objects-2.png)

1. 格線會顯示物件名稱、記錄數、欄位數，以及最新更新的日期。

   >[!TIP]
   >
   >Marketo會自動更新這些欄位，但您可以按一下「記錄」欄中的圖示，以重新整理顯示畫面。

1. 按一下右側的物件名稱，以開啟詳細資訊頁面。

   ![](assets/understanding-marketo-custom-objects-3.png)

## 查看與人員關聯的自定義對象 {#view-custom-objects-associated-to-a-person}

建立自訂物件結構後，上傳特定自訂物件資料時，自訂物件會使用自訂物件中的連結欄位，自動與資料庫中的人員建立關聯。 您可以從人員詳細資訊頁面上的「自定義對象」頁簽查看資訊。

1. 前往 **資料庫**.

   ![](assets/understanding-marketo-custom-objects-4.png)

1. 開啟資料庫，然後按一下 **人員** 標籤。 按兩下與自定義對象關聯的人員的記錄。

   ![](assets/understanding-marketo-custom-objects-5.png)

1. 在人員詳細資訊頁面上，按一下 **自訂物件** 標籤。 從下拉式清單中選取物件。

   ![](assets/understanding-marketo-custom-objects-6.png)

1. 現在，您可以檢視與該人員相關聯的該類型所有自訂物件清單。

   ![](assets/understanding-marketo-custom-objects-7.png)

## 搭配公司使用自訂物件 {#using-custom-objects-with-companies}

如果您從CRM同步公司，或您使用API明確建立公司，連結至公司的自訂物件最能運作。 我們也建議您使用公司ID作為連結欄位。

如果Marketo中有多個人員是CRM中的記錄或僅限Marketo的記錄，則連結至公司的自訂物件將不會與多個個別記錄建立關聯。 這是因為，只有當公司從CRM向下同步，或您使用API明確建立公司時，才支援底下有多人的公司。

自定義對象只能直接連結到單個記錄。 這表示當您的自訂物件類型依公司欄位連結時，如果您使用Marketo的REST API管理公司，應確保您的人員記錄與公司相關聯，或是透過CRM中的聯絡人轉換，或是使用externalCompanyId欄位。 對於未明確連結至公司記錄的人員記錄，使用公司連結的自訂物件將隨機連結至單一記錄，即使公司欄位的值已共用給許多人亦然。

請參閱 [匯入自訂物件資料](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md) 以取得更多資訊。

>[!MORELIKETHIS]
>
>* [建立Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [核准自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [編輯和刪除Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [新增Marketo自訂物件欄位](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [編輯和刪除Marketo自訂物件欄位](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [匯入自訂物件資料](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)

