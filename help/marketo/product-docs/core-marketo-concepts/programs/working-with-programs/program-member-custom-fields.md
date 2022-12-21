---
unique-page-id: 37355569
description: 方案成員自訂欄位 — Marketo檔案 — 產品檔案
title: 方案成員自定義欄位
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
source-git-commit: 56f429dabf19c4425c68b0dcd745621681a038ae
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 1%

---

# 方案成員自定義欄位 {#program-member-custom-fields}

方案成員自定義欄位允許您收集每個成員的方案特定資料。 這些變數可用於：Marketo表單、智慧清單篩選器和觸發器，以及智慧促銷活動流程動作。 可在程式的「成員」(Members)頁簽中查看資料。

>[!NOTE]
>
>方案成員自定義欄位目前與Salesforce促銷活動成員欄位沒有整合。

## 建立方案成員自定義欄位 {#create-a-program-member-custom-field}

1. 在Marketo中，按一下 **管理**.

   ![](assets/one.png)

1. 按一下 **欄位管理**.

   ![](assets/two.png)

1. 按一下 **新自訂欄位**.

   ![](assets/three.png)

1. 按一下「物件」下拉式清單，然後選取所需的物件。

   ![](assets/four.png)

   >[!NOTE]
   >
   >「人員」和「方案成員」自定義欄位不能共用同一個名稱。

1. 填寫剩餘欄位，然後按一下 **建立**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >方案成員自定義欄位支援的類型包括：布林值、日期、日期時間、浮點數、整數、字串、URL。 [進一步了解欄位類型](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target=&quot;_blank&quot;}。

## 物件說明 {#object-descriptions}

| 物件 | 說明 |
|---|---|
| 公司 | 與人員相關聯的公司名稱。 |
| 機會 | 機會可以作為潛在的未來銷售與個人或帳戶相關聯。 他們通常透過CRM或API進入Marketo。 |
| 個人 | 您透過行銷活動參與之Marketo資料庫中的個人。 |
| 計畫成員 | 同時是方案成員的人 |

## 觸發器和篩選器 {#triggers-and-filters}

您可以透過 [觸發](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target=&quot;_blank&quot;}和/或 [篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target=&quot;_blank&quot;}。

![](assets/six.png)

## 須知 {#things-to-know}

* 方案成員自訂欄位僅適用於本機資產。 Design Studio不支援這些參數，因為無法將其與特定程式連結。
* 無法將包含程式成員自定義欄位的表單（或具有表單的登錄頁）克隆/移動到Design Studio。
* 程式成員對象最多可以有20個自定義欄位。 這些欄位可供任何方案使用。
* 刪除程式的成員時，如果程式成員的「程式成員」自定義欄位中有任何資料，則會從該欄位刪除該資料。
* 要查看資料，請按一下程式中的「成員」頁簽，並建立包含所述欄位的自定義視圖。
* 透過匯入和匯出 [清單](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target=&quot;_blank&quot;}和 [API](https://developers.marketo.com/)支援{target=&quot;_blank&quot;}。 導出僅適用於方案成員清單，而非靜態清單。
* 當您合併兩人時，將會使用獲勝者的方案成員自訂欄位資料。 但如果獲勝者沒有，則會使用失敗者的價值。
* 方案成員資訊欄位中不允許更改類型。
* 方案成員自定義欄位不支援「包含」智慧清單約束。

>[!MORELIKETHIS]
>
>[在Marketo中建立自訂欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target=&quot;_blank&quot;}
