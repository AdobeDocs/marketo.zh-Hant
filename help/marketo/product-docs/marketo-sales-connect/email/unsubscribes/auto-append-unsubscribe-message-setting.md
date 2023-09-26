---
description: 自動附加取消訂閱訊息設定 — Marketo檔案 — 產品檔案
title: 自動附加取消訂閱訊息設定
hide: true
hidefromtoc: true
feature: Marketo Sales Connect
source-git-commit: 8b2eed5e28c46ea9c467fd25dd732c1654a09bed
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 自動附加取消訂閱訊息設定 {#auto-append-unsubscribe-message-setting}

確保每封傳送的電子郵件都包含取消訂閱訊息，讓收件者可以輕鬆選擇退出通訊。 啟用附加取消訂閱訊息後，您的團隊從Marketo Sales傳送的所有通訊都會包含取消訂閱訊息，包括從網頁應用程式、Salesforce、Gmail外掛程式和Outlook外掛程式傳送的電子郵件。

## 注意事項 {#things-to-note}

* 對於從外掛程式傳送的電子郵件，只有當使用範本時才會附加取消訂閱。

* 如果您使用 `{{team_unsubscribe}}` 電子郵件範本中的動態欄位且「取消訂閱訊息附加」設定已啟用時，「專案團隊取消訂閱動態」欄位會填入您的取消訂閱訊息 _而非_ 正在附加您的取消訂閱訊息。

## 啟用/停用取消訂閱附加 {#enable-disable-unsubscribe-append}

1. 按一下齒輪圖示並選取 **設定**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. 在管理設定下，按一下 **取消訂閱**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. 在「訊息」標籤中的「附加取消訂閱訊息」下方，將滑桿移動至所需的狀態。

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>如果您停用附加取消訂閱訊息設定，建議將取消訂閱頁尾新增至您的範本，以確保您的通訊具有選擇退出選項。 若要這麼做，您可以將自己的自訂訊息新增至每個範本，或使用 `{{team_unsubscribe}}` [動態欄位](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"}.
