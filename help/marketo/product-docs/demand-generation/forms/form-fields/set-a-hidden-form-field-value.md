---
unique-page-id: 2359663
description: 設定隱藏的表單欄位值——行銷檔案——產品檔案
title: 設定隱藏表單欄位值
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# 設定隱藏表單欄位值 {#set-a-hidden-form-field-value}

隱藏欄位通常會動態填入。 不會向填寫表格的人顯示。 以下是如何設定值。

>[!NOTE]
>
>**必要條件**
>
>[將表單欄位設為隱藏](set-a-form-field-as-hidden.md)

## 選擇欄位 {#select-the-field}

1. 在表單中，選取隱藏欄位，然後按一下「 **編輯** 」 **以自動填滿**。

   ![](assets/autofill.png)

## 使用預設值 {#use-default-value}

選取「使用預設值」，您可以硬式編碼特定值，以便在提交此表單時一律使用。 輸入預設值，然後按一下保存。

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL參數 {#url-parameter}

如果您想在填寫表單時從人員所在的頁面擷取URL參數（查詢字串），可以使用 **URL****參數** ，填入隱藏欄位。

>[!NOTE]
>
>參數有點技術化，不是嗎？ 但一旦你得到了它們，它們就變得強大了。 查詢字 [串上的這個維基百科頁面](http://en.wikipedia.org/wiki/Query_string) ，有些幫助。

1. 選取 **「取得值類型** 」 **的「URL參數」**。

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. 輸入「參 **數名稱** 」，然後單 **擊「保存」**。

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>您可以輸入預設值，以備找不到URL參數時使用。

## Cookie值 {#cookie-value}

如果您將資料儲存在Cookie中，則可以使用 **Cookie****值** ，在提交表單時擷取資料。

1. 選擇 **Cookie****的** Value **for** Get **Value Cookie****** From Throm

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. 輸入您想要的Cookie參數名稱，然後按一下「 **儲存**」。

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >您可以輸入預設值，以備找不到參數/Cookie時使用。

## 反向連結參數 {#referrer-parameter}

如果您想在填寫表單之前，從訪客來自的頁面擷取資料，可以使用「反向連 **結****參數」**。

1. 設 **定從Get** **From** To **Referrer Paremert Prameters(從反向連結到參**********&#x200B;數參數)。

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. 輸入您 **要從反向連結URL擷取的參數名稱** ，然後按一下「 **儲存」**。

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >您可以輸入 **Default** **Value** （預設值），以防找不到反向連結參數。

1. 按一 **下完成**。

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. 按一 **下「核准並關閉**」。

   ![](assets/image2014-9-15-13-3a10-3a43.png)

真貼心！ 你幹得不錯。 有更多表格相關資 [訊](http://docs.marketo.com/display/docs/forms)。
