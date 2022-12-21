---
unique-page-id: 2359663
description: 設定隱藏的表單欄位值 — Marketo檔案 — 產品檔案
title: 設定隱藏的表單欄位值
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# 設定隱藏的表單欄位值 {#set-a-hidden-form-field-value}

隱藏欄位通常會動態填入。 不會向填寫表單的人顯示。 以下說明如何設定值。

>[!PREREQUISITES]
>
>[將表單欄位設為隱藏](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## 選取欄位 {#select-the-field}

1. 在表單中，選取隱藏欄位並按一下 **編輯** for **自動填充**.

   ![](assets/autofill.png)

## 使用預設值 {#use-default-value}

通過選擇使用預設值，您可以硬編碼特定值，以便在提交此表單時始終使用。 輸入預設值，然後按一下「保存」。

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL參數 {#url-parameter}

如果您想在填寫表單時從人員所在的頁面擷取URL參數（查詢字串），可使用 **URL參數** 填入隱藏欄位。

>[!NOTE]
>
>參數有點技術，不是嗎？ 一旦你得到了它們，它們就會強大。 此 [查詢字串上的維基百科頁面](https://en.wikipedia.org/wiki/Query_string) 有幫助。

1. 選擇 **URL參數** for **獲取值類型**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. 輸入 **參數名稱** 按一下 **儲存**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>您可以輸入預設值，以備找不到URL參數時使用。

## Cookie值 {#cookie-value}

如果您將資料儲存在Cookie中，則可以使用 **Cookie值** 以在提交表單時擷取資料。

1. 選擇 **Cookie值** for **從獲取值**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. 輸入您想要的Cookie參數名稱，然後按一下 **儲存**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >您可以輸入預設值，以備找不到參數/Cookie時使用。

## 反向連結參數 {#referrer-parameter}

如果您想在填寫表單前，從訪客來自的頁面擷取資料，可以使用 **反向連結參數**.

1. 設定 **從獲取值** to **反向連結參數**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. 輸入 **參數名稱** 從反向連結URL中擷取，然後按一下 **儲存**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >您可以輸入 **預設值** 若找不到反向連結參數。

1. 按一下 **完成**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. 按一下 **核准並關閉**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
