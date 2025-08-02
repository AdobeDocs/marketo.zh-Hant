---
unique-page-id: 1147352
description: 傳送範例電子郵件 — Marketo檔案 — 產品檔案
title: 傳送範例電子郵件
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# 傳送範例電子郵件 {#send-a-sample-email}

傳送電子郵件範例既快速又簡單。 若要傳送動態內容電子郵件，請參閱[預覽包含動態內容的電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)。

>[!NOTE]
>
>您必須擁有&#x200B;**存取資料庫 — 執行單一流量動作**&#x200B;許可權，才能傳送範例電子郵件。

## 傳送範例電子郵件 {#send-a-sample-email-1}

1. 尋找並選取您的電子郵件。 按一下&#x200B;**[!UICONTROL Email Actions]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL Send Sample]**。
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >我的Token會解析為適用於電子郵件程式的值。

1. 輸入一或多個要傳送的電子郵件地址。 如果有多個電子郵件地址，請使用逗號來區隔。 完成時，按一下&#x200B;**[!UICONTROL Send]**。

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >如果您輸入多個電子郵件地址，則每個收件者都會看到這些地址。 第一個輸入的是主要收件者，後續的每個電子郵件地址都是副本收件人。

   >[!TIP]
   >
   >如果您要將權杖解析為特定人員，請在步驟2的&#x200B;**人員下拉式清單**&#x200B;中選擇該人員。

## 編輯時傳送範例電子郵件 {#send-a-sample-email-while-editing}

1. 尋找您的電子郵件，選取它並按一下&#x200B;**[!UICONTROL Edit Draft]**&#x200B;標籤。

   ![](assets/three-281-29.jpg)

1. 按一下&#x200B;**[!UICONTROL Email Actions]**，選取&#x200B;**[!UICONTROL Send Sample]**。

   ![](assets/four.png)

1. 輸入傳遞的電子郵件地址，然後按一下&#x200B;**[!UICONTROL Send]**。

   ![](assets/two.png)

   >[!NOTE]
   >
   >觸發欄位僅適用於使用[電子郵件指令碼](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)的使用者。

## 根據區段傳送範例電子郵件 {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[將分段套用至您的電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md)。

1. 尋找您的電子郵件，選取它並按一下&#x200B;**[!UICONTROL Edit Draft]**&#x200B;標籤。

   ![](assets/three-281-29.jpg)

1. 按一下「**[!UICONTROL Preview]**」。

   ![](assets/1.png)

1. 按一下&#x200B;**[!UICONTROL View By]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL Segmentation]**。

   ![](assets/2.png)

1. 會顯示一個下拉式清單，內含可用的區段。 按一下並選取您想要的。

   ![](assets/3.png)

1. 使用箭頭來捲動您的選項（在此情況下，我們會動態變更主旨行）。

   ![](assets/4.png)

1. 按一下「**[!UICONTROL Send Sample]**」以接收使用中區段的測試電子郵件。

   ![](assets/5.png)

   >[!TIP]
   >
   >您也可以在電子郵件的編輯模式下，根據區段傳送範例電子郵件。 按一下&#x200B;**[!UICONTROL Email Actions]**&#x200B;下拉式清單，選取&#x200B;**[!UICONTROL Send Sample]**，然後選擇您的區段。

在啟動行銷活動之前取樣內容非常重要。 測量兩次，剪下一次！
