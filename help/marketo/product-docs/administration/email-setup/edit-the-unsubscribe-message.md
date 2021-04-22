---
unique-page-id: 2360251
description: 編輯取消訂閱訊息-Marketo檔案——產品檔案
title: 編輯取消訂閱訊息
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# 編輯取消訂閱消息{#edit-the-unsubscribe-message}

>[!NOTE]
>
>**需要管理員權限**

當您傳送行銷電子郵件（非[operational](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)）時，取消訂閱文字和連結會附加至底部。 您可以變更預設值。 這是方法。

## 編輯取消訂閱消息{#edit-the-unsubscribe-message-1}

1. 在&#x200B;**Admin**&#x200B;下，按一下&#x200B;**電子郵件**。

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >下列變數很重要。 不要刪除！
   >
   >* **%mkt_opt_out_prefix%**
   >* **mkt_unsubscribe=1&amp;mkt_tok=##MKT_TOK##**


1. 編輯&#x200B;**取消訂閱HTML**&#x200B;和&#x200B;**取消訂閱文字**&#x200B;版本，然後按一下&#x200B;**儲存變更**。

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   給你。 _一定要測試！_ 您不希望行銷電子郵件中斷取消訂閱連結。

>[!TIP]
>
>您可以使用[Token](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)自訂取消訂閱HTML在電子郵件中的位置。

## 預設取消訂閱文本{#default-unsubscribe-text}

如果您需要回復為預設系統取消訂閱，請複製／貼上以下內容：

取消訂閱HTML:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>`取消訂閱文字：
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[編輯「以網頁形式檢視」訊息](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
