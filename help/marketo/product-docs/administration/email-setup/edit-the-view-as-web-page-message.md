---
unique-page-id: 2360253
description: 編輯「檢視為網頁」訊息 — Marketo檔案 — 產品檔案
title: 編輯「以網頁形式檢視」訊息
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# 編輯「以網頁形式檢視」訊息 {#edit-the-view-as-web-page-message}

如果您需要編輯「[以網頁形式檢視](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)「文本，這是方法。

>[!NOTE]
>
>**需要管理權限**

## 編輯「以網頁形式檢視」訊息 {#edit-the-view-as-web-page-message-1}

1. 前往 **管理** 的上界。

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. 按一下 **電子郵件**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >下列變數至關重要。 不要刪除！
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >第二部分 `##MKT_TOK##` 是那個人的munchkin cookie。 這可確保當使用者按一下連結時，會適當地獲得Cookie。

1. 編輯 **以網頁形式檢視HTML** 和 **以網頁文字檢視** 按一下 **儲存變更**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>請務必避免：
>
>* 新增其他URL至任一HTML方塊
>* 將HTML放入文字版本


給你。 傳送測試電子郵件以確保格式設定。

## 預設「以網頁形式檢視」文字 {#default-view-as-web-page-text}

如果您需要回復到預設系統「以網頁形式查看」，請複製/貼上以下內容：

**作為網頁查看HTML:**

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**作為網頁文本查看：**

若要以網頁形式檢視此電子郵件，請前往下列地址：
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

就這樣！
