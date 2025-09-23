---
unique-page-id: 10095554
description: 將表單內嵌至網站行銷活動 — Marketo檔案 — 產品檔案
title: 將表單嵌入至網頁行銷活動中
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 8%

---

# 將表單嵌入至網頁行銷活動中 {#embed-a-form-into-a-web-campaign}

瞭解如何將Marketo表單內嵌至網路行銷活動（對話方塊、在區域或Widget）。

1. 以滑鼠右鍵按一下已核准的表單。 選取「**[!UICONTROL Embed Code]**」。

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. 複製代碼。

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. 在[!DNL Web Personalization]中，移至&#x200B;**[!UICONTROL Web Campaigns]**。

   ![](assets/web-campaigns-hand-7.jpg)

1. 按一下「**[!UICONTROL Create New Campaign]**」。

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. 在RTF編輯器中，按一下HTML圖示。

   ![](assets/five-1.png)

1. 將表單內嵌程式碼貼到[!UICONTROL HTML Source Editor]中。 按一下「**[!UICONTROL Update]**」。

   ![](assets/six-1.png)

1. 該表單不會顯示在編輯器檢視中，但您可以預覽該表單，以檢視其在行銷活動中的呈現方式。

1. 按一下&#x200B;**[!UICONTROL Launch]**&#x200B;以開始行銷活動。

   >[!NOTE]
   >
   >對表單欄位所做的任何變更，都必須在編輯表單草稿的Marketo行銷活動中完成。

## 將背景影像新增至表單的三種方式 {#three-ways-to-add-a-background-image-to-a-form}

若要將背景影像新增至表單，您可以：

* 編輯表單主題的 CSS
* 在Set Campaign中變更對話方塊或Widget顏色
* 將CSS程式碼新增至指令碼

若要編輯表單主題的CSS，請參閱[本文章](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)。

若要變更「設定促銷活動」中的對話方塊或Widget顏色：

1. 在RTF編輯器中，選取對話方塊促銷活動型別和對話方塊樣式、標題顏色和背景顏色，以自訂表單的背景顏色。 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. 以下範例說明「現代修剪對話方塊樣式」搭配淺紫色標題與背景顏色的外觀。

   ![](assets/image2015-12-29-18-3a27-3a31.png)

若要將CSS程式碼新增至指令碼：

1. 在RTF編輯器中，按一下HTML圖示。

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. 將含有背景樣式程式碼的表單內嵌程式碼貼到[!UICONTROL HTML Source Editor]中。 按一下「**[!UICONTROL Update]**」。

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. 按一下&#x200B;**[!UICONTROL Preview]**&#x200B;以檢視它如何在行銷活動中呈現（該表單不會顯示在編輯器檢視中）。 以下範例說明上述表單程式碼如何在具有背景影像的行銷活動中轉譯。

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [編輯表單主題的CSS](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [顯示沒有後續登陸頁面的感謝訊息](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Forms 2.0](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/javascriptapi/forms-api-reference)
