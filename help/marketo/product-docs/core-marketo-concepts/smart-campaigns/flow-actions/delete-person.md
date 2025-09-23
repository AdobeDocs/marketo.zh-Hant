---
unique-page-id: 1147082
description: 刪除人員 — Marketo檔案 — 產品檔案
title: 刪除人員
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# 刪除人員 {#delete-person}

錯誤的人有時會進入您的資料庫。 「刪除人員」流程步驟可以移除這些人員。

![](assets/delete-person-1.png)

>[!CAUTION]
>
>當您刪除人員時，也會一併刪除其所有歷史RCE資料。 此動作無法還原。

1. 當您在流程步驟中拖曳時，系統會自動將其設定為也從CRM中刪除。

   ![](assets/delete-person-2.png)

1. 您可以從Marketo Engage中刪除，但無法從CRM中刪除，如下所示：

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>從您的CRM _移除人員只適用於[!DNL Salesforce]_。 如果您從Marketo中刪除人員並選擇將他們保留在[!DNL Salesforce]中，則當他們的[!DNL Salesforce]記錄更新時，將在Marketo中重新建立他們。
