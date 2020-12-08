---
unique-page-id: 4719312
description: 新增／移除Picklist值——行銷人員檔案——產品檔案
title: 添加／刪除選擇清單值
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# 添加／刪除選擇清單值 {#add-remove-picklist-values}

以下是在Salesforce中新增和移除挑選清單值的一些相關資訊。

## 添加選擇清單值 {#adding-picklist-values}

1. 如果Salesforce中有額外值新增至挑選清單欄位類型，您會收到通知 [](../../../product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md) ，指出這會影響哪些表單。

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. 前往表單編輯器，並 [將其他值新增至您的建議清單](../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md) 。

## 刪除選擇清單值 {#remove-picklist-values}

從Salesforce的欄位移除選取清單值時，您必須從托管此欄位的所有表單中手動移除此值。

>[!NOTE]
>
>如果Salesforce中的銷售機會欄位和連絡人欄位有不同的值，Marketo中將可使用常用的值。

如果Salesforce中的銷售機會欄位和連絡人欄位有不同的值：

1. 將SFDC中的附加值添加到選擇清單將獲得通知。
1. 通知會告訴您其使用位置。 您現在可以視需要在表單上新增此新值。

如果SFDC銷售線索的挑庫清單與SFDC聯繫人的挑庫清單的值不同，則公用值將用作表單中的預設值選項。

如果從選取清單移除值，您必須從表單中以選項的形式手動移除。
