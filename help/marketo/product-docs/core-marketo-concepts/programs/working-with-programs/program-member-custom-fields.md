---
unique-page-id: 37355569
description: 計畫成員自定義欄位 — Marketo文檔 — 產品文檔
title: 程式成員自定義欄位
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
source-git-commit: 05f31bc1d48dff0351fb6084893be7f5a96a8754
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# 程式成員自定義欄位 {#program-member-custom-fields}

「程式成員」自定義欄位允許您收集每個成員的程式特定資料。 它們可用於：Marketo表單、智慧清單篩選器和觸發器以及智慧市場活動流操作。 在程式的「成員」(Members)頁籤中可查看資料。

>[!NOTE]
>
>此時，「程式成員」自定義欄位與「Salesforce市場活動成員」欄位沒有整合。

## 建立程式成員自定義欄位 {#create-a-program-member-custom-field}

1. 在Marketo，按一下 **管理**。

   ![](assets/one.png)

1. 按一下 **欄位管理**。

   ![](assets/two.png)

1. 按一下 **新建自定義域**。

   ![](assets/three.png)

1. 按一下「對象」(Object)下拉清單並選擇所需對象。

   ![](assets/four.png)

   >[!NOTE]
   >
   >「人員」和「程式成員」自定義欄位不能共用同一名稱。

1. 填寫剩餘欄位，然後按一下 **建立**。

   ![](assets/five.png)

   >[!NOTE]
   >
   >程式成員自定義欄位支援的類型有：boolean 、 date 、 datetime 、 float 、 integer 、 string 、 URL。 [瞭解有關欄位類型的詳細資訊](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md)。

## 對象說明 {#object-descriptions}

| 對象 | 說明 |
|---|---|
| 公司 | 與人員關聯的公司的名稱。 |
| 機會 | 機會可以與個人或帳戶關聯，作為潛在的未來銷售。 他們通常通過CRM或API進入Marketo。 |
| 人員 | 您通過營銷活動參與的Marketo資料庫中的個人。 |
| 計畫成員 | 也是計畫成員的人員 |

## 觸發器和篩選器 {#triggers-and-filters}

您可以通過以下方式在智慧清單中利用此特定於程式的資料： [觸發器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md) 和/或 [篩選](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)。

![](assets/six.png)

## 要知道的事 {#things-to-know}

* 「程式成員」自定義欄位僅在本地資產中可用。 在Design Studio中不支援它們，因為無法將其與特定程式關聯。
* 不能將包含程式成員自定義欄位的表單（或包含表單的登錄頁）克隆/移動到Design Studio。
* 程式成員對象最多可包含20個自定義欄位。 這些欄位可用於任何程式。
* 刪除程式的成員時，如果他們在「程式成員」自定義欄位中有任何資料，則會從該欄位中清除資料。
* 要查看資料，請按一下程式中的「成員」頁籤，然後建立包含該欄位的自定義視圖。
* 通過 [清單](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md) 和 [API](https://developers.marketo.com/) 。
* 合併兩個人時，將使用獲獎者的「計畫成員」自定義欄位資料。 但如果贏家沒有，那麼輸家的價值將被利用。
* 更改類型為 **不** 在「程式成員資訊」欄位上允許。

>[!MORELIKETHIS]
>
>[在Marketo建立自定義欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
