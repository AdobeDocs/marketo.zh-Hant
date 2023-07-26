---
unique-page-id: 2360253
description: 編輯「以網頁方式檢視」訊息 — Marketo檔案 — 產品檔案
title: 編輯「以網頁檢視」訊息
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# 編輯「以網頁檢視」訊息 {#edit-the-view-as-web-page-message}

如果您需要編輯&quot;[以網頁檢視](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)「文字，說明如下。

>[!NOTE]
>
>**需要管理員許可權**

## 編輯「以網頁檢視」訊息 {#edit-the-view-as-web-page-message-1}

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. 按一下 **[!UICONTROL 電子郵件]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >下列變數至關重要。 請勿刪除它們！
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >第二部分 `##MKT_TOK##` 是 [!UICONTROL munchkin] 該人員的Cookie。 它會確保他們在按一下連結時獲得適當的編碼。

1. 編輯 **[!UICONTROL 以網頁HTML檢視]** 和 **[!UICONTROL 以網頁文字檢視]** 版本以符合您的喜好並按一下 **[!UICONTROL 儲存變更]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>請務必避免：
>
>* 新增其他URL至其中一個HTML方塊
>* 在文字版本中置入HTML

您有。 傳送測試電子郵件以確保格式化。

## 預設「以網頁檢視」文字 {#default-view-as-web-page-text}

如果您需要還原為預設系統»[!UICONTROL 以網頁檢視]「」，複製/貼上下列內容：

**[!UICONTROL 以網頁HTML檢視]**：

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**[!UICONTROL 以網頁文字檢視]**：

若要以網頁的形式檢視此電子郵件，請前往下列地址：
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

完成了！
