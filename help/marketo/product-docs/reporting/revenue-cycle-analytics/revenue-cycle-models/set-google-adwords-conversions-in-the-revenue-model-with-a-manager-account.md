---
unique-page-id: 7504923
description: 使用管理員帳戶在收入模型中設定Google AdWords轉換 — Marketo檔案 — 產品檔案
title: 透過管理員帳戶在收入模型中設定Google AdWords轉換
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# 透過管理員帳戶在收入模型中設定Google AdWords轉換 {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

將您的Google AdWords帳戶連結至Marketo，以便自動將離線轉換資料從Marketo上傳至Google AdWords。 接著，在AdWords中[新增自訂欄](https://support.google.com/adwords/answer/3073556)後，您可以從AdWords UI輕鬆檢視哪些點按導致合格的銷售機會、商機及新客戶（或您要追蹤的任何收入階段）。

如果您有多個Google Adwords帳戶，可以使用[Google AdWords管理員帳戶](https://www.google.com/adwords/manager-accounts/) （先前稱為「我的使用者端中心」）將它們與Marketo整合。

您可以將AdWords離線轉換對應至收入模型中的一或多個階段。 有兩種方式：

* 中繼動作
* AdWords對映

>[!PREREQUISITES]
>
>[將Google AdWords新增為具有管理員帳戶的Launchpoint服務](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## 使用階段動作 {#use-stage-action}

在「舞台動作」底下對應AdWords轉換。

1. 選取您要對應至AdWords轉換的步驟。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 在&#x200B;**階段動作**&#x200B;下拉式清單中，選取&#x200B;**設定AdWords轉換**。

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 設定&#x200B;**AdWords轉換**。

   >[!NOTE]
   >
   >可以為每個子帳戶選取不同的AdWords轉換。

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   秘訣：如果您沒有任何AdWords轉換，請按一下&#x200B;**+新增轉換**&#x200B;來建立轉換。

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. 按一下&#x200B;**保存**。

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. 輸入&#x200B;**轉換名稱**。 按一下&#x200B;**保存**。

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   太好了！ 這個新的轉換將會顯示在您的AdWords帳戶中。

## 使用AdWords對應 {#use-adwords-mapping}

您可以使用「AdWords對應」，將所有模型階段與AdWords轉換建立關聯。

1. 選取&#x200B;**編輯AdWords對應**。

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 針對您要追蹤的每個階段，選取所需的&#x200B;**AdWords帳戶**&#x200B;和所需的&#x200B;**AdWords轉換**。

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. 完成階段對應後，請按一下&#x200B;**儲存**。

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. 完成將所有AdWords轉換對應至收入階段後，請返回摘要頁面。 選取&#x200B;**模型動作**&#x200B;並選擇&#x200B;**核准階段**。

   ![](assets/image2015-2-27-12-3a20-3a20.png)

若要檢視離線轉換資料，您必須登入AdWords帳戶。 建議您使用其[自訂欄功能](https://support.google.com/adwords/answer/3073556)，為您從Marketo匯入的每個離線轉換建立轉換計數欄。
