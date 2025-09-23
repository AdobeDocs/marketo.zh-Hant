---
unique-page-id: 2360291
description: 封鎖欄位更新 — Marketo檔案 — 產品檔案
title: 封鎖欄位更新
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 9%

---

# 封鎖欄位更新 {#block-updates-to-a-field}

封鎖欄位的更新可讓您寫入欄位一次，然後保留欄位存留期的原始值。 這對[!UICONTROL Person Source]之類的欄位很有用。

>[!NOTE]
>
>**需要管理員許可權**

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/block-updates-to-a-field-1.png)

1. 按一下「**[!UICONTROL Field Management]**」。

   ![](assets/block-updates-to-a-field-2.png)

1. 尋找欄位，選取該欄位，然後在&#x200B;**[!UICONTROL Field Actions]**&#x200B;下按一下&#x200B;**[!UICONTROL Block Field Updates]**。

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >您也可以封鎖[程式成員自訂欄位](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)的更新。

1. 選取您要封鎖的&#x200B;**[!UICONTROL Input Sources]**&#x200B;並按一下&#x200B;**[!UICONTROL Apply]**。

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >執行清單匯入時，只有在Marketo根據符合&#x200B;_完全_&#x200B;的欄位名稱（或如果已建立別名）自動識別欄位時，才會顯示匯入預覽中遭封鎖欄位的狀態。 如果從「Marketo欄位」下拉式清單手動選擇欄位，封鎖的狀態將不會在匯入預覽中顯示，但該欄位的更新封鎖仍會實施。
