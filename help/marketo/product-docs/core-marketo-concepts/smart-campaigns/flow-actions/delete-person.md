---
unique-page-id: 1147082
description: 瞭解如何使用流程步驟從資料庫刪除人員。 從Marketo中移除符合條件的人員。
title: 刪除人員
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/89EPt9SVBCuluSojdqLE4BawaPGGbzHLSmYHV9w6Uko
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 127
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
