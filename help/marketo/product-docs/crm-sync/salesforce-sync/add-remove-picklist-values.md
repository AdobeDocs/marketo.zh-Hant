---
unique-page-id: 4719312
description: 新增/移除挑選清單值 — Marketo檔案 — 產品檔案
title: 新增/移除挑選清單值
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# 新增/移除挑選清單值 {#add-remove-picklist-values}

以下是有關在Salesforce中新增和移除挑選清單值的幾點須知。

## 新增挑選清單值 {#adding-picklist-values}

1. 如果在Salesforce中為挑選清單欄位型別新增了其他值，您將收到 [通知](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md) 識別此動作將影響的表單。

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. 前往表單編輯器並 [新增其他值](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md) 至您的建議清單。

## 移除挑選清單值 {#remove-picklist-values}

從Salesforce的欄位中移除挑選清單值時，您必須從託管此欄位的所有表單中手動移除此值。

>[!NOTE]
>
>如果Salesforce中的潛在客戶欄位和聯絡人欄位有不同的值，則共同的值將可用於Marketo。

如果Salesforce中的潛在客戶欄位和聯絡人欄位有不同的值：

1. 在SFDC中新增其他值至挑選清單將會收到通知。
1. 通知會告訴您其使用位置。 如有需要，您現在可以將這個新值新增為表單上的選項。

如果SFDC潛在客戶的挑選清單與SFDC連絡人的挑選清單的值不同，則通用值會用作表單中的預設值選項。

如果您從挑選清單中移除值，您必須手動將其作為選項從表單中移除。
