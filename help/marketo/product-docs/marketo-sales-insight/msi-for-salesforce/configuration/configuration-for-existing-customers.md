---
unique-page-id: 42762519
description: 現有客戶的設定 — Marketo檔案 — 產品檔案
title: 現有客戶的設定
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 2%

---

# 現有客戶的設定 {#configuration-for-existing-customers}

請設定下列設定，以開始使用新的前瞻分析控制面板。

>[!PREREQUISITES]
>
>請確定您已將[!DNL Salesforce]套件升級至最新版本

## 在Marketo中設定[!DNL Sales Insight] {#configure-sales-insight-in-marketo}

1. 在瀏覽器中開啟新索引標籤，以從您的Marketo帳戶取得[!DNL Marketo Sales Insights]認證。

1. 移至&#x200B;**[!UICONTROL Admin]**&#x200B;區域。

   ![](assets/configuration-for-existing-customers-1.png)

1. 按一下「**[!UICONTROL Sales Insight]**」。

   ![](assets/configuration-for-existing-customers-2.png)

1. 按一下&#x200B;**[!UICONTROL View]**&#x200B;以填入Rest API認證。

   ![](assets/configuration-for-existing-customers-3.png)

1. 您會看到確認快顯視窗。 按一下「**[!UICONTROL OK]**」。

## 在[!DNL Sales Insight]中設定[!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，按一下&#x200B;**[!UICONTROL Setup]**。

   ![](assets/configuration-for-existing-customers-4.png)

1. 搜尋並選取&#x200B;**[!UICONTROL Remote Site Settings]**。

   ![](assets/configuration-for-existing-customers-5.png)

1. 按一下「**[!UICONTROL New Remote Site]**」。

   ![](assets/configuration-for-existing-customers-6.png)

1. 輸入[!UICONTROL Remote Site Name] （可能類似於「MarketoRestAPI」）和[!UICONTROL Remote Site URL] (您在Marketo中來自Rest API設定面板的API URL)。

   ![](assets/configuration-for-existing-customers-7.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/configuration-for-existing-customers-8.png)

   您現在已建立Rest API的遠端站台設定。

## 存取Marketo Sales Insight {#access-marketo-sales-insight}

1. 從[!DNL Marketo’s Sales Insight]管理頁面的Rest API面板複製認證。 將它們貼到Salesforce的[!DNL Sales Insight]設定頁面的Rest API區段中。

1. 輸入[!UICONTROL API Secret Key]。

   ![](assets/configuration-for-existing-customers-9.png)
