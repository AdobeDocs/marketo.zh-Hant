---
unique-page-id: 2360360
description: 在Admin中建立Webhook，以呼叫簡訊、人員資料等的協力廠商網站服務。
title: 建立 [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
TQID: https://experienceleague.adobe.com/O4xw1wSvFeTJ2xqZn4Eo7JbrUBQQmKcl7mvLkduFXGc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: fc9b09fe-b844-4544-887b-e420c3b82065
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 202
ht-degree: 3%

---

# 建立[!DNL Webhook] {#create-a-webhook}

使用[!DNL Webhooks]以利用協力廠商網站服務來傳送簡訊、擴充個人資料等。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/create-a-webhook-1.png)

1. 按一下「**[!UICONTROL Webhooks]**」。

   ![](assets/create-a-webhook-2.png)

1. 按一下「**[!UICONTROL New Webhook]**」。

   ![](assets/create-a-webhook-3.png)

1. 命名並設定您的[!DNL Webhook]。

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >這通常包括以URL引數或在POST範本中輸入您的協力廠商服務認證。

   * **[!UICONTROL URL]**：輸入您在對Web服務的要求中使用的URL。 若要在您的要求中插入權杖，例如人員的電子郵件地址(**`{{lead.Email Address}}`**)，請按一下&#x200B;**[!UICONTROL Insert Token]**。

   * **[!UICONTROL Template]**：如果您想要在要求內文中傳輸資訊，請透過裝載範本輸入。 以下請求型別允許的範本：POST、DELETE、PATCH或PUT。 您可以使用JSON或XML等資料格式。 若要在範本中插入權杖，請按一下&#x200B;**[!UICONTROL Insert Token]**。

   * **[!UICONTROL Request Token Encoding]**：如果權杖值包含特殊字元（例如&amp;符號），請指出您要求的格式（**JSON**&#x200B;或&#x200B;**表單/URL**）。

   * **[!UICONTROL Response type]**：選取您從服務收到的回應格式（**JSON**&#x200B;或&#x200B;**XML**）。

   * **[!UICONTROL Request Type]**：選取要使用的HTTP方法(DELETE、GET、PATCH、POST、PUT)。

1. 按一下「**[!UICONTROL Create]**」。

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>深入瞭解[[!DNL Webhooks]](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}。
