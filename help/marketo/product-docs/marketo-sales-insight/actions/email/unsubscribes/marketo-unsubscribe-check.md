---
description: Marketo取消訂閱檢查 — Marketo檔案 — 產品檔案
title: Marketo取消訂閱檢查
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Marketo取消訂閱檢查 {#marketo-unsubscribe-check}

Marketo取消訂閱檢查會使用您團隊與Marketo的連線，防止電子郵件傳送給在Marketo的銷售機會管理系統中取消訂閱的人。 當銷售使用者傳送包含Marketo Sales的電子郵件時，將會對Marketo進行API呼叫，以檢查電子郵件ID是否已取消訂閱。 如果是，我們將封鎖電子郵件的傳送。

>[!NOTE]
>
>**需要管理員許可權**

## 開啟 {#turning-it-on}

1. 按一下齒輪圖示並選取 **設定**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. 在管理設定下，按一下 **取消訂閱**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. 按一下 **整合** 標籤。 在Marketo取消訂閱檢查區段中，按一下滑桿以啟動檢查。

   ![](assets/marketo-unsubscribe-check-3.png)

## 須知 {#things-to-know}

Marketo取消訂閱檢查……

* 不會計入API限制中
* 需要建立Marketo連線
* 是全域設定
* 封鎖從網頁應用程式、電子郵件使用者端和Salesforce傳送的電子郵件
