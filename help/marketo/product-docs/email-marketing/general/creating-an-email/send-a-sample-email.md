---
unique-page-id: 1147352
description: 傳送範例電子郵件 — Marketo檔案 — 產品檔案
title: 傳送範例電子郵件
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
source-git-commit: 1586b71ec9f9c4f8abc4fd9a3277d5a5f5b88080
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# 傳送範例電子郵件 {#send-a-sample-email}

傳送電子郵件範例既快速又簡單。 若要傳送動態內容電子郵件，請參閱 [使用動態內容預覽電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>您必須擁有 **訪問資料庫 — 運行單流操作** 傳送範例電子郵件的權限。

## 傳送範例電子郵件 {#send-a-sample-email-1}

1. 尋找並選取您的電子郵件。 按一下 **電子郵件動作** 下拉式清單並選取 **傳送範例**.\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >我的代號解析到與電子郵件程式相適的值。

1. 輸入要傳送的一或多個電子郵件地址。 若是多個電子郵件地址，請使用逗號加以區隔。 按一下 **傳送** 時才能使用。

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >如果您輸入多個電子郵件地址，每個收件者都會看到這些地址。 輸入的第一個是主要收件者，每個後續電子郵件地址都是CC收件者。

   >[!TIP]
   >
   >如果您想將代號解析為特定人員，請在 **人員下拉式清單** 步驟2.

## 編輯時傳送範例電子郵件 {#send-a-sample-email-while-editing}

1. 找到您的電子郵件，選取它，然後按一下 **編輯草稿** 標籤。

   ![](assets/three-281-29.jpg)

1. 按一下 **電子郵件動作**，選取 **傳送範例**.

   ![](assets/four.png)

1. 輸入要傳送的電子郵件地址，然後按一下 **傳送**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >觸發欄位僅適用於使用 [電子郵件指令碼](https://developers.marketo.com/documentation/velocity-script/).

## 根據區段傳送範例電子郵件 {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[將區段套用至您的電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. 找到您的電子郵件，選取它，然後按一下 **編輯草稿** 標籤。

   ![](assets/three-281-29.jpg)

1. 按一下 **預覽**.

   ![](assets/1.png)

1. 按一下 **檢視依據** 下拉式清單並選取 **區段**.

   ![](assets/2.png)

1. 下拉式清單隨即出現，其中包含可用的區段。 按一下它，然後選取您想要的。

   ![](assets/3.png)

1. 使用箭頭來捲動您的選項（在此案例中，我們會以動態方式變更主旨行）。

   ![](assets/4.png)

1. 按一下 **傳送範例** 接收您區段的測試電子郵件。

   ![](assets/5.png)

   >[!TIP]
   >
   >您也可以根據電子郵件編輯模式中的區段，傳送範例電子郵件。 按一下 **電子郵件動作** 下拉式清單，選取 **傳送範例**，然後選擇您的區段。

啟動促銷活動之前先取樣您的內容非常重要。 測量兩次，剪一次！
