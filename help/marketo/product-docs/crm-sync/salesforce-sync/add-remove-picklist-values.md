---
unique-page-id: 4719312
description: 新增/移除選擇清單值 — Marketo檔案 — 產品檔案
title: 添加/刪除選擇清單值
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# 添加/刪除選擇清單值 {#add-remove-picklist-values}

以下是有關在Salesforce中新增和移除選擇清單值的一些須知。

## 新增選擇清單值 {#adding-picklist-values}

1. 如果Salesforce中的附加值被添加到選擇清單欄位類型，您將收到 [通知](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md) 識別這會影響的表單。

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. 前往表單編輯器，然後 [添加附加值](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md) 建議清單。

## 刪除選擇清單值 {#remove-picklist-values}

從Salesforce的欄位移除挑選清單值時，您必須從托管此欄位的所有表單中手動移除此值。

>[!NOTE]
>
>如果Salesforce中的銷售機會欄位和聯絡人欄位有不同的值，則通用的值將可在Marketo中使用。

如果Salesforce中的潛在客戶欄位和聯繫人欄位具有不同的值：

1. 在SFDC中新增其他值至選擇清單將會收到通知。
1. 通知會告訴您其使用位置。 您現在可以視需要將這個新值新增為表單上的選項。

如果SFDC線索的選擇清單與SFDC聯繫人的選擇清單的值不同，則公用值將用作表單中的預設值選項。

如果您從選擇清單中移除值，則必須從表單中手動將其移除為選項。
