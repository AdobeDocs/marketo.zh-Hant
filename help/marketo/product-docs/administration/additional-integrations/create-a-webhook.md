---
unique-page-id: 2360360
description: 建立Webhook - Marketo檔案 — 產品檔案
title: 建立網頁連結
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 0%

---

# 建立網頁連結 {#create-a-webhook}

使用Webhook來利用協力廠商Web服務來傳送文字訊息、擴展人員資料等。

>[!AVAILABILITY]
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請連絡您的銷售代表。

1. 前往 **管理** 的上界。

   ![](assets/create-a-webhook-1.png)

1. 按一下 **Webhook**.

   ![](assets/create-a-webhook-2.png)

1. 按一下 **全新Webhook**.

   ![](assets/create-a-webhook-3.png)

1. 命名並設定您的網頁連結。

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >這通常包括以URL參數或POST範本的形式輸入您的協力廠商服務憑證。

   * **URL**:輸入您在向Web服務提出的請求中使用的URL。 插入代號，例如人員的電子郵件地址(**`{{lead.Email Address}}`**)，在您的請求中，按一下 **插入代號**.

   * **範本**:如果要在POST正文中傳輸資訊，請輸入模板。 使用支援HTTPPOST的任何資料格式，包括XML、JSON或SOAP。 若要在範本中插入代號，請按一下 **插入代號**.

   * **請求權杖編碼**:如果代號值包含特殊字元（例如&amp;），請指出請求的格式(**JSON** 或 **表單/URL**)。

   * **回應類型**:選取您從服務收到的回應格式(**JSON** 或 **XML**)。

   * **請求類型**:選取要使用的HTTP方法(DELETE、GET、PATCH、POST、PUT)。

1. 按一下 **建立**。

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>了解更多 [webhook](https://developers.marketo.com/documentation/webhooks/) 深潛。
