---
unique-page-id: 37355569
description: 程式成員自訂欄位 — Marketo檔案 — 產品檔案
title: 方案成員自訂欄位
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 1%

---

# 方案成員自訂欄位 {#program-member-custom-fields}

方案成員自訂欄位可讓您收集每個成員的方案特定資料。 它們可用於： Marketo表單、智慧清單篩選器和觸發器，以及智慧行銷活動流量動作。 可在方案的「成員」標籤中檢視資料。

## 建立方案成員自訂欄位 {#create-a-program-member-custom-field}

1. 在Marketo中，按一下 **管理員**.

   ![](assets/one.png)

1. 按一下 **欄位管理**.

   ![](assets/two.png)

1. 按一下 **新增自訂欄位**.

   ![](assets/three.png)

1. 按一下「物件」下拉式清單，然後選取所需的物件。

   ![](assets/four.png)

   >[!NOTE]
   >
   >「人員」和「方案成員」自訂欄位不能共用相同的名稱。

1. 填寫其餘欄位，然後按一下 **建立**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >程式成員自訂欄位支援的型別為：布林值、日期、日期時間、浮點數、整數、字串、URL。 [進一步瞭解欄位型別](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}.

## 物件說明 {#object-descriptions}

| 物件 | 說明 |
|---|---|
| 公司 | 與個人相關聯的公司名稱。 |
| 機會 | 商機可以與個人或帳戶相關聯，作為潛在的未來銷售。 他們通常會透過CRM或API進入Marketo。 |
| 個人 | 您透過行銷活動與之Marketo資料庫中的個人互動。 |
| 計畫成員 | 同時身為計畫成員的人 |

## 觸發器和篩選器 {#triggers-and-filters}

您可以透過以下方式在智慧清單中運用此程式特有的資料： [觸發器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"} and/or [filters](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}.

![](assets/six.png)

## 須知 {#things-to-know}

* 方案成員自訂欄位僅可用於本機資產。 Design Studio不支援這些設定，因為無法將其繫結至特定程式。
* 您無法複製/移動包含程式成員自訂欄位的表單（或含有表單的登陸頁面）至Design Studio。
* [您可以同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"} 方案成員自訂欄位和促銷活動成員自訂欄位。
* 程式成員物件最多可以有20個自訂欄位。 這些欄位適用於任何計畫。
* 當您移除某個方案的成員時，如果他們的方案成員自訂欄位中有任何資料，則會從該欄位中清除該資料。
* 若要檢視資料，請按一下方案中的成員索引標籤，並建立包含上述欄位的自訂檢視。
* 透過匯入和匯出 [清單](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"} and [API](https://developers.marketo.com/){target="_blank"} 支援。 匯出僅適用於「方案成員」清單，不適用於靜態清單。
* 合併兩個人時，將會使用獲勝者的方案成員自訂欄位資料。 但如果成功者沒有值，則會使用失敗者的值。
* 計畫成員資訊欄位不允許變更型別。
* 「方案成員」自訂欄位不支援「包含」智慧清單限制。

>[!MORELIKETHIS]
>
>* [在Marketo中建立自訂欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}
>
>* [程式成員自訂欄位同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"}
