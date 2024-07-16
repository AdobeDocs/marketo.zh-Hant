---
unique-page-id: 1147324
description: 清除欄位值 — Marketo檔案 — 產品檔案
title: 清除欄位值
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 7dd2e21969b71a50bfd4643ab15459150ca07c92
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# 清除欄位值 {#clear-field-values}

[變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)很好，但您如何&#x200B;_完全移除_&#x200B;值？ 好問題！

1. 在流程步驟中，選擇要清除的欄位，並輸入&#x200B;**NULL** （全部大寫）作為&#x200B;**新值**。

   ![](assets/clear-field-values-1.png)

1. 搖晃！ 我打賭您不知道這點！ 流程步驟完成後，會清除所選欄位的值。

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >將新值保留為空白或僅輸入SPACE並不會真正清空欄位。 您必須輸入NULL。 此外，請記住，執行後無法復原流程步驟。
