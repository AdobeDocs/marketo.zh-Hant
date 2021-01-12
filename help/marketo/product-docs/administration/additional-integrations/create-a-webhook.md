---
unique-page-id: 2360360
description: 建立網頁掛接——行銷檔案——產品檔案
title: 建立網頁掛接
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---


# 建立Webhook {#create-a-webhook}

使用網頁勾點，運用協力廠商的Web服務來傳送文字訊息、擴充人員資料等。

>[!AVAILABILITY]
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請洽詢您的銷售代表。

1. 前往&#x200B;**Admin**，然後按一下&#x200B;**Webhooks**。

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. 按一下「**新建Webhook**」。

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. 命名並設定您的網頁掛接。

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >這通常包括以URL參數或在POST範本中輸入您的協力廠商服務認證。

   * **URL**:輸入您用來將請求張貼至Web服務的URL。若要在您的請求中插入Token，例如人員的電子郵件地址(**`{{lead.Email Address}}`**)，請按一下「插入Token」（插入Token）**。**

   * **範本**:如果要在POST正文中傳輸資訊，請輸入模板。使用任何支援HTTP POST的資料格式，包括XML、JSON或SOAP。 若要在範本中插入Token，請按一下「插入Token **」。**

   * **請求代號編碼**:如果Token值包含特殊字元（例如&amp;符號、&#39;&amp;&#39;），請指出您請求的格式(**** JSON或 **Form/Url**)。

   * **回應類型**:選取您從服務(**** JSON或 **XML**)收到的回應格式。

   按一下「建立」。

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>從[webhooks](http://developers.marketo.com/documentation/webhooks/)深入探討進一步瞭解。
