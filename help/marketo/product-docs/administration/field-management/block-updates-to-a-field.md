---
unique-page-id: 2360291
description: 封鎖欄位更新 — Marketo檔案 — 產品檔案
title: 封鎖欄位更新
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# 封鎖欄位更新 {#block-updates-to-a-field}

封鎖欄位的更新可讓您寫入欄位一次，然後保留欄位存留期的原始值。 這對於之類的欄位很有用 [!UICONTROL 個人來源].

>[!NOTE]
>
>**需要管理員許可權**

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/block-updates-to-a-field-1.png)

1. 按一下 **[!UICONTROL 欄位管理]**.

   ![](assets/block-updates-to-a-field-2.png)

1. 尋找欄位，選取該欄位，然後在下方 **[!UICONTROL 欄位動作]**，按一下 **[!UICONTROL 封鎖欄位更新]**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >您可以封鎖更新 [方案成員自訂欄位](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) 以及。

1. 選取 **[!UICONTROL 輸入來源]** 要封鎖並按一下 **[!UICONTROL 套用]**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >執行清單匯入時，匯入預覽中遭封鎖欄位的狀態僅在Marketo根據欄位比對的名稱自動識別欄位時顯示 _完全符合_ （或如果已建立別名）。 如果從「Marketo欄位」下拉式清單手動選擇欄位，封鎖的狀態將不會在匯入預覽中顯示，但該欄位的更新封鎖仍會實施。
