---
unique-page-id: 7514956
description: 為網頁多媒體啟用預測性內容 — Marketo檔案 — 產品檔案
title: 為網頁多媒體啟用預測內容
exl-id: 030f1dd7-8fe7-4c82-be5e-052f0a259e3c
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# 為網頁多媒體啟用預測內容 {#enable-predictive-content-for-web-rich-media}

透過機器學習和預測性分析，預測性內容可讓您的網站訪客接觸到最相關的內容。 透過Web Rich Media，您可以透過文字說明和影像來增強內容，並在網站上嵌入多個預測性內容建議。

>[!NOTE]
>
>建議您在測試和使用預測性內容之前，先為每個類別和每個來源（電子郵件、多媒體和長條）啟用超過五個內容。 更多內容可提供更好的預測性結果。

>[!PREREQUISITES]
>
>在啟用預測性內容之前，您必須：
>
>* **準備您的預測性內容**
>
>   * [編輯電子郵件的預測性內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"} 或
>   * [編輯多媒體預測性內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"} 或
>   * [編輯建議列的預測性內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [核准預測性內容的標題](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

一旦您準備好豐富媒體的內容標題、說明和影像，您就可以啟用個別或多個內容片段。

1. 若要啟用個別標題，請按一下標題以開啟編輯器。 按一下「多媒體」，然後檢查 **啟用多媒體中的預測性內容** 方塊並按一下 **儲存**.

   ![](assets/image2017-10-3-9-3a50-3a29.png)

1. 如需多個內容片段，請前往 **預測性內容** 頁面，勾選標題旁的方塊。

   ![](assets/image2017-10-3-10-3a0-3a42.png)

1. 按一下 **內容動作** 下拉式清單並選取 **為Web多媒體啟用**.

   ![](assets/image2017-10-3-10-3a2-3a6.png)|

## 自訂Javascript程式碼並將其內嵌至您的網站  {#customize-the-javascript-code-and-embed-it-into-your-website}

請參閱多媒體建議範本的檔案 [在Marketo開發人員網站上](https://developers.marketo.com/documentation/websites/rtp-rich-media-recommendations-api){target="_blank"}. 以下說明如何自訂網站的範本。

將JavaScript程式碼貼到您網站中要顯示範本的位置。

**範本範例**

* 範本1：三個水準內容片段，包含影像、標題和說明
* 範本2：三個垂直內容片段，包含影像、頁首和說明

以下是Rich Media建議範本1的範例：

![](assets/image2015-6-1-17-3a8-3a33.png)

以下是Rich Media建議範本2的範例：

![](assets/image2015-12-20-10-3a35-3a12.png)
