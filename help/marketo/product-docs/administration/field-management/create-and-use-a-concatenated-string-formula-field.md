---
unique-page-id: 2360337
description: 建立並使用串連字串（公式）欄位 — Marketo檔案 — 產品檔案
title: 建立和使用串連字串 (公式) 欄位
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 13%

---

# 建立和使用串連字串 (公式) 欄位 {#create-and-use-a-concatenated-string-formula-field}

您可以合併多個欄位的值，或使用Marketo Engage公式欄位建立條件值。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. 按一下「**[!UICONTROL Field Management]**」。

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. 按一下「**[!UICONTROL New Custom Field]**」。

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. 為&#x200B;**[!UICONTROL Formula]**&#x200B;選取&#x200B;**[!UICONTROL Type]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. 輸入欄位的&#x200B;**[!UICONTROL Name]**，然後按一下&#x200B;**[!UICONTROL Create]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. 尋找並選取您的公式欄位，然後按一下&#x200B;**[!UICONTROL Edit Rules]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. 新增兩個選項並定義它們，如下面的熒幕擷圖所示。

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >深入瞭解流程步驟[的](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md)權杖。

1. 現在您可以在電子郵件中新增公式欄位做為代號。

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>公式欄位可用於登陸頁面、電子郵件和智慧列示欄。 含有公式欄位的電子郵件&#x200B;_無法_&#x200B;使用批次行銷活動傳送。 請在此案例中使用[電子郵件指令碼權杖](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)。

做得好！ 現在您有了一個智慧型欄位，可根據性別知道要包含哪些稱呼。 玩得開心，發揮創意。
