---
unique-page-id: 6095029
description: 在「收入模型——行銷人員檔案——產品檔案」中設定Google AdWords轉換
title: 在收入模型中設定Google AdWords轉換
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---


# 在收入模型中設定Google AdWords轉換 {#set-google-adwords-conversions-in-the-revenue-model}

將您的Google AdWords帳戶連結至Marketo，以自動將離線轉換資料從Marketo上傳至Google AdWords。 然後，在AdWords中新增自訂欄後，您就可以從AdWords UI中輕鬆看到哪些點按產生了合格的潛在客戶、機會和新客戶(或您想要追蹤的任何收入階段 [](https://support.google.com/adwords/answer/3073556) )。

>[!NOTE]
>
>這是從Marketo到Google AdWords的推播整合。 轉換資料只會 *出現在* Google AdWords入口網站**中，而不會出現在Marketo UI中。**

進一步了 [解Google的離線轉換匯入功能](https://support.google.com/adwords/answer/2998031?hl=en)。  將AdWords離線轉換對應至收入模型中的一或多個階段。 有三種方法可執行對應：

* AdWords轉換
* 舞台動作
* AdWords對應

如果您使用「舞台動作」，可以從Market建立新的AdWords離線轉換。

>[!PREREQUISITES]
>
>* [將Google AdWords新增為LaunchPoint服務](../../../../product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

>



## 使用AdWords轉換 {#use-adwords-conversion}

1. 前往「分 **析** 」區。

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. 選取模型。

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. 按一下「 **編輯草稿**」。

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. 選取您要對應至AdWords轉換的收入階段。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 選取 **您要對應至** 「行銷人員」舞台的「AdWords轉換」。

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   不錯！ 您的AdWords轉換資料將會在您選取的節奏下上傳至您的Google AdWords。

## 使用階段動作 {#use-stage-action}

您也可以在「舞台動作」下對應AdWords轉換。

1. 選取您要對應至AdWords轉換的步驟。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 在「階 **段動作** 」下拉式清單中，選 **取「設定AdWords轉換」**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 選取「 **AdWords轉換」**。

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **提示**:如果您沒有任何AdWords轉換，請按一下「新增轉換」 **建立轉換**。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 按一下 **儲存**。

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. 將所有AdWords轉換對應至收入階段後，請返回摘要頁面。 選擇「 **模型操作** 」，然後選擇「 **批准階段」**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## 專業提示：新增轉換 {#pro-tip-add-a-new-conversion}

專業提示！ 您可從Marketo建立新的AdWords離線轉換。

>[!CAUTION]
>
>從Market建立的新轉換，啟用「最佳化」設定。 這表示AdWords競標策略可讓您最佳化這些轉換的競標。 您可以從AdWords帳戶變更此設定。

1. 在「階 **段動作** 」下拉式清單中，選 **取「設定AdWords轉換」**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 選擇 **新轉換**。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 輸入轉 **換名稱**。 按一下 **儲存**。

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   太棒了！ 此新轉換將會出現在您的AdWords帳戶中。

## 使用AdWords對應 {#use-adwords-mapping}

您可以使用「AdWords對應」，將所有模型階段與AdWords轉換在同一個位置建立關聯。

1. 選取「 **編輯AdWords對應」**。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 針對您要 **追蹤的每個階段** ，選取所要的AdWords轉換。

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. 對應階段後，按一下「儲 **存」**。

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. 將所有AdWords轉換對應至收入階段後，請返回摘要頁面。 選擇「 **模型操作** 」，然後選擇「 **批准階段」**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

若要檢視離線轉換資料，您必須登入您的AdWords帳戶。 建議您使用其「自訂 [欄」功能](https://support.google.com/adwords/answer/3073556) ，為您從Marketo匯入的每個離線轉換建立轉換計數欄。
