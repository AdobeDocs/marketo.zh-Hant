---
description: 在 [!DNL Velocity Scripting] - Marketo檔案 — 產品檔案中變更自訂物件擷取限制
title: 變更 [!DNL Velocity Scripting]中的自訂物件擷取限制
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# 變更[!DNL Velocity Scripting]中的自訂物件擷取限制 {#change-custom-object-retrieval-limits-in-velocity-scripting}

如果您使用[!DNL Velocity Script]在電子郵件中顯示自訂物件資料，則此功能可能適合您。 預設情況下，您可以從Velocity指令碼存取10個父系自訂物件。 如果您需要存取更多資訊，請閱讀。

## 什麼是[!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/)是建置在[!DNL Java]上的語言，專為範本化和指令碼HTML內容而設計。 Marketo可透過使用[指令碼Token](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)，將其用於電子郵件內容中。 除了其他功能以外，這還可以讓您存取儲存在自訂物件中的資料。

您可以參照直接連線至Lead或Contact的父項和子項自訂物件，但不能參照第三層自訂物件。 對於每個自訂物件，每個人員/聯絡人的10個最近更新記錄在執行階段可用，並且按照從最近更新（於0時）到最舊更新（於9時）的順序排列。

## 如何變更限制 {#how-to-change-the-limit}

1. 移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區段。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. 按一下&#x200B;**[!UICONTROL 電子郵件]**。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. 在[!UICONTROL 自訂物件擷取限制]表格中，輸入新的[!UICONTROL 父擷取限制]，然後按一下&#x200B;**[!UICONTROL 儲存變更]**。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>[!UICONTROL 父擷取限制]值必須在10到100的範圍內。 已自動為您設定[!UICONTROL 子擷取限制]。 若要這麼做，請將1000除以[!UICONTROL 父擷取限制]。 例如，如果您將父限制設為50，子限制會變成20 (1000 ÷ 50 = 20)。

很好！ 您現在可以從[!DNL Velocity script]存取更多自訂物件。
