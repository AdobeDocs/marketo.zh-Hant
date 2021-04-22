---
unique-page-id: 2360291
description: 欄位的區塊更新-Marketo檔案——產品檔案
title: 塊對欄位的更新
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 對欄位{#block-updates-to-a-field}的塊更新

封鎖對欄位的更新可讓您只需寫入欄位一次，然後保留欄位存留期的原始值。 這對於「人員來源」之類的欄位非常有用。

>[!NOTE]
>
>**需要管理員權限**

1. 前往&#x200B;**Admin**，然後按一下「欄位管理」。****

   ![](assets/image2014-9-24-13-3a54-3a40.png)

1. 查找欄位，選擇它，然後在&#x200B;**欄位操作**&#x200B;下，按一下&#x200B;**塊欄位更新**。

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >您也可以阻止[程式成員自定義欄位](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)的更新。

1. 選擇要阻止的&#x200B;**輸入源** ，然後按一下&#x200B;**應用**。

   ![](assets/image2014-9-24-13-3a55-3a16.png)

   >[!CAUTION]
   >
   >執行清單匯入時，「匯入預覽」中被封鎖的欄位狀態只有在Marketo根據與&#x200B;_完全符合_&#x200B;的欄位名稱自動識別欄位（或如果已建立別名）時，才會顯示。 如果從「Marketo欄位」下拉式清單中手動選擇欄位，則「導入預覽」中不會顯示被阻止狀態，但該欄位的更新阻止仍將實施。
