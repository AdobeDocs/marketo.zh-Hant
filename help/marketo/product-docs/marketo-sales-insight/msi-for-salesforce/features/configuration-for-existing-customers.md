---
unique-page-id: 42762519
description: 現有客戶的設定——行銷檔案——產品檔案
title: 現有客戶的配置
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---


# 現有客戶的配置{#configuration-for-existing-customers}

請設定下列設定，以開始使用新的前瞻分析控制面板。

>[!PREREQUISITES]
>
>請確定您已將Salesforce套件升級至最新版本

## 在Marketon中設定Sales Insight {#configure-sales-insight-in-marketo}

1. 在您的瀏覽器中開啟新標籤，從您的Marketo帳戶取得Marketo Sales Insights認證。

1. 前往&#x200B;**Admin**&#x200B;區域。

   ![](assets/configure-1.png)

1. 按一下&#x200B;**Sales Insight**。

   ![](assets/configure-2.png)

1. 按一下&#x200B;**View**&#x200B;以填充Rest API憑據。

   ![](assets/configure-3.png)

1. 您會看到確認快顯視窗。 按一下&#x200B;**確定**。

## 在Salesforce {#configure-sales-insight-in-salesforce}中設定Sales Insight

1. 在Salesforce中，按一下「**Setup**」。

   ![](assets/sfdc-1.png)

1. 搜索並選擇&#x200B;**遠程站點設定**。

   ![](assets/sfdc-2.png)

1. 按一下&#x200B;**新建遠程站點**。

   ![](assets/sfdc-3.png)

1. 輸入「遠端網站名稱」（可能類似「MarketoRestAPI」），以及「遠端網站URL」（您在Marketo的「Rest API設定」面板中的API URL）。

   ![](assets/sfdc-4.png)

1. 按一下&#x200B;**保存**。

   ![](assets/sfdc-5.png)

   您現在已建立Rest API的遠端網站設定。

## 存取Marketor Sales Insight {#access-marketo-sales-insight}

1. 從Marketo的「銷售分析管理」頁面的「其餘API」面板複製認證。 將它們貼至Salesforce的「Sales Insight設定」頁面的「其餘API」區段。

1. 輸入API密碼。

   ![](assets/config.png)
