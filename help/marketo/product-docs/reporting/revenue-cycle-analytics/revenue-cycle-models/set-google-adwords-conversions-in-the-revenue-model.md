---
unique-page-id: 6095029
description: 在收入模型中設定 [!DNL Google AdWords] 轉換 — Marketo檔案 — 產品檔案
title: 在收入模型中設定 [!DNL Google AdWords] 轉換
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 2%

---

# 在收入模型中設定[!DNL Google AdWords]轉換 {#set-google-adwords-conversions-in-the-revenue-model}

將您的[!DNL Google AdWords]帳戶連結至Marketo，以自動將離線轉換資料從Marketo上傳至[!DNL Google AdWords]。 接著，在[!DNL AdWords]中[新增自訂欄](https://support.google.com/adwords/answer/3073556)後，您就可以從[!DNL AdWords] UI中輕鬆檢視哪些點按導致合格的銷售機會、商機及新客戶（或您要追蹤的任何收入階段）。

>[!NOTE]
>
>這是從Marketo到[!DNL Google AdWords]的推播整合。 轉換資料將&#x200B;_僅_&#x200B;顯示在您的[!DNL Google AdWords]入口網站中，_不會顯示在Marketo UI_&#x200B;中。

深入瞭解[Google的離線轉換匯入功能](https://support.google.com/adwords/answer/2998031?hl=en)。 將[!DNL AdWords]個離線轉換對應至收入模型中的一或多個階段。 有三種方式可以進行對應：

* [!DNL AdWords]轉換
* 中繼動作
* [!DNL AdWords]對應

如果您使用中繼動作，可以從Marketo建立新的[!DNL AdWords]離線轉換。

>[!PREREQUISITES]
>
>[新增 [!DNL Google AdWords] 為LaunchPoint服務](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## 使用[!DNL AdWords]轉換 {#use-adwords-conversion}

1. 前往「**[!UICONTROL Analytics]**」區域。

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. 選取模型。

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. 按一下「**[!UICONTROL Edit Draft]**」。

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. 選取您要對應至[!DNL AdWords]轉換的收入階段。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 選取您要對應至Marketo階段的&#x200B;**[!UICONTROL AdWords Conversion]**。

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   很好！ 您的[!DNL AdWords]轉換資料將會以您選取的順序上傳至您的[!DNL Google AdWords]。

## 使用階段動作 {#use-stage-action}

您也可以在[!UICONTROL AdWords Conversion]下對應&#x200B;**[!UICONTROL Stage Actions]**。

1. 選取您要對應至[!DNL AdWords]轉換的步驟。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 在&#x200B;**[!UICONTROL Stage Actions]**&#x200B;下拉式清單中，選取&#x200B;**[!UICONTROL Set AdWords Conversion]**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 選取&#x200B;**[!UICONTROL AdWords Conversion]**。

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **秘訣**：如果您沒有任何[!DNL AdWords]轉換，請按一下&#x200B;**[!UICONTROL +New Conversion]**&#x200B;建立一個轉換。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. 完成將所有[!DNL AdWords]轉換對應到收入階段後，請返回摘要頁面。 選取&#x200B;**[!UICONTROL Model Actions]**&#x200B;並選擇&#x200B;**[!UICONTROL Approve Stages]**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## 專業秘訣：新增轉換 {#pro-tip-add-a-new-conversion}

專業秘訣！ 可從Marketo建立新的[!DNL AdWords]離線轉換。

>[!CAUTION]
>
>從Marketo建立的新轉換已啟用「最佳化」設定。 這表示允許[!DNL AdWords]競標策略針對這些轉換最佳化您的競標。 您可以從您的[!DNL AdWords]帳戶變更此設定。

1. 在&#x200B;**[!UICONTROL Stage Actions]**&#x200B;下拉式清單中，選取&#x200B;**[!UICONTROL Set AdWords Conversion]**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 選取「**[!UICONTROL New Conversion]**」。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 輸入&#x200B;**[!UICONTROL Conversion Name]**。 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   太好了！ 此新轉換將顯示在您的[!DNL AdWords]帳戶中。

## 使用[!DNL AdWords]對應 {#use-adwords-mapping}

您可以使用[!UICONTROL AdWords Conversion]對應將所有模型階段與[!DNL AdWords]在一個位置建立關聯。

1. 選取「**[!UICONTROL Edit AdWords Mappings]**」。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 針對您要追蹤的每個階段選取所需的&#x200B;**[!UICONTROL AdWords Conversion]**。

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. 在對應階段之後，請按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. 完成將所有[!DNL AdWords]轉換對應到收入階段後，請返回摘要頁面。 選取&#x200B;**[!UICONTROL Model Actions]**&#x200B;並選擇&#x200B;**[!UICONTROL Approve Stages]**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

若要檢視離線轉換資料，您必須登入[!DNL AdWords]帳戶。 建議您使用其[自訂欄功能](https://support.google.com/adwords/answer/3073556)，為您從Marketo匯入的每個離線轉換建立轉換計數欄。
