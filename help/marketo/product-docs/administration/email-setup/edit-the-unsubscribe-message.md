---
unique-page-id: 2360251
description: 編輯取消訂閱訊息——行銷人員檔案——產品檔案
title: 編輯取消訂閱訊息
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# 編輯取消訂閱訊息 {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**需要管理員權限**

當您傳送行銷電子郵件(非 [運作](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md))時，取消訂閱文字和連結會附加至底部。 您可以變更預設值。 這是方法。

## 編輯取消訂閱訊息 {#edit-the-unsubscribe-message-1}

1. 在「管 **理員**」下，按一 **下「電子郵件**」。

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >
   >下列變數很重要。 不要刪除！
   >
   >    
   >    
   >    * **%mkt_opt_out_prefix%**
   >    * **mkt_unsubscribe=1&amp;mkt_tok=##MKT_TOK##**


1. 依您的喜 **好編輯「取消訂閱HTML** 」和「取消訂閱文字版本 **」，然後按一下「** 儲存變更」 ****。

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   給你。 **一定要測試！** 您不希望行銷電子郵件中斷取消訂閱連結。

>[!TIP]
>
>您可以使用Token，自訂取消訂閱HTML在電子郵件中的 [位置](../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)。

## 預設取消訂閱文字 {#default-unsubscribe-text}

如果您需要回復為預設系統取消訂閱，請複製／貼上以下內容：

取消訂閱HTML:`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` 取消訂閱文字：
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!NOTE]
>
>**相關文章**
>
>* [編輯「以網頁形式檢視」訊息](edit-the-view-as-web-page-message.md)

>



