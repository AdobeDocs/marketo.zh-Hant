---
unique-page-id: 10093188
description: 瞭解Marketo自定義對象 — Marketo文檔 — 產品文檔
title: 瞭解Marketo自定義對象
exl-id: f18b1689-c7bc-4da0-8326-7b29733d527d
source-git-commit: 6f17d79344653d1b2c364753d774998e343c9808
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# 瞭解Marketo自定義對象 {#understanding-marketo-custom-objects}

使用自定義對象跟蹤特定於您的業務的度量。

>[!AVAILABILITY]
>
>並非所有客戶都購買了此功能。 請與銷售代表聯繫以瞭解詳細資訊。

將自定義對象用作智慧市場活動中的篩選器和觸發器。 例如：

* **篩選**:僅向特定汽車品牌的所有者發送電子郵件
* **觸發器**:將自定義對象添加到個人或公司時發送電子郵件。

您可以在一對多或多對多關係中設定自定義對象。 例如：

* **一對多**:一個人擁有幾輛車
* **多對多**:從課程目錄中註冊多個課程的多個學生

一對多結構使用單個連結欄位將自定義對象連接到個人或公司。

多對多自定義對象使用兩個連結欄位，這是中間對象的一部分。 一個「連結」欄位連接到個人或公司，另一個欄位連接到自定義對象，如課程目錄。 此中介對象可以包含附加的自定義欄位，如課程等級或考勤日期，這進一步定義了連接的性質。

>[!TIP]
>
>在用戶介面中使用逗號分隔值(CSV)導入自定義對象以test和驗證資料示例。 然後，使用API上載所有檔案。

>[!CAUTION]
>
>無法還原自定義對象，因此在刪除這些對象之前，請確保不再需要它們。

## 訪問Marketo自定義對象 {#accessing-marketo-custom-objects}

1. 要建立或編輯Marketo自定義對象，請按一下 **管理** 然後 **Marketo自定義對象** 的子菜單。

   ![](assets/understanding-marketo-custom-objects-1.png)

1. 「Marketo自定義對象」顯示右側列出了所有自定義對象，但只列出了主網格中已批准的對象。

   ![](assets/understanding-marketo-custom-objects-2.png)

1. 網格顯示對象名稱、記錄數、欄位數和最近更新的日期。

   >[!TIP]
   >
   >Marketo會自動更新這些欄位，但您可以通過按一下「記錄」列中的表徵圖來刷新顯示。

1. 按一下右側的對象名稱以開啟詳細資訊頁面。

   ![](assets/understanding-marketo-custom-objects-3.png)

## 查看與人員關聯的自定義對象 {#view-custom-objects-associated-to-a-person}

建立自定義對象結構後，在上載特定的自定義對象資料時，自定義對象將自動使用自定義對象中的連結欄位與資料庫中的人員相關聯。 您可以從人員詳細資訊頁面的「自定義對象」頁籤中查看資訊。

1. 轉到 **資料庫**。

   ![](assets/understanding-marketo-custom-objects-4.png)

1. 開啟資料庫，然後按一下 **人物** 頁籤。 按兩下您與自定義對象關聯的人員的記錄。

   ![](assets/understanding-marketo-custom-objects-5.png)

1. 在人員詳細資訊頁面上，按一下 **自定義對象** 頁籤。 從下拉清單中選擇對象。

   ![](assets/understanding-marketo-custom-objects-6.png)

1. 現在，您可以查看與該人員關聯的該類型的所有自定義對象的清單。

   ![](assets/understanding-marketo-custom-objects-7.png)

## 將自定義對象與公司一起使用 {#using-custom-objects-with-companies}

如果您從CRM中同步公司，或者您使用API顯式建立公司，則連結到公司的自定義對象最有效。 我們還建議您使用公司ID作為連結欄位。

如果您在Marketo有多個人員，這些人員是CRM或僅Marketo記錄中的記錄，則連結到公司的自定義對象將不會與多個單個記錄關聯。 這是因為只有當公司從CRM向下同步或您使用API顯式建立公司時，才支援在其下面具有多個人員的公司。

自定義對象只能直接連結到單個記錄。 這意味著，當您的自定義對象類型按公司欄位連結時，如果您使用Marketo的REST API管理公司，則應確保您的人員記錄與公司關聯，或者使用CRM中的聯繫人轉換，或者使用externalCompanyId欄位。 對於未明確連結到公司記錄的人員記錄，使用公司連結的自定義對象將隨機連結到單個記錄，即使公司欄位的值在多個人之間共用。

請參閱 [導入自定義對象資料](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md) 的子菜單。

>[!MORELIKETHIS]
>
>* [建立Marketo自定義對象](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [批准自定義對象](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [編輯和刪除Marketo自定義對象](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [添加Marketo自定義對象欄位](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [編輯和刪除Marketo自定義對象欄位](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [導入自定義對象資料](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)

