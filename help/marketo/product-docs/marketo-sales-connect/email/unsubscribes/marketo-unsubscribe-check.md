---
unique-page-id: 18317340
description: Marketo取消訂閱檢查 — Marketo檔案 — 產品檔案
title: Marketo取消訂閱檢查
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Marketo取消訂閱檢查 {#marketo-unsubscribe-check}

Marketo取消訂閱檢查會使用您團隊與Marketo的連線，以防止電子郵件傳送給在Marketo的銷售機會管理系統中取消訂閱的人。 當銷售使用者使用Sales Connect傳送電子郵件時，將會對Marketo進行API呼叫，以檢查電子郵件ID是否已取消訂閱。 如果是，我們會封鎖電子郵件的傳送。

>[!NOTE]
>
>**需要管理員許可權**

## 開啟 {#turning-it-on}

1. 在網頁應用程式中，按一下齒輪圖示並選取 **設定**.

   ![](assets/one-2.png)

1. 在「管理設定」底下，按一下 **取消訂閱**.

   ![](assets/two-3.png)

1. 按一下 **整合**.

   ![](assets/three-3.png)

1. 在Marketo取消訂閱檢查區段中，按一下滑桿以啟動檢查。

   ![](assets/four-2.png)

## 須知事項 {#things-to-know}

Marketo取消訂閱檢查……

* 不會計入API限制中
* 需要建立Marketo連線
* 是全域設定
* 封鎖從Web應用程式、電子郵件使用者端和Salesforce傳送的電子郵件
* 將記錄失敗的電子郵件，或在使用者嘗試傳送所有工作流程（電子郵件外掛程式傳送、個人傳送、銷售行銷活動傳送、多重選取和傳送）時阻止傳送，但 [群組電子郵件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md)，藉此我們將防止電子郵件以無訊息傳送
