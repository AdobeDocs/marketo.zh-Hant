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

當您傳送行銷電子郵件時(非[營運](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md))，則會將取消訂閱文字和連結附加至底部。 您可以變更預設值。 方法如下。

## 在何處進行編輯 {#where-to-make-the-edit}

1. 前往 **[!UICONTROL 管理員]** 區段。

   ![](assets/edit-the-unsubscribe-message-1.png)

1. 按一下 **[!UICONTROL 電子郵件]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >下列變數相當重要。 不要刪除它們！
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. 編輯 **[!UICONTROL 取消訂閱HTML]** 和 **[!UICONTROL 取消訂閱文字]** 版本以符合您的喜好並按一下 **[!UICONTROL 儲存變更]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   給你。 _請務必測試！_ 您不希望行銷電子郵件中的取消訂閱連結損毀。

>[!TIP]
>
>您可以使用自訂取消訂閱HTML在電子郵件中的位置 [Token](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## 預設取消訂閱文字 {#default-unsubscribe-text}

如果您需要恢復為預設系統取消訂閱，請複製/貼上以下內容：

[!UICONTROL 取消訂閱HTML]：
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` [!UICONTROL 取消訂閱文字]：
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[編輯「以網頁檢視」訊息](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
