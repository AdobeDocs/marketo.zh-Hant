---
unique-page-id: 7514956
description: 為網頁多媒體啟用預測性內容 — Marketo檔案 — 產品檔案
title: 為網頁多媒體啟用預測性內容
exl-id: 030f1dd7-8fe7-4c82-be5e-052f0a259e3c
feature: Predictive Content
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# 為網頁多媒體啟用預測性內容 {#enable-predictive-content-for-web-rich-media}

預測性內容透過機器學習和預測性分析，讓您的網頁訪客獲得最相關的內容。 使用Web Rich Media，您可以透過文字說明和影像來增強內容，並在網站上嵌入多個預測性內容建議。

>[!NOTE]
>
>在測試和使用預測性內容之前，建議您為每個類別和每個來源（電子郵件、豐富媒體、長條）啟用超過五個內容。 更多內容可為您提供更好的預測性結果。

>[!PREREQUISITES]
>
>在啟用預測性內容之前，您必須：
>
>* **準備您的預測性內容**
>
>   * [編輯電子郵件的預測性內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"}或
>   * [編輯多媒體預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"}或
>   * [編輯建議列的預測性內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [核准預測性內容的標題](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

準備好豐富媒體的內容標題、說明和影像後，您就可以啟用個別或多個內容片段。

1. 若要啟用個別標題，請按一下標題以開啟編輯器。 按一下「豐富型媒體」，然後勾選「**啟用豐富型媒體中的預測性內容**」方塊，並按一下「儲存&#x200B;**」**。

   ![](assets/image2017-10-3-9-3a50-3a29.png)

1. 針對多個內容，在&#x200B;**預測性內容**&#x200B;頁面上，勾選標題旁的方塊。

   ![](assets/image2017-10-3-10-3a0-3a42.png)

1. 按一下&#x200B;**內容動作**&#x200B;下拉式清單，然後選取&#x200B;**啟用Web Rich Media**。

   ![](assets/image2017-10-3-10-3a2-3a6.png)|

## 自訂Javascript程式碼並將其內嵌至您的網站  {#customize-the-javascript-code-and-embed-it-into-your-website}

請參閱Marketo開發人員網站[&#128279;](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/rich-media-recommendation){target="_blank"}上Rich Media Recommendation範本的檔案。 以下說明如何自訂網站的範本。

將JavaScript程式碼貼入網站中您要顯示範本的位置。

**範本範例**

* 範本1：三個水準內容片段，包含影像、標題和說明
* 範本2：三個垂直內容片段，包含影像、標題和說明

以下是Rich Media建議範本1的範例：

![](assets/image2015-6-1-17-3a8-3a33.png)

以下是Rich Media建議範本2的範例：

![](assets/image2015-12-20-10-3a35-3a12.png)
