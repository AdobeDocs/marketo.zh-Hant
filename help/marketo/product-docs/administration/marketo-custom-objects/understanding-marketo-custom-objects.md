---
unique-page-id: 10093188
description: 瞭解行銷人員自訂物件——行銷人員檔案——產品檔案
title: 瞭解Marketo自訂物件
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---


# 瞭解Marketo自訂物件{#understanding-marketo-custom-objects}

使用自訂物件來追蹤您業務的特定量度。

>[!NOTE]
>
>**可用性**
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請洽詢您的銷售代表。

在智慧型促銷活動中使用自訂物件做為篩選和觸發器。 例如：

* **篩選**:僅傳送電子郵件給特定汽車品牌的擁有者
* **觸發器**:當自訂物件新增至個人或公司時，傳送電子郵件。

您可以在一對多或多對多關係中設定自訂物件。 例如：

* **一對多**:一個人擁有幾輛汽車
* **多對多**:從課程目錄註冊多個課程的學生

一對多結構使用單一連結欄位將自訂物件連接至個人或公司。

多對多自訂物件使用兩個連結欄位，這是中間物件的一部分。 一個「連結」欄位會連接至人員或公司，另一個欄位則會連接至自訂物件，例如課程目錄。 此中介物件可包含其他自訂欄位，例如課程等級或出勤日期，進一步定義連線的性質。

>[!TIP]
>
>在使用者介面中使用逗號分隔值(CSV)匯入自訂物件，以測試和驗證資料範例。 然後，使用API上傳您的所有檔案。

>[!CAUTION]
>
>您無法還原自訂物件，因此在刪除物件之前，請務必不再需要這些物件。

## 存取行銷人員自訂物件{#accessing-marketo-custom-objects}

1. 若要建立或編輯Marketo自訂物件，請按一下**管理**，然後按一下&#x200B;**Marketo自訂物件**&#x200B;連結。

   ![](assets/image2016-5-18-16-3a59-3a30.png)

1. 「行銷自訂物件」會在右側列出您的所有自訂物件，但僅會列在主格線中已核准的物件。

   ![](assets/image2016-6-10-15-3a14-3a18.png)

1. 網格顯示對象名稱、記錄數、欄位數和最近更新的日期。

   >[!TIP]
   >
   >Market會自動更新這些欄位，但您可以按一下「記錄」欄中的圖示，重新整理顯示畫面。

1. 按一下右側的物件名稱，以開啟詳細資訊頁面。

   ![](assets/image2016-6-10-15-3a15-3a29.png)

## 查看與{#view-custom-objects-associated-to-a-person}人員關聯的自定義對象

在您建立自訂物件結構後，當您上傳特定自訂物件資料時，自訂物件會使用自訂物件中的連結欄位，自動與資料庫中的人員建立關聯。 您可以從人員詳細資料頁面的「自訂物件」索引標籤中檢視資訊。

1. 轉至&#x200B;**Database**。

   ![](assets/db.png)

1. 開啟資料庫，然後按一下&#x200B;**People**&#x200B;頁籤。 連按兩下您與自訂物件關聯之人員的記錄。

   ![](assets/five.png)

1. 在人員詳細資訊頁面上，按一下&#x200B;**自定義對象**&#x200B;頁籤。 從下拉式清單中選取物件。

   ![](assets/six.png)

1. 現在，您可以檢視與該人員相關聯之該類型所有自訂物件的清單。

   ![](assets/seven.png)

## 搭配公司使用自訂物件{#using-custom-objects-with-companies}

如果您從CRM同步公司，或者您使用API明確建立公司，連結至公司的自訂物件最能運作。 我們也建議您使用「公司ID」作為連結欄位。

如果您在Marketo中有多個人是CRM或Marketo-only記錄中的記錄，連結至公司的自訂物件將不會與多個個別記錄產生關聯。 這是因為，只有當公司與CRM同步或您使用API明確建立公司時，才支援在其下有多人的公司。

自訂物件只能直接連結至單一記錄。 這表示當您的自訂物件類型依公司欄位連結時，如果您管理使用Marketo的REST API的公司，您應確保您的個人記錄與公司相關聯，或者使用CRM中的連絡人轉換，或使用externalCompanyId欄位。 對於未明確連結至公司記錄的個人記錄，使用公司連結的自訂物件會隨機連結至單一記錄，即使公司欄位的值已共用給許多人亦然。

如需詳細資訊，請參閱[匯入自訂物件資料](import-custom-object-data.md)。

>[!MORELIKETHIS]
>
>* [建立Marketo自訂物件](create-marketo-custom-objects.md)
>* [批准自訂物件](approve-a-custom-object.md)
>* [編輯和刪除行銷人員自訂物件](edit-and-delete-a-marketo-custom-object.md)
>* [新增行銷至自訂物件欄位](add-marketo-custom-object-fields.md)
>* [編輯和刪除Marketo自訂物件欄位](edit-and-delete-marketo-custom-object-fields.md)
>* [匯入自訂物件資料](import-custom-object-data.md)

>



