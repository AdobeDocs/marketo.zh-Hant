---
unique-page-id: 2360253
description: 自訂「管理員電子郵件」中的「以網頁連結文字檢視」和「HTML」，同時保持所需變數不變。
title: 編輯「以網頁形式檢視」訊息
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
source-git-commit: df76402e5fb0c002afeb04d41c52801be67a7136
workflow-type: tm+mt
source-wordcount: '153'
ht-degree: 31%

---

# 編輯「以網頁形式檢視」訊息 {#edit-the-view-as-web-page-message}

瞭解如何編輯[以網頁](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)檢視的文字。

>[!NOTE]
>
>**需要管理員權限**

## 編輯「以網頁形式檢視」訊息 {#edit-the-view-as-web-page-message-1}

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. 按一下「**[!UICONTROL Email]**」。

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >下列變數至關重要。 請勿刪除它們！
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >第二部分`##MKT_TOK##`是該人員的[!UICONTROL Munchkin] Cookie。 這樣可確保他們在按一下連結時受到適當的追蹤。

1. 編輯您喜歡的&#x200B;**[!UICONTROL View as Web Page HTML]**&#x200B;和&#x200B;**[!UICONTROL View as Web Page Text]**&#x200B;版本，然後按一下&#x200B;**[!UICONTROL Save Changes]**。

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>請務必避免：
>
>* 在任一HTML方塊中新增其他URL
>* 將HTML放在文字版本中

傳送測試電子郵件以驗證格式。

## 預設「以網頁檢視」文字 {#default-view-as-web-page-text}

如果您需要還原至預設系統&quot;[!UICONTROL View as Web Page]&quot;，請複製/貼上下列專案：

**[!UICONTROL View as Web Page HTML]**:

`<div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div>`

**[!UICONTROL View as Web Page Text]**:

若要以網頁的形式檢視此電子郵件，請前往下列地址：
`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
