---
unique-page-id: 1147352
description: 發送示例電子郵件 — Marketo文檔 — 產品文檔
title: 發送示例電子郵件
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
source-git-commit: 1586b71ec9f9c4f8abc4fd9a3277d5a5f5b88080
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# 發送示例電子郵件 {#send-a-sample-email}

發送電子郵件的樣本既快又容易。 要發送動態內容電子郵件，請參閱 [預覽包含動態內容的電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)。

>[!NOTE]
>
>您必須 **訪問資料庫 — 運行單個流操作** 發送示例電子郵件的權限。

## 發送示例電子郵件 {#send-a-sample-email-1}

1. 查找並選擇您的電子郵件。 按一下 **電子郵件操作** 下拉並選擇 **發送示例**。\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >「My Tokens（我的令牌）」解析為與電子郵件程式相適應的值。

1. 輸入一個或多個電子郵件地址以供遞送。 對於多個電子郵件地址，請使用逗號來分隔它們。 按一下 **發送** 完成。

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >如果輸入多個電子郵件地址，則每個收件人都可以看到這些地址。 輸入的第一個收件人是主收件人，每個後續電子郵件地址都是抄送收件人。

   >[!TIP]
   >
   >如果要將令牌作為特定人解析，請在 **人員下拉** 的子菜單。

## 編輯時發送示例電子郵件 {#send-a-sample-email-while-editing}

1. 查找您的電子郵件，選擇它並按一下 **編輯草稿** 頁籤。

   ![](assets/three-281-29.jpg)

1. 按一下 **電子郵件操作**&#x200B;選中 **發送示例**。

   ![](assets/four.png)

1. 輸入要傳遞的電子郵件地址，然後按一下 **發送**。

   ![](assets/two.png)

   >[!NOTE]
   >
   >觸發器欄位僅適用於那些使用觸發器的 [電子郵件指令碼](https://developers.marketo.com/documentation/velocity-script/)。

## 基於段發送示例電子郵件 {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[將分段應用於電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md)。

1. 查找您的電子郵件，選擇它並按一下 **編輯草稿** 頁籤。

   ![](assets/three-281-29.jpg)

1. 按一下 **預覽**。

   ![](assets/1.png)

1. 按一下 **查看依據** 下拉並選擇 **分段**。

   ![](assets/2.png)

1. 此時將顯示一個帶有可用分段的下拉清單。 按一下它，然後選擇所需的。

   ![](assets/3.png)

1. 使用箭頭滾動查看您的選項（在本例中，我們動態更改了主題行）。

   ![](assets/4.png)

1. 按一下 **發送示例** 接收您所在行動區域的test電子郵件。

   ![](assets/5.png)

   >[!TIP]
   >
   >您還可以在電子郵件的編輯模式下基於段發送示例電子郵件。 按一下 **電子郵件操作** 下拉，選擇 **發送示例**，然後選擇段。

在發起活動之前先對您的內容進行採樣非常重要。 量兩次，剪一次！
