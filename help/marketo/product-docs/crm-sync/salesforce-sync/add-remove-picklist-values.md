---
unique-page-id: 4719312
description: 新增／移除挑選清單值-Marketo檔案——產品檔案
title: 添加／刪除選擇清單值
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# 添加／刪除選擇清單值{#add-remove-picklist-values}

以下是在Salesforce中新增和移除選取清單值的一些相關資訊。

## 添加選擇清單值{#adding-picklist-values}

1. 如果Salesforce中有附加值新增至挑選清單欄位類型，您會收到[通知](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md)，指出這會影響哪些表單。

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. 前往表單編輯器，並將[附加值](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)新增至建議清單。

## 刪除選擇清單值{#remove-picklist-values}

從Salesforce的欄位移除選取清單值時，您必須從托管此欄位的所有表單中手動移除此值。

>[!NOTE]
>
>如果Salesforce中的銷售機會欄位和連絡人欄位有不同的值，則通用值將可用於Marketo。

如果Salesforce中的銷售機會欄位和連絡人欄位有不同的值：

1. 將SFDC中的附加值添加到選擇清單將獲得通知。
1. 通知會告訴您其使用位置。 您現在可以視需要在表單上新增此新值。

如果SFDC銷售線索的挑庫清單與SFDC聯繫人的挑庫清單的值不同，則公用值將用作表單中的預設值選項。

如果從選取清單移除值，您必須從表單中以選項的形式手動移除。
