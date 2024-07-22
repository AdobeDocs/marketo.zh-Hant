---
unique-page-id: 2359663
description: 設定隱藏表單欄位值 — Marketo檔案 — 產品檔案
title: 設定隱藏表單欄位值
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# 設定隱藏表單欄位值 {#set-a-hidden-form-field-value}

隱藏欄位通常會動態填入。 未向填寫表單的人顯示。 以下說明設定值的方式。

>[!PREREQUISITES]
>
>[將表單欄位設定為隱藏](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## 選取欄位 {#select-the-field}

1. 在您的表單中，選取隱藏欄位，然後針對&#x200B;**自動填寫**&#x200B;按一下&#x200B;**編輯**。

   ![](assets/autofill.png)

## 使用預設值 {#use-default-value}

透過選擇「使用預設值」 ，您可以硬式編碼特定值，以便在提交此表單時始終使用。 輸入「預設值」，然後按一下「儲存」。

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL引數 {#url-parameter}

如果您要在填寫表單時從人員所在的頁面擷取URL引數（查詢字串），您可以使用&#x200B;**URL引數**&#x200B;來填入您的隱藏欄位。

>[!NOTE]
>
>引數有點技術化，不是嗎？ 不過一旦您取得，就表示它們是強大的。 查詢字串](https://en.wikipedia.org/wiki/Query_string)上的這個[Wikipedia頁面有些幫助。

1. 選取&#x200B;**取得值型別**&#x200B;的&#x200B;**URL引數**。

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. 輸入&#x200B;**引數名稱**&#x200B;並按一下&#x200B;**儲存**。

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>您可以輸入預設值，以備找不到URL引數時使用。

## Cookie值 {#cookie-value}

如果您要將資料儲存在Cookie中，可以使用&#x200B;**Cookie值**&#x200B;在提交表單時擷取資料。

1. 選取&#x200B;**從**&#x200B;取得值的&#x200B;**Cookie值**。

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. 輸入您想要的Cookie引數名稱，然後按一下&#x200B;**儲存**。

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >您可以輸入預設值，以備找不到引數/Cookie時使用。

## 反向連結引數 {#referrer-parameter}

如果您想要在填寫表單前從訪客來自的頁面擷取資料，可以使用&#x200B;**反向連結引數**。

1. 設定&#x200B;**從**&#x200B;取得值到&#x200B;**反向連結引數**。

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. 輸入您要從反向連結URL擷取的&#x200B;**引數名稱**，然後按一下&#x200B;**儲存**。

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >您可以輸入&#x200B;**預設值**，以備找不到反向連結引數時使用。

1. 按一下&#x200B;**完成**。

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. 按一下&#x200B;**核准並關閉**。

   ![](assets/image2014-9-15-13-3a10-3a43.png)
