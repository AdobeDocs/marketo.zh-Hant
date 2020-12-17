---
unique-page-id: 2359663
description: 設定隱藏的表單欄位值——行銷檔案——產品檔案
title: 設定隱藏表單欄位值
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---


# 設定隱藏表單欄位值{#set-a-hidden-form-field-value}

隱藏欄位通常會動態填入。 不會向填寫表格的人顯示。 以下是如何設定值。

>[!PREREQUISITES]
>
>[將表單欄位設為隱藏](set-a-form-field-as-hidden.md)

## 選擇欄位{#select-the-field}

1. 在表單中，選擇隱藏欄位，然後按一下&#x200B;**Edit** for **Autofill**。

   ![](assets/autofill.png)

## 使用預設值{#use-default-value}

選取「使用預設值」，您可以硬式編碼特定值，以便在提交此表單時一律使用。 輸入預設值，然後按一下保存。

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL參數{#url-parameter}

如果您想在填寫表單時從人員所在的頁面擷取URL參數（查詢字串），可使用&#x200B;**URL** **參數**&#x200B;填入隱藏欄位。

>[!NOTE]
>
>參數有點技術化，不是嗎？ 但一旦你得到了它們，它們就變得強大了。 查詢字串上的此[Wikipedia頁面](http://en.wikipedia.org/wiki/Query_string)有些幫助。

1. 為&#x200B;**獲取值類型**&#x200B;選擇&#x200B;**URL參數**。

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. 輸入&#x200B;**參數名稱**，然後按一下&#x200B;**保存**。

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>您可以輸入預設值，以備找不到URL參數時使用。

## Cookie值{#cookie-value}

如果您將資料儲存在Cookie中，則可在提交表單時使用&#x200B;**Cookie****Value**&#x200B;來擷取資料。

1. 選擇&#x200B;**Cookie********Get********From**&#x200B;的值。

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. 輸入您想要的Cookie參數名稱，然後按一下「儲存&#x200B;**」。**

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >您可以輸入預設值，以備找不到參數/Cookie時使用。

## 反向連結參數{#referrer-parameter}

如果您想在填寫表單前從訪客來自的頁面擷取資料，可以使用&#x200B;**Referrer** **Parameter**。

1. 將&#x200B;**Get****Value****From**&#x200B;設定為&#x200B;**Referrer****Parameter**。

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. 輸入您要從反向連結URL擷取的&#x200B;**參數名稱**，然後按一下「儲存&#x200B;**」。**

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >如果找不到反向連結參數，您可以輸入&#x200B;**Default** **Value**。

1. 按一下&#x200B;**完成**。

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. 按一下「核准並關閉」。****

   ![](assets/image2014-9-15-13-3a10-3a43.png)

真貼心！ 你幹得不錯。 有關[forms](http://docs.marketo.com/display/docs/forms)的更多資訊。
