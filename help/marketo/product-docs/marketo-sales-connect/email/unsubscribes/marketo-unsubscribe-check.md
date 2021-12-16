---
unique-page-id: 18317340
description: Marketo取消訂閱檢查 — Marketo檔案 — 產品檔案
title: Marketo取消訂閱檢查
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
source-git-commit: 82c75d52caf3a0320cd3e8534b3b0870cf12d660
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Marketo取消訂閱檢查 {#marketo-unsubscribe-check}

Marketo取消訂閱檢查會使用您的團隊與Marketo的連線，防止電子郵件傳送給在Marketo銷售機會管理系統中取消訂閱的人。 當銷售使用者透過Sales Connect傳送電子郵件時，會向Marketo發出API呼叫，以檢查電子郵件ID是否已取消訂閱。 如果是，我們會封鎖電子郵件的傳送。

>[!NOTE]
>
>**需要管理權限**

## 開啟它 {#turning-it-on}

1. 在Web應用程式中，按一下齒輪圖示並選取 **設定**.

   ![](assets/one-2.png)

1. 在「管理設定」下，按一下 **取消訂閱數**.

   ![](assets/two-3.png)

1. 按一下 **整合**.

   ![](assets/three-3.png)

1. 在「Marketo取消訂閱檢查」區段中，按一下滑桿以啟動檢查。

   ![](assets/four-2.png)

## 須知 {#things-to-know}

Marketo取消訂閱支票……

* 不會計入您的API限制
* 需要建立Marketo連線
* 是全域設定
* 阻止從Web應用程式、電子郵件客戶端和Salesforce發送的電子郵件
* 會記錄失敗的電子郵件，或在使用者嘗試針對所有工作流程（電子郵件外掛程式傳送、個別傳送、銷售促銷活動傳送、多個選取和傳送）傳送時，阻止他們傳送，除 [群組電子郵件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md)，我們將防止電子郵件無訊息傳送
