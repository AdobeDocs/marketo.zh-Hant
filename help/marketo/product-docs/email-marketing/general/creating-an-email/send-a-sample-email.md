---
unique-page-id: 1147352
description: 傳送範例電子郵件 — Marketo檔案 — 產品檔案
title: 傳送範例電子郵件
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
feature: Email Editor
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# 傳送範例電子郵件 {#send-a-sample-email}

傳送電子郵件範例既快速又簡單。 若要傳送動態內容電子郵件，請參閱 [預覽包含動態內容的電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>您必須擁有 **Access資料庫 — 執行單一流程動作** 傳送範例電子郵件的許可權。

## 傳送範例電子郵件 {#send-a-sample-email-1}

1. 尋找並選取您的電子郵件。 按一下 **電子郵件動作** 下拉式清單並選取 **傳送範例**.\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >我的Token會解析為適用於電子郵件程式的值。

1. 輸入一或多個要傳送的電子郵件地址。 如果有多個電子郵件地址，請使用逗號來區隔。 按一下 **傳送** 完成時。

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >如果您輸入多個電子郵件地址，則每個收件者都會看到這些地址。 第一個輸入的是主要收件者，後續的每個電子郵件地址都是副本收件人。

   >[!TIP]
   >
   >如果您想要以特定人員身分解析權杖，請在 **人員下拉式清單** 在步驟2中。

## 編輯時傳送範例電子郵件 {#send-a-sample-email-while-editing}

1. 尋找您的電子郵件，選取它並按一下 **編輯草稿** 標籤。

   ![](assets/three-281-29.jpg)

1. 按一下 **電子郵件動作**，選取 **傳送範例**.

   ![](assets/four.png)

1. 輸入傳遞的電子郵件地址，然後按一下 **傳送**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >觸發欄位僅適用於使用下列專案的使用者： [電子郵件指令碼](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting).

## 根據區段傳送範例電子郵件 {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[將區段套用至您的電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. 尋找您的電子郵件，選取它並按一下 **編輯草稿** 標籤。

   ![](assets/three-281-29.jpg)

1. 按一下 **預覽**.

   ![](assets/1.png)

1. 按一下 **檢視方式** 下拉式清單並選取 **細分**.

   ![](assets/2.png)

1. 會顯示一個下拉式清單，內含可用的區段。 按一下並選取您想要的。

   ![](assets/3.png)

1. 使用箭頭來捲動您的選項（在此情況下，我們會動態變更主旨行）。

   ![](assets/4.png)

1. 按一下 **傳送範例** 以接收您作用中區段的測試電子郵件。

   ![](assets/5.png)

   >[!TIP]
   >
   >您也可以在電子郵件的編輯模式下，根據區段傳送範例電子郵件。 按一下 **電子郵件動作** 下拉式清單，選取 **傳送範例**，然後選擇您的區段。

在啟動行銷活動之前取樣內容非常重要。 測量兩次，剪下一次！
