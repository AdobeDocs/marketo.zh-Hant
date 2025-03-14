---
unique-page-id: 6095029
description: 在收入模型中設定Google AdWords轉換 — Marketo檔案 — 產品檔案
title: 在收入模型中設定Google AdWords轉換
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# 在收入模型中設定Google AdWords轉換 {#set-google-adwords-conversions-in-the-revenue-model}

將您的Google AdWords帳戶連結至Marketo，以便自動將離線轉換資料從Marketo上傳至Google AdWords。 接著，在AdWords中[新增自訂欄](https://support.google.com/adwords/answer/3073556)後，您可以從AdWords UI輕鬆檢視哪些點按導致合格的銷售機會、商機及新客戶（或您要追蹤的任何收入階段）。

>[!NOTE]
>
>這是從Marketo到Google AdWords的推送整合。 轉換資料將&#x200B;_僅_&#x200B;顯示在您的Google AdWords入口網站中，_不會顯示在Marketo UI_&#x200B;中。

深入瞭解[Google的離線轉換匯入功能](https://support.google.com/adwords/answer/2998031?hl=en)。 將AdWords離線轉換對應至收入模型中的一或多個階段。 有三種方式可以進行對應：

* AdWords轉換
* 中繼動作
* AdWords對映

如果您使用「舞台動作」，可以從Marketo建立新的AdWords離線轉換。

>[!PREREQUISITES]
>
>[將Google AdWords新增為LaunchPoint Service](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## 使用AdWords轉換 {#use-adwords-conversion}

1. 移至&#x200B;**Analytics**&#x200B;區域。

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. 選取模型。

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. 按一下&#x200B;**編輯草稿**。

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. 選取您要對應至AdWords轉換的收入階段。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 選取您要對應至Marketo階段的&#x200B;**AdWords轉換**。

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   很好！ 您的AdWords轉換資料會以您選取的順序上傳至您的Google AdWords。

## 使用階段動作 {#use-stage-action}

您也可以在「舞台動作」底下對應AdWords轉換。

1. 選取您要對應至AdWords轉換的步驟。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 在&#x200B;**階段動作**&#x200B;下拉式清單中，選取&#x200B;**設定AdWords轉換**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 選取&#x200B;**AdWords轉換**。

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **秘訣**：如果您沒有任何AdWords轉換，請按一下&#x200B;**+新增轉換**&#x200B;來建立轉換。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 按一下&#x200B;**保存**。

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. 完成將所有AdWords轉換對應至收入階段後，請返回摘要頁面。 選取&#x200B;**模型動作**&#x200B;並選擇&#x200B;**核准階段**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## 專業秘訣：新增轉換 {#pro-tip-add-a-new-conversion}

專業秘訣！ 可從Marketo建立新的AdWords離線轉換。

>[!CAUTION]
>
>從Marketo建立的新轉換已啟用「最佳化」設定。 這表示AdWords競標策略可讓您針對這些轉換最佳化競標。 您可以從您的AdWords帳戶變更此設定。

1. 在&#x200B;**階段動作**&#x200B;下拉式清單中，選取&#x200B;**設定AdWords轉換**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 選取&#x200B;**新轉換**。

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. 輸入&#x200B;**轉換名稱**。 按一下&#x200B;**保存**。

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   太好了！ 這個新的轉換將會顯示在您的AdWords帳戶中。

## 使用AdWords對應 {#use-adwords-mapping}

您可以使用「AdWords對應」，將所有模型階段與AdWords轉換建立關聯。

1. 選取&#x200B;**編輯AdWords對應**。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 針對您要追蹤的每個階段選取所需的&#x200B;**AdWords轉換**。

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. 完成階段對應後，請按一下&#x200B;**儲存**。

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. 完成將所有AdWords轉換對應至收入階段後，請返回摘要頁面。 選取&#x200B;**模型動作**&#x200B;並選擇&#x200B;**核准階段**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

若要檢視離線轉換資料，您必須登入AdWords帳戶。 建議您使用其[自訂欄功能](https://support.google.com/adwords/answer/3073556)，為您從Marketo匯入的每個離線轉換建立轉換計數欄。
