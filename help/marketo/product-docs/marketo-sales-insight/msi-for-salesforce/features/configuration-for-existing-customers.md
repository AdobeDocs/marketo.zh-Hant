---
unique-page-id: 42762519
description: 現有客戶的設定——行銷檔案——產品檔案
title: 現有客戶的配置
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# 現有客戶的配置 {#configuration-for-existing-customers}

請設定下列設定，以開始使用新的前瞻分析控制面板。

>[!NOTE]
>
>**必要條件**
>
>請確定您已將Salesforce套件升級至最新版本

## 在Marketo中設定Sales Insight {#configure-sales-insight-in-marketo}

1. 在您的瀏覽器中開啟新標籤，從您的Marketo帳戶取得Marketo Sales Insights認證。
1. 前往「管 **理** 」區。

   ![](assets/configure-1.png)

1. 按一 **下Sales Insight**。

   ![](assets/configure-2.png)

1. 按一 **下「檢視** 」以填入Rest API憑證。

   ![](assets/configure-3.png)

1. 您會看到確認快顯視窗。 按一下 **確定**。

## 在Salesforce中設定Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，按一下「 **設定**」。

   ![](assets/sfdc-1.png)

1. 搜索並選擇「 **遠程站點設定」**。

   ![](assets/sfdc-2.png)

1. 按一下 **新建遠程站點**。

   ![](assets/sfdc-3.png)

1. 輸入「遠端網站名稱」（可能類似「MarketoRestAPI」），以及「遠端網站URL」（您在Marketo的「Rest API設定」面板中的API URL）。

   ![](assets/sfdc-4.png)

1. 按一下 **儲存**。

   ![](assets/sfdc-5.png)

   您現在已建立Rest API的遠端網站設定。

## Access Marketto Sales Insight {#access-marketo-sales-insight}

1. 從Marketo的「銷售分析管理」頁面的「其餘API」面板複製認證。 將它們貼至Salesforce的「Sales Insight設定」頁面的「其餘API」區段。
1. 輸入API密碼。

   ![](assets/config.png)

