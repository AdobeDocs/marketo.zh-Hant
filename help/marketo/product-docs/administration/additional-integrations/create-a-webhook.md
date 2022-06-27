---
unique-page-id: 2360360
description: 建立網頁掛接 — Marketo文檔 — 產品文檔
title: 建立網頁掛接
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 25a574719eb6c064d33b6a1cebafe2668ed1330d
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# 建立網頁掛接 {#create-a-webhook}

使用Webhooks利用第三方Web服務發送文本消息、擴展人員資料等。

>[!AVAILABILITY]
>
>並非所有客戶都購買了此功能。 請與銷售代表聯繫以瞭解詳細資訊。

1. 轉到 **管理** 按一下 **網鈎**。

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. 按一下 **新建Webhook**。

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. 命名並配置網路掛接。

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >這通常包括將第三方服務憑據作為URL參數輸入，或在POST模板中輸入。

   * **URL**:輸入在請求Web服務時使用的URL。 插入令牌，如人員的電子郵件地址(**`{{lead.Email Address}}`**)，在您的請求中，按一下 **插入標籤**。

   * **模板**:如果要在POST正文中傳輸資訊，請輸入模板。 使用支援HTTPPOST的任何資料格式，包括XML、JSON或SOAP。 要在模板中插入令牌，請按一下 **插入標籤**。

   * **請求令牌編碼**:如果令牌值包含特殊字元（如「&amp;」和符號），請指示請求的格式(**JSON** 或 **窗體/URL**)。

   * **響應類型**:選擇從服務接收的響應的格式(**JSON** 或 **XML**)。

   * **請求類型**:選擇要使用的HTTP方法(DELETE、GET、PATCH、POST、PUT)。

   按一下 **建立**。

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>在 [網鈎](https://developers.marketo.com/documentation/webhooks/) 深潛。
