---
description: Marketo取消訂閱檢查 — Marketo文檔 — 產品文檔
title: Marketo取消訂閱支票
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Marketo取消訂閱支票 {#marketo-unsubscribe-check}

「Marketo取消訂閱檢查」使用您的團隊與Marketo的聯繫，防止電子郵件發給在Marketo的Lead Management系統中未訂閱的人。 當銷售用戶向Marketo銷售部門發送電子郵件時，將向Marketo發出API調用，以檢查電子郵件ID是否未訂閱。 如果是，我們將阻止發送電子郵件。

>[!NOTE]
>
>**需要管理權限**

## 開啟 {#turning-it-on}

1. 按一下齒輪表徵圖並選擇 **設定**。

   ![](assets/marketo-unsubscribe-check-1.png)

1. 在「Admin Settings（管理設定）」下，按一下 **取消訂閱**。

   ![](assets/marketo-unsubscribe-check-2.png)

1. 按一下 **整合** 頁籤。 在「Marketo取消訂閱檢查」部分，按一下滑塊以激活檢查。

   ![](assets/marketo-unsubscribe-check-3.png)

## 要知道的事 {#things-to-know}

Marketo取消訂閱支票……

* 不計入API限制
* 需要建立Marketo連接
* 是全局設定
* 阻止從Web應用程式、電子郵件客戶端和Salesforce發送的電子郵件
