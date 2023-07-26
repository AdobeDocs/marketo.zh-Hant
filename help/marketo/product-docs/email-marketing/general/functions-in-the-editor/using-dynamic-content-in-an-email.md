---
unique-page-id: 2950617
description: 在電子郵件中使用動態內容 — Marketo檔案 — 產品檔案
title: 在電子郵件中使用動態內容
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 在電子郵件中使用動態內容 {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[建立細分](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

在電子郵件中使用動態內容來傳送您的潛在客戶目標資訊。

>[!NOTE]
>
>只有當使用「觸發行銷活動」時，才支援在電子郵件中的動態內容中使用變數。 它是 **非** 使用批次行銷活動時支援。

## 新增分段 {#add-segmentation}

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities.png)

1. 選取您的電子郵件並按一下 **編輯草稿**.

   ![](assets/1.2.png)

1. 在此範例中，我們讓主旨列成為動態的。 按一下「主旨」欄位，然後按一下 **設定為動態** 按鈕。

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >您也可以將電子郵件內的元素設為動態。 要執行此操作，請選取區域，按一下齒輪圖示，然後選取 **設定為動態** (或 [取代為代碼片段](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md)，視您正在執行的動作而定)。

1. 輸入區段名稱，選取該名稱，然後按一下 **儲存**.

   ![](assets/1.4.png)

   您的區段及其區段會顯示在右側的「動態」標籤下方。

   ![](assets/1.5.png)

## 套用動態內容 {#apply-dynamic-content}

>[!CAUTION]
>
>允許的動態內容元素數量並非無限制。 雖然沒有特定的數量限制（可能會因內容組合而異），但過度使用動態內容可能會對電子郵件的效能造成負面影響。 我們建議將每封電子郵件的動態內容元素使用量維持在20個以下。

1. 按一下您的區段並新增主旨列。

![](assets/2.1.png)

1. 對每個區段重複。

   ![](assets/2.2.png)

>[!TIP]
>
>將內容套用至各種區段之前，請先建立預設電子郵件。

>[!CAUTION]
>
>對預設區段內容區塊的變更會套用至所有區段。

真貼心！ 現在您可以傳送彈性電子郵件給目標對象。

>[!MORELIKETHIS]
>
>* [預覽包含動態內容的電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [在登入頁面中使用動態內容](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)
