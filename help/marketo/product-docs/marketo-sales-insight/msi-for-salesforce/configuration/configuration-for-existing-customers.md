---
unique-page-id: 42762519
description: 現有客戶的設定 — Marketo檔案 — 產品檔案
title: 現有客戶的設定
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 現有客戶的設定 {#configuration-for-existing-customers}

請設定下列設定，以開始使用新的前瞻分析控制面板。

>[!PREREQUISITES]
>
>請確定您已將Salesforce套件升級至最新版本

## 在Marketo中設定Sales Insight {#configure-sales-insight-in-marketo}

1. 在瀏覽器中開啟新標籤，以便從您的Marketo帳戶取得Marketo銷售分析憑證。

1. 前往 **管理員** 區域。

   ![](assets/configuration-for-existing-customers-1.png)

1. 按一下 **銷售分析**.

   ![](assets/configuration-for-existing-customers-2.png)

1. 按一下 **檢視** 以填入Rest API認證。

   ![](assets/configuration-for-existing-customers-3.png)

1. 您會看到確認快顯視窗。 按一下 **確定**.

## 在Salesforce中設定Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，按一下 **設定**.

   ![](assets/configuration-for-existing-customers-4.png)

1. 搜尋並選取 **遠端站台設定**.

   ![](assets/configuration-for-existing-customers-5.png)

1. 按一下 **新增遠端站台**.

   ![](assets/configuration-for-existing-customers-6.png)

1. 輸入遠端網站名稱（可能類似於「MarketoRestAPI」）和遠端網站URL (您在Marketo中來自Rest API設定面板的API URL)。

   ![](assets/configuration-for-existing-customers-7.png)

1. 按一下 **儲存**.

   ![](assets/configuration-for-existing-customers-8.png)

   您現在已建立Rest API的遠端站台設定。

## 存取Marketo Sales Insight {#access-marketo-sales-insight}

1. 從Marketo的Sales Insight「管理頁面」中的Rest API面板複製認證。 將它們貼到Salesforce的Sales Insight設定頁面的Rest API區段。

1. 輸入API金鑰。

   ![](assets/configuration-for-existing-customers-9.png)
