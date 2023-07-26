---
unique-page-id: 1147324
description: 清除欄位值 — Marketo檔案 — 產品檔案
title: 清除欄位值
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# 清除欄位值 {#clear-field-values}

[變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) 很好，但您如何 _移除_ 值是否完全相同？ 好問題！

1. 在流程步驟中，選擇要清除的欄位並輸入 **空** （全部大寫） **新值**.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. 搖晃！ 我打賭您不知道這點！ 流程步驟完成後，會清除所選欄位的值。

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >將新值保留為空白或僅輸入SPACE並不會真正清空欄位。 您必須輸入NULL。 此外，請記住，執行後無法復原流程步驟。
