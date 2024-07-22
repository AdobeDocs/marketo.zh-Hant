---
description: 異動銷售電子郵件範本 — Marketo檔案 — 產品檔案
title: 異動銷售電子郵件範本
feature: Marketo Sales Connect
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# 異動銷售電子郵件範本 {#transactional-sales-email-templates}

如果您的團隊要傳送交易或非商業電子郵件，您可以將電子郵件範本標示為非商業性範本，如此可略過取消訂閱。

## 注意事項 {#things-to-note}

* 非商業電子郵件會略過銷售取消訂閱和[Marketo Engage取消訂閱檢查](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}，但不會略過[封鎖的網域](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md){target="_blank"}。

* 即使[附加取消訂閱訊息管理員設定](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"}已啟用，取消訂閱訊息也不會自動附加至非商業電子郵件。 不過，`{{team_unsubscribe}}` [動態欄位](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"}仍會填入您的團隊取消訂閱訊息。

## 設定非商業用途的電子郵件範本 {#configure-an-email-template-for-non-commercial-use}

1. 在標題中，按一下&#x200B;**範本**。

   ![](assets/transactional-sales-email-templates-1.png)

1. 尋找並選取您要更新的範本。

   ![](assets/transactional-sales-email-templates-2.png)

1. 在「範本設定」底下啟用非商業電子郵件切換。

   ![](assets/transactional-sales-email-templates-3.png)

## 傳送非商業電子郵件 {#send-a-non-commercial-email}

>[!NOTE]
>
>選取取消訂閱的人員時，他們將會反白顯示為橙色。

1. 在標題中，按一下&#x200B;**撰寫**。 尋找並選取所需的非商業範本。

   ![](assets/transactional-sales-email-templates-4.png)

1. 使用者會看到橫幅，顯示他們已選取非商業電子郵件範本。

   ![](assets/transactional-sales-email-templates-5.png)

1. 按一下&#x200B;**傳送**。

   ![](assets/transactional-sales-email-templates-6.png)

即使該人已取消訂閱，仍會傳送電子郵件。
