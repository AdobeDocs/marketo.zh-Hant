---
unique-page-id: 7514956
description: 為Web富媒體啟用預測性內容 — Marketo文檔 — 產品文檔
title: 為Web富媒體啟用預測性內容
exl-id: 030f1dd7-8fe7-4c82-be5e-052f0a259e3c
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# 為Web富媒體啟用預測性內容 {#enable-predictive-content-for-web-rich-media}

預測性內容通過機器學習和預測分析功能，讓您的Web訪問者獲得最相關的內容。 使用Web Rich Media，您可以通過文本描述和影像增強內容，並在網站上嵌入多個預測性內容建議。

>[!NOTE]
>
>建議在測試和使用預測性內容之前，先按類別和每個源啟用五個以上的內容（電子郵件、富媒體、欄）。 更多內容將為您提供更好的預測結果。

>[!PREREQUISITES]
>
>在啟用預測性內容之前，必須：
>
>* **準備預測性內容**
   >
   >   * [編輯電子郵件的預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target=&quot;_blank&quot;或
   >   * [編輯富媒體的預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target=&quot;_blank&quot;或
   >   * [編輯建議欄的預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target=&quot;_blank&quot;
>
>* [批准預測內容的標題](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target=&quot;_blank&quot;


一旦為富媒體準備了內容標題、描述和影像，就可以啟用單個或多個內容片段。

1. 要啟用單個標題，請按一下標題以開啟編輯器。 按一下「Rich Media（富媒體）」 ，然後檢查 **為富媒體中的預測性內容啟用** 框中，按一下 **保存**。

   ![](assets/image2017-10-3-9-3a50-3a29.png)

1. 對於多個內容，在 **預測內容** 的上界。

   ![](assets/image2017-10-3-10-3a0-3a42.png)

1. 按一下 **內容操作** 下拉並選擇 **啟用Web富媒體**。

   ![](assets/image2017-10-3-10-3a2-3a6.png)|

## 自定義Javascript代碼並將其嵌入到您的網站  {#customize-the-javascript-code-and-embed-it-into-your-website}

請參閱富媒體建議模板的文檔 [在Marketo開發商網站上](https://developers.marketo.com/documentation/websites/rtp-rich-media-recommendations-api){target=&quot;_blank&quot;}。 這說明了如何自定義網站的模板。

將JavaScript代碼貼上到您希望模板出現的位置的網站中。

**模板示例**

* 模板1:包含影像、標題和說明的三個水準內容段
* 模板2:三個包含影像、標題和說明的垂直內容段

以下是富媒體建議模板1的示例：

![](assets/image2015-6-1-17-3a8-3a33.png)

下面是富媒體建議模板2的示例：

![](assets/image2015-12-20-10-3a35-3a12.png)
