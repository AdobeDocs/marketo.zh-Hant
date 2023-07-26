---
description: 將來電原因和來電結果記錄到Salesforce - Marketo檔案 — 產品檔案
title: 將通話原因和通話結果記錄到Salesforce
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 將通話原因和通話結果記錄到Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

如果您想要將來電結果記錄並向Salesforce呼叫原因以用於報表或可見度，您可以為每個建立自訂活動欄位。 每個欄位都必須使用特定的API名稱（在Salesforce中稱為「欄位名稱」）。

* 通話結果欄位名稱：mktosales_call_output
* 來電原因欄位名稱： mktosales_call_reason

若要利用這些欄位，您首先需要將欄位建立為自訂活動欄位。 為了讓使用者看得見，您需要將它新增至任務物件頁面版面配置。

## Salesforce Classic {#salesforce-classic}

### 在Salesforce Classic中建立自訂活動欄位  {#create-custom-activity-field-in-salesforce-classic}

1. 在Salesforce中，按一下 **設定**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. 在「快速尋找」方塊中輸入「活動」。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. 按一下 **活動自訂欄位**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. 按一下 **新增**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. 選取資料型別「文字」並按一下 **下一個**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. 為自訂欄位指定如上定義的欄位名稱。 欄位長度有255個字元的限制。 欄位標籤將是您的銷售團隊可見的欄位，並且可以根據您的團隊需求進行自訂。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. 其餘設定是選用的。 完成設定後，請按一下 **下一個**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. 為此欄位選取所需的欄位層級安全性設定，然後按一下 **下一個** （下圖只是範例）。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >請確定您的Sales Connect使用者所使用的設定檔可看見自訂欄位，以及您想要的其他顯示專案。

1. 選取您要新增欄位的頁面配置，然後按一下 **儲存** (您也可以按一下 **儲存並新增** 並針對「來電原因」欄位重複此程式)。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### 在Salesforce Classic中新增自訂活動欄位至任務頁面配置 {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>如果您未在上述步驟9中選取想要的頁面配置，您僅需遵循這些步驟。

1. 在Salesforce中，按一下 **設定**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. 在「快速尋找」方塊中輸入「任務」。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. 按一下 **任務頁面配置**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. 按一下 **編輯** 在您要新增此欄位的「任務頁面配置」旁邊。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. 將欄位拖放至「任務」頁面配置的所需區段。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. 按一下 **儲存**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## Salesforce閃電 {#salesforce-lightning}

### 在Salesforce閃電中建立自訂活動欄位 {#create-custom-activity-field-in-salesforce-lightning}

1. 在Salesforce中，按一下右上方的齒輪圖示並選取 **設定**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. 按一下 **物件管理員**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. 在「快速尋找」方塊中輸入「Activity」。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. 按一下 **活動** 標籤。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. 按一下 **欄位和關係**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. 按一下 **新增**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### 在Salesforce Lightning中將自訂活動欄位新增到任務頁面配置 {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. 在Salesforce中，按一下右上方的齒輪圖示並選取 **設定**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. 按一下 **物件管理員**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. 在「快速尋找」方塊中輸入「任務」。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. 按一下 **任務** 標籤。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. 按一下 **頁面配置**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. 按一下您要新增此欄位的任務頁面配置。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. 將欄位拖放至「任務」頁面配置的所需區段。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. 按一下 **儲存**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>[在活動歷史記錄上安裝Sales Connect事件欄位](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
