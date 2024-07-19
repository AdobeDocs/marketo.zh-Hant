---
unique-page-id: 2360360
description: 建立 [!DNL Webhook] - Marketo檔案 — 產品檔案
title: 建立 [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
source-git-commit: 23a7b8cb1cd07c0194c08d30218602a52d03df5b
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# 建立[!DNL Webhook] {#create-a-webhook}

使用[!DNL Webhooks]以利用協力廠商網站服務來傳送簡訊、擴充個人資料等。

1. 移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區域。

   ![](assets/create-a-webhook-1.png)

1. 按一下&#x200B;**[!UICONTROL Webhooks]**。

   ![](assets/create-a-webhook-2.png)

1. 按一下&#x200B;**[!UICONTROL 新增Webhook]**。

   ![](assets/create-a-webhook-3.png)

1. 命名並設定您的[!DNL Webhook]。

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >這通常包括以URL引數或POST範本的形式輸入您的協力廠商服務認證。

   * **[!UICONTROL URL]**：輸入您在向Web服務提出的要求中使用的URL。 若要在您的要求中插入權杖，例如人員的電子郵件地址(**`{{lead.Email Address}}`**)，請按一下[插入Token] **[!UICONTROL 。]**

   * **[!UICONTROL 範本]**：如果您想要在要求內文中傳輸資訊，請透過裝載範本輸入。 允許用於以下請求型別的範本：POST、DELETE、PATCH或PUT。 您可以使用JSON或XML等資料格式。 若要在範本中插入權杖，請按一下[插入Token] ****。

   * **[!UICONTROL 要求權杖編碼]**：如果權杖值包含特殊字元（例如&amp;符號、&#39;&amp;&#39;），請指出您要求的格式（**JSON**&#x200B;或&#x200B;**表單/URL**）。

   * **[!UICONTROL 回應型別]**：選取您從服務收到的回應格式（**JSON**&#x200B;或&#x200B;**XML**）。

   * **[!UICONTROL 要求型別]**：選取要使用的HTTP方法(DELETE、GET、PATCH、POST、PUT)。

1. 按一下&#x200B;**[!UICONTROL 建立]**。

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>在[[!DNL Webhooks]](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}深入剖析中瞭解更多。
