---
unique-page-id: 2360291
description: 區塊欄位更新 — Marketo檔案 — 產品檔案
title: 塊對欄位的更新
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# 塊對欄位的更新 {#block-updates-to-a-field}

封鎖欄位更新可讓您寫入欄位一次，然後保留欄位存留期的原始值。 這對「人員來源」之類的欄位非常有用。

>[!NOTE]
>
>**需要管理權限**

1. 前往 **管理** 的上界。

   ![](assets/block-updates-to-a-field-1.png)

1. 按一下 **欄位管理**.

   ![](assets/block-updates-to-a-field-2.png)

1. 找到欄位，選取它，然後在 **欄位動作**，按一下 **塊欄位更新**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >您可以封鎖 [方案成員自定義欄位](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) 還有。

1. 選取 **輸入源** 要阻止並按一下 **套用**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >執行清單匯入時，只有在Marketo根據欄位比對名稱自動辨識欄位時，才會顯示「匯入預覽」中遭封鎖欄位的狀態 _恰好_ （如果已建立別名）。 如果從「Marketo欄位」下拉式清單中手動選擇欄位，則封鎖狀態不會顯示在「匯入預覽」中，但仍會實作該欄位的更新封鎖。
