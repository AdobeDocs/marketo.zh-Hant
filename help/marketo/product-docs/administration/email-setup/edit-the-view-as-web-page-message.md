---
unique-page-id: 2360253
description: 編輯「檢視為網頁」訊息——行銷人員檔案——產品檔案
title: 編輯「以網頁形式檢視」訊息
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# 編輯「以網頁形式檢視」訊息 {#edit-the-view-as-web-page-message}

如果您需要編輯「以網頁 [形式檢視](../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)」文字，請以下說明方式。

>[!NOTE]
>
>**需要管理員權限**

## 編輯「以網頁形式檢視」訊息 {#edit-the-view-as-web-page-message-1}

1. 在「管 **理員**」下，按一 **下「電子郵件**」。

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >下列變數很重要。 不要刪除！
   >
   >    
   >    
   >    * %mkt_webview_url%?mkt_tok=##MKT_TOK##
   >    
   >    
   >第二部分##MKT_TOK##是該人的Munchkin Cookie。 如此可確保當他們按一下連結時，會適當地獲得Cookie。

1. 依您 **的喜好編輯「以網頁檢視** HTML」和「以網頁檢視文字**版本」，然後按一下「儲 **存變更」**。

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>請務必避免：
>
>* 新增其他URL至任一HTML方塊
>* 將HTML放入文字版本

>



給你。 寄出測試電子郵件，以確保格式化。

## 預設「檢視為網頁」文字 {#default-view-as-web-page-text}

如果您需要回復到預設系統「View as Web Page」（以網頁形式查看），請複製／貼上以下內容：

**檢視為網頁HTML:**`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>` **檢視為網頁文字：**

若要以網頁形式檢視此電子郵件，請前往下列地址：`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>` 砰！ 你完了。
