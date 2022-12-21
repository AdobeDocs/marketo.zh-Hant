---
unique-page-id: 7504923
description: 在收入模型中使用經理帳戶設定Google AdWords轉換 — Marketo檔案 — 產品檔案
title: 在收入模型中使用經理帳戶設定Google AdWords轉換
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# 在收入模型中使用經理帳戶設定Google AdWords轉換 {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

將您的Google AdWords帳戶連結至Marketo，以自動將離線轉換資料從Marketo上傳至Google AdWords。 然後，從AdWords UI中，您將可輕鬆查看哪些點按在您之後產生了合格銷售機會、機會和新客戶（或您要追蹤的任何收入階段） [新增自訂欄](https://support.google.com/adwords/answer/3073556) 在AdWords中。

如果您有多個Google Adwords帳戶，則可使用 [Google AdWords管理員帳戶](https://www.google.com/adwords/manager-accounts/) （舊稱「My Client Center」），將其與Marketo整合。

您可以將AdWords離線轉換對應至收入模型中的一或多個階段。 有兩種方式：

* 階段動作
* AdWords對應

>[!PREREQUISITES]
>
>[以Manager帳戶將Google AdWords新增為Launchpoint服務](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## 使用階段操作 {#use-stage-action}

在「階段動作」下對應AdWords轉換。

1. 選取您要對應至AdWords轉換的步驟。

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. 在 **階段動作** 下拉式清單，選取 **設定AdWords轉換**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 設定 **AdWords轉換**.

   >[!NOTE]
   >
   >可為每個子帳戶選取不同的AdWords轉換。

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   提示：如果您沒有任何AdWords轉換，請按一下 **+新轉換**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. 按一下 **儲存**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. 將所有AdWords轉換對應至收入階段後，返回摘要頁面。 選擇 **模型動作** 選擇 **核准階段**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## 專業提示：新增轉換 {#pro-tip-add-a-new-conversion}

小費！ 可從Marketo建立新的AdWords離線轉換。

>[!CAUTION]
>
>從Marketo建立的新轉換已啟用「最佳化」設定。 這表示可允許AdWords競標策略來最佳化您對這些轉換的出價。 您可以從AdWords帳戶變更此設定。

1. 在 **階段動作** 下拉式清單，選取 **設定AdWords轉換**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. 選擇 **新轉換**.

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. 輸入 **轉換名稱**. 按一下 **儲存**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   太棒了！ 這個新轉換會顯示在您的AdWords帳戶中。

## 使用AdWords對應 {#use-adwords-mapping}

您可以使用「AdWords對應」，將所有模型階段與AdWords轉換在單一位置建立關聯。

1. 選擇 **編輯AdWords對應**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. 選取所需 **AdWords帳戶** 和期望 **AdWords轉換** 針對您要追蹤的每個階段。

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. 對應階段後，按一下 **儲存**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. 將所有AdWords轉換對應至收入階段後，返回摘要頁面。 選擇 **模型動作** 選擇 **核准階段**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

若要檢視離線轉換資料，您需要登入您的AdWords帳戶。 建議您使用 [自訂欄功能](https://support.google.com/adwords/answer/3073556) 若要為您從Marketo匯入的每個離線轉換建立轉換計數欄。
