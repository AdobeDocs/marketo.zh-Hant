---
unique-page-id: 42762519
description: 現有客戶的設定 — Marketo檔案 — 產品檔案
title: 現有客戶的設定
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
source-git-commit: 0701121597f33580ada09fe975c1740cb55f945d
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

1. 在瀏覽器中開啟新標籤，從您的Marketo帳戶取得Marketo Sales Insights認證。

1. 前往&#x200B;**Admin**&#x200B;區域。

   ![](assets/configuration-for-existing-customers-1.png)

1. 按一下&#x200B;**Sales Insight**。

   ![](assets/configuration-for-existing-customers-2.png)

1. 按一下&#x200B;**View**&#x200B;以填入Rest API憑證。

   ![](assets/configuration-for-existing-customers-3.png)

1. 您會看到確認快顯視窗。 按一下&#x200B;**確定**。

## 在Salesforce中設定Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，按一下&#x200B;**Setup**。

   ![](assets/configuration-for-existing-customers-4.png)

1. 搜索並選擇&#x200B;**遠程站點設定**。

   ![](assets/configuration-for-existing-customers-5.png)

1. 按一下「**新建遠程站點**」。

   ![](assets/configuration-for-existing-customers-6.png)

1. 輸入遠端網站名稱（可以是「MarketoRestAPI」之類的名稱）和遠端網站URL(您來自Marketo中「Rest API設定」面板的API URL)。

   ![](assets/configuration-for-existing-customers-7.png)

1. 按一下「**儲存**」。

   ![](assets/configuration-for-existing-customers-8.png)

   您現在已為Rest API建立遠端網站設定。

## 存取Marketo Sales Insight {#access-marketo-sales-insight}

1. 從Marketo的Sales Insight管理頁面的Rest API面板複製憑證。 將它們貼到Salesforce的「Sales Insight設定」頁面的「Rest API」區段中。

1. 輸入API密鑰。

   ![](assets/configuration-for-existing-customers-9.png)
