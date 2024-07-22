---
unique-page-id: 2360251
description: 編輯取消訂閱訊息 — Marketo檔案 — 產品檔案
title: 編輯取消訂閱訊息
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# 編輯取消訂閱訊息 {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**需要管理員許可權**

當您傳送行銷電子郵件（非[可操作](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)）時，取消訂閱文字和連結會附加至底部。 您可以變更預設值。 方法如下。

## 在何處進行編輯 {#where-to-make-the-edit}

1. 移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區段。

   ![](assets/edit-the-unsubscribe-message-1.png)

1. 按一下&#x200B;**[!UICONTROL 電子郵件]**。

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >下列變數至關重要。 請勿刪除它們！
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. 編輯您喜歡的&#x200B;**[!UICONTROL 取消訂閱HTML]**&#x200B;和&#x200B;**[!UICONTROL 取消訂閱文字]**&#x200B;版本，然後按一下&#x200B;**[!UICONTROL 儲存變更]**。

   ![](assets/edit-the-unsubscribe-message-3.png)

   您有。 _請確定測試！_&#x200B;您不希望行銷電子郵件有已中斷的取消訂閱連結。

>[!TIP]
>
>您可以使用[代號](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)來自訂電子郵件中取消訂閱HTML的位置。

## 預設取消訂閱文字 {#default-unsubscribe-text}

如果您需要恢復為預設系統取消訂閱，請複製/貼上以下內容：

[!UICONTROL 取消訂閱HTML]：
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` [!UICONTROL 取消訂閱文字]：
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[編輯[以網頁檢視]訊息](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
