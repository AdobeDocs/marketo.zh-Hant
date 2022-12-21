---
description: Marketo取消訂閱檢查 — Marketo檔案 — 產品檔案
title: Marketo取消訂閱檢查
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Marketo取消訂閱檢查 {#marketo-unsubscribe-check}

Marketo取消訂閱檢查會使用您的團隊與Marketo的連線，防止電子郵件傳送給在Marketo銷售機會管理系統中取消訂閱的人。 當銷售使用者傳送含有Marketo Sales的電子郵件時，會向Marketo發出API呼叫，以檢查電子郵件ID是否已取消訂閱。 如果是，我們會封鎖電子郵件的傳送。

>[!NOTE]
>
>**需要管理權限**

## 開啟它 {#turning-it-on}

1. 按一下齒輪圖示並選取 **設定**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. 在「管理設定」下，按一下 **取消訂閱數**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. 按一下 **整合** 標籤。 在「Marketo取消訂閱檢查」區段中，按一下滑桿以啟動檢查。

   ![](assets/marketo-unsubscribe-check-3.png)

## 須知 {#things-to-know}

Marketo取消訂閱支票……

* 不會計入您的API限制
* 需要建立Marketo連線
* 是全域設定
* 阻止從Web應用程式、電子郵件客戶端和Salesforce發送的電子郵件
