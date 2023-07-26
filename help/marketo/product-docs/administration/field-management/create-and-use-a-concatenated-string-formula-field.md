---
unique-page-id: 2360337
description: 建立並使用串連字串（公式）欄位 — Marketo檔案 — 產品檔案
title: 建立並使用串連字串（公式）欄位
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# 建立並使用串連字串（公式）欄位 {#create-and-use-a-concatenated-string-formula-field}

您可以合併多個欄位的值，或使用Marketo公式欄位建立條件值。

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. 按一下 **[!UICONTROL 欄位管理]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. 按一下 **[!UICONTROL 新增自訂欄位]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. 選取 **[!UICONTROL 公式]** 針對 **[!UICONTROL 型別]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. 輸入 **[!UICONTROL 名稱]** 然後按一下您的欄位 **[!UICONTROL 建立]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. 尋找並選取您的公式欄位，然後按一下 **[!UICONTROL 編輯規則]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. 新增兩個選項並定義它們，如下面的熒幕擷圖所示。

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >進一步瞭解 [流程步驟的權杖](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. 現在您可以在電子郵件中新增公式欄位做為代號。

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>公式欄位可用於登入頁面、電子郵件和智慧列示欄（不會匯出）。 包含公式欄位的電子郵件可以 _非_ 會使用批次行銷活動傳送。 請使用 [電子郵件指令碼Token](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) 在此案例中。

做得好！ 現在您有了一個智慧型欄位，可根據性別知道要包含哪些稱呼。 玩得開心，發揮創意。
