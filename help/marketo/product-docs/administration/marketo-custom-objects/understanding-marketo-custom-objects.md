---
unique-page-id: 10093188
description: 瞭解Marketo自訂物件 — Marketo檔案 — 產品檔案
title: 瞭解Marketo自訂物件
exl-id: f18b1689-c7bc-4da0-8326-7b29733d527d
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 0%

---

# 瞭解Marketo自訂物件 {#understanding-marketo-custom-objects}

使用自訂物件來追蹤您企業的特定量度。

>[!AVAILABILITY]
>
>並非所有客戶都已購買此功能。 請聯絡您的銷售代表以取得詳細資訊。

在智慧型行銷活動中使用自訂物件作為篩選器和觸發器。 例如：

* **篩選**：僅傳送電子郵件給特定車輛品牌的所有者
* **觸發**：當自訂物件新增至人員或公司時傳送電子郵件。

您可以在一對多或多對多關係中設定自訂物件。 例如：

* **一對多**：一個人擁有多輛汽車
* **多對多**：多名學生從課程目錄註冊了多個課程

一對多結構使用單一連結欄位來將自訂物件連線到個人或公司。

多對多的自訂物件使用兩個連結欄位，是中介物件的一部分。 一個「連結」欄位會連線至個人或公司，另一個則連線至自訂物件，例如課程目錄。 此中介物件可包含其他自訂欄位，例如課程等級或出勤日期，以進一步定義連線的性質。

>[!TIP]
>
>在使用者介面中使用逗號分隔值(CSV)匯入自訂物件，以測試和驗證資料範例。 然後，使用API上傳您的所有檔案。

>[!CAUTION]
>
>您無法還原自訂物件，因此在刪除前請確定不再需要這些物件。

## 存取Marketo自訂物件 {#accessing-marketo-custom-objects}

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/understanding-marketo-custom-objects-1.png)

1. 按一下 **[!UICONTROL Marketo自訂物件]**.

   ![](assets/understanding-marketo-custom-objects-2.png)

1. 「Marketo自訂物件」顯示會在右側列出所有自訂物件，但只列出主格線中核准的物件。

   ![](assets/understanding-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >網格會顯示物件名稱、記錄數、欄位數以及最近更新的日期。

   >[!TIP]
   >
   >Marketo會自動更新這些欄位，但您可以按一下「記錄」欄中的圖示重新整理顯示。

1. 按一下右側的物件名稱以開啟詳細資訊頁面。

   ![](assets/understanding-marketo-custom-objects-4.png)

## 檢視與個人相關聯的自訂物件 {#view-custom-objects-associated-to-a-person}

建立自訂物件結構後，當您上傳特定自訂物件資料時，自訂物件會自動使用自訂物件中的連結欄位與資料庫中的人員建立關聯。 您可以檢視以下專案的資訊： [!UICONTROL 自訂物件] 「個人詳細資料」頁面上的標籤。

1. 前往 **[!UICONTROL 資料庫]**.

   ![](assets/understanding-marketo-custom-objects-5.png)

1. 開啟資料庫並按一下 **[!UICONTROL 人員]** 標籤。 連按兩下您與自訂物件相關聯之人員的記錄。

   ![](assets/understanding-marketo-custom-objects-6.png)

1. 在人員詳細資訊頁面上，按一下 **[!UICONTROL 自訂物件]** 標籤。 從下拉式清單中選取物件。

   ![](assets/understanding-marketo-custom-objects-7.png)

1. 現在您可以檢視與該人員相關聯之該型別的所有自訂物件清單。

   ![](assets/understanding-marketo-custom-objects-8.png)

## 搭配公司使用自訂物件 {#using-custom-objects-with-companies}

從CRM同步公司，或使用API明確建立公司時，連結至公司的自訂物件最能發揮效用。 我們也建議您使用公司ID作為連結欄位。

如果您的Marketo中有多個人員屬於CRM或僅限Marketo的記錄中，連結至公司的自訂物件將不會與多個個別記錄相關聯。 這是因為只有當公司從CRM同步下來，或您使用API明確建立公司時，才能支援其下有多名人員的公司。

自訂物件只能直接連結到單一記錄。 這表示，當您的自訂物件型別依公司欄位連結時，如果您使用Marketo的REST API管理公司，則應確保個人記錄透過CRM中的聯絡人轉換或使用externalCompanyId欄位，與公司相關聯。 對於未明確連結至公司記錄的人員記錄，即使公司欄位的值在多個人之間共用，使用公司連結的自訂物件也將隨機連結至單一記錄。

另請參閱 [匯入自訂物件資料](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md) 以取得詳細資訊。

>[!MORELIKETHIS]
>
>* [建立Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [核准自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [編輯和刪除Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [新增Marketo自訂物件欄位](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [編輯和刪除Marketo自訂物件欄位](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [匯入自訂物件資料](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)
