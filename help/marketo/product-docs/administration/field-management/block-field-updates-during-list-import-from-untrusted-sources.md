---
unique-page-id: 2360335
description: 從不受信任的來源匯入清單期間的區塊欄位更新-Marketo檔案——產品檔案
title: 從不受信任的來源匯入清單期間的區塊欄位更新
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 從不受信任的來源匯入清單期間的區塊欄位更新{#block-field-updates-during-list-import-from-untrusted-sources}

您可以比其他清單更信任某些清單中的資料。 有時候，您有可疑的資料，如果欄位空白，但現有值則不要。 您可以封鎖關鍵欄位的欄位更新，以完成此作業。

>[!NOTE]
>
>**需要管理員權限**

## 阻止來自不受信任源的欄位更新{#blocking-field-updates-from-untrusted-sources}

1. 前往&#x200B;**Admin**，然後按一下「欄位管理」。****

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. 查找所需欄位，選擇它，然後在&#x200B;**欄位操作**&#x200B;下，按一下&#x200B;**塊欄位更新**。

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. 勾選「**清單匯入不信任的來源**」，然後按一下「套用&#x200B;**」。**

   ![](assets/blockupdates.png)

>[!TIP]
>
>您也可以勾選「清單匯入信任來源」，以保護欄位不受所有清單（受信任和不受信任）的限制。****

對您想要避免不受信任清單影響的任何其他欄位，重複上述步驟。

## 運行不信任清單導入{#running-an-untrusted-list-import}

1. 運行清單導入時，如果希望在上一步中設定的所有欄位都安全，請務必選擇&#x200B;**不受信任的**。

   ![](assets/importpersondetails.jpg)

有關導入清單的詳細說明，請參閱[導入人員清單](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)。

幹得好！ 現在，您已瞭解如何避免金鑰欄位受到不受信任的清單的影響。
