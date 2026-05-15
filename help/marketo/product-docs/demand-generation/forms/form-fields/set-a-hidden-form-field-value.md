---
unique-page-id: 2359663
description: 瞭解如何在Marketo中設定隱藏的表單欄位值。 在提交表單時傳遞靜態或權杖值。
title: 設定隱藏表單欄位值
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
TQID: https://experienceleague.adobe.com/uw1Xfgoa51WI-Ca6knnBGlwfrruPTYldJ--3zF5Jlzc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 266
ht-degree: 6%

---

# 設定隱藏表單欄位值 {#set-a-hidden-form-field-value}

隱藏欄位通常會動態填入。 未向填寫表單的人顯示。 以下說明設定值的方式。

>[!PREREQUISITES]
>
>[將表單欄位設定為隱藏](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## 選取欄位 {#select-the-field}

1. 在您的表單中，選取隱藏欄位並按一下&#x200B;**[!UICONTROL Autofill]**&#x200B;的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/autofill.png)

## 使用預設值 {#use-default-value}

透過選取「使用&#x200B;**[!UICONTROL Default Value]**」，您可以硬式編碼特定值，以便在提交此表單時一律使用。 輸入&#x200B;**[!UICONTROL Default Value]**&#x200B;並按一下&#x200B;**[!UICONTROL Save]**。

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL 參數 {#url-parameter}

如果您想要在填寫表單時從人員所在的頁面擷取URL引數（查詢字串），您可以使用&#x200B;**[!UICONTROL URL Parameters]**&#x200B;填入您的隱藏欄位。

>[!NOTE]
>
>引數是技術性的。 一旦您瞭解這些功能，就表示它們是強大的。 查詢字串](https://en.wikipedia.org/wiki/Query_string)上的這個[Wikipedia頁面有些幫助。

1. 為&#x200B;**[!UICONTROL Get Value Type]**&#x200B;選取&#x200B;**[!UICONTROL URL Parameter]**。

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. 輸入&#x200B;**[!UICONTROL Parameter Name]**&#x200B;並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>如果找不到URL引數，您可以輸入&#x200B;**[!UICONTROL Default Value]**。

## Cookie值 {#cookie-value}

如果您要將資料儲存在Cookie中，您可以在提交表單時使用&#x200B;**[!UICONTROL Cookie Value]**&#x200B;擷取資料。

1. 為&#x200B;**[!UICONTROL Get Value From]**&#x200B;選取&#x200B;**[!UICONTROL Cookie Value]**。

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. 輸入您想要的Cookie **[!UICONTROL Parameter Name]**&#x200B;並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >您可以輸入&#x200B;**[!UICONTROL Default Value]**，以備找不到引數/Cookie時使用。

## 反向連結引數 {#referrer-parameter}

如果您想要在填寫表單前從訪客來自的頁面擷取資料，可以使用&#x200B;**[!UICONTROL Referrer Parameter]**。

1. 將&#x200B;**[!UICONTROL Get Value From]**&#x200B;設為&#x200B;**[!UICONTROL Referrer Parameter]**。

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. 輸入您要從反向連結URL擷取的&#x200B;**[!UICONTROL Parameter Name]**，然後按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >您可以輸入&#x200B;**[!UICONTROL Default Value]**，以備找不到反向連結引數時使用。

1. 按一下「**[!UICONTROL Finish]**」。

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. 按一下「**[!UICONTROL Approve and Close]**」。

   ![](assets/image2014-9-15-13-3a10-3a43.png)
