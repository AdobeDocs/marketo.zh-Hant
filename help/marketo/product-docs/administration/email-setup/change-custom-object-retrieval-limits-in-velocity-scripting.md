---
description: 變更Velocity指令碼——行銷人員檔案——產品檔案中的自訂物件擷取限制
title: 變更速度指令碼中的自訂物件擷取限制
translation-type: tm+mt
source-git-commit: cfefff241b34571b9778cbd827f45d1b468d121e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---


# 在Velocity指令碼中變更自訂物件擷取限制{#change-custom-object-retrieval-limits-in-velocity-scripting}

如果您使用Velocity指令碼在電子郵件中顯示自訂物件資料，此功能可能適合您。 預設情況下，允許您從Velocity指令碼訪問10個父自定義對象。 如果您需要存取更多資訊，請閱讀。

## 什麼是Velocity {#what-is-velocity}

[Apache Velocity](https://velocity.apache.org/)是以Java為基礎的語言，專為範本化和編寫HTML內容指令碼而設計。Marketo可讓您透過使用[指令碼Token](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)，在電子郵件中使用它。 除了其他功能，這可讓您存取儲存在自訂物件中的資料。

您可以參考直接連接至Lead或Contact的父項和子項自訂物件，但不能參考第三層自訂物件。 對於每個自訂物件，每位人員／連絡人有10個最近更新的記錄可在執行時期使用，並依序從最近更新(0)到最舊更新(9)。

## 如何更改限制{#how-to-change-the-limit}

1. 前往&#x200B;**Admin**&#x200B;區段。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. 按一下&#x200B;**電子郵件**。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. 在「自定義對象檢索限制」(Custom Object Retrieval Limits)表中，輸入新的父檢索限制，然後按一下「保存更改」(Save Changes)**。**

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>父檢索限制值必須在10 - 100範圍內。 系統會自動為您設定子檢索限制。 這是透過將1000除以父項擷取限制來完成。 例如，如果您將父代限制設定為50，則子代限制將變為20(1000 ÷ 50 = 20)。

真貼心！ 現在，您可以從Velocity指令碼存取更多自訂物件。
