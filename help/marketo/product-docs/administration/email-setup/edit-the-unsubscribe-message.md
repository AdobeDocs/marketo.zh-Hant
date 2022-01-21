---
unique-page-id: 2360251
description: 編輯取消訂閱消息 — Marketo文檔 — 產品文檔
title: 編輯取消訂閱消息
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
source-git-commit: 931b42d7266b9c57308567527042dfcad9847993
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 編輯取消訂閱消息 {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**需要管理權限**

當您發送市場營銷電子郵件時(非[操作](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md))，取消訂閱文本和連結將附加到底部。 您可以更改預設值。 這是方法。

## 編輯取消訂閱消息 {#edit-the-unsubscribe-message-1}

1. 下 **管理**&#x200B;按一下 **電子郵件**。

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >以下變數至關重要。 不要刪除它們！
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`


1. 編輯 **取消訂閱HTML** 和 **取消訂閱文本** 按 **保存更改**。

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   給你。 _一定要test!_ 您不希望您的營銷電子郵件中斷了取消訂閱連結。

>[!TIP]
>
>您可以使用 [令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)。

## 預設取消訂閱文本 {#default-unsubscribe-text}

如果您需要恢復為預設系統取消訂閱，請複製/貼上以下內容：

取消訂閱HTML:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` 取消訂閱文本：
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[編輯「作為網頁查看」消息](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
