---
unique-page-id: 4719312
description: 新增/移除挑選清單值 — Marketo檔案 — 產品檔案
title: 新增/移除選項清單值
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 3%

---

# 新增/移除選項清單值 {#add-remove-picklist-values}

以下是在[!DNL Salesforce]中新增和移除挑選清單值的一些須知事項。

## 新增挑選清單值 {#adding-picklist-values}

1. 如果在Salesforce中將額外的值新增至挑選清單欄位型別，您將會收到識別這會影響哪些表單的[通知](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md){target="_blank"}。

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. 移至表單編輯器，然後[將其他值](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md){target="_blank"}新增至您的建議清單。

## 移除挑選清單值 {#remove-picklist-values}

從[!DNL Salesforce]中的欄位移除挑選清單值時，您必須從託管此欄位的所有表單中手動移除此值。

>[!NOTE]
>
>如果Salesforce中的潛在客戶欄位和聯絡人欄位有不同的值，則共同值可用於Marketo Engage。

如果[!DNL Salesforce]中的潛在客戶欄位和聯絡人欄位有不同的值：

1. 在SFDC中新增其他值至選擇清單會收到通知。
1. 通知會說明其使用位置。 如有需要，您現在可以將這個新值新增為表單上的選項。

如果SFDC潛在客戶選擇清單的值與SFDC聯絡人的選擇清單不同，則通用值會用作表單中的預設值選項。

如果您從選擇清單中移除值，您必須手動將其從表單中移除作為選項。
