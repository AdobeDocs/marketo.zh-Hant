---
unique-page-id: 10095554
description: 將表單內嵌至Web Campaign - Marketo檔案 — 產品檔案
title: 將表單內嵌至網頁行銷活動
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# 將表單內嵌至網頁行銷活動 {#embed-a-form-into-a-web-campaign}

了解如何將Marketo表單內嵌至網頁促銷活動（對話方塊、區域或介面工具集）。

1. 以滑鼠右鍵按一下已核准的表單。 選擇 **內嵌程式碼**.

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. 復製程式碼。

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. 在Web個人化中，前往 **網路行銷活動**.

   ![](assets/web-campaigns-hand-7.jpg)

1. 按一下 **建立新促銷活動**.

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. 在RTF編輯器中，按一下HTML圖示。

   ![](assets/five-1.png)

1. 將表單內嵌程式碼貼到HTML原始碼編輯器中。 按一下 **更新**.

   ![](assets/six-1.png)

1. 表單不會顯示在編輯器檢視中，但您可以預覽它，以查看它在促銷活動中的呈現方式。

1. 按一下 **Launch** 來啟動促銷活動。

   >[!NOTE]
   >
   >表單欄位的任何變更都必須在Marketo的「編輯表單草稿的行銷活動」中完成。

## 將背景影像新增至表單的三種方式 {#three-ways-to-add-a-background-image-to-a-form}

若要將背景影像新增至表單，您可以：

* 編輯表單主題的CSS
* 在「設定促銷活動」中變更對話方塊或介面工具集顏色
* 將CSS程式碼新增至指令碼

若要編輯表單主題的CSS，請參閱 [這篇文章](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md).

若要在「設定促銷活動」中變更對話方塊或介面工具集顏色：

1. 在RTF編輯器中，選取「對話」促銷活動類型和對話方塊樣式、標題顏色和背景顏色，以自訂表單的背景顏色。 按一下 **儲存**.

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. 以下範例說明現代修剪對話方塊樣式如何以淡紫色標題和背景顏色顯示。

   ![](assets/image2015-12-29-18-3a27-3a31.png)

若要將CSS程式碼新增至指令碼：

1. 在RTF編輯器中，按一下HTML圖示。

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. 將含有背景樣式程式碼的表單內嵌程式碼貼到HTML原始碼編輯器中。 按一下 **更新**.

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. 按一下 **預覽** 它可檢視其在促銷活動中的呈現方式（表單不會顯示在編輯器檢視中）。 以下範例說明上述表單程式碼如何在具有背景影像的促銷活動中轉譯。

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [編輯表單主題的CSS](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [不顯示後續登錄頁面而顯示感謝訊息](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Forms 2.0](https://developers.marketo.com/documentation/websites/forms-2-0/)

