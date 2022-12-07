---
unique-page-id: 2360335
description: 從不受信任的來源匯入清單期間封鎖欄位更新 — Marketo檔案 — 產品檔案
title: 從不受信任的源導入清單期間塊欄位更新
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# 從不受信任的源導入清單期間塊欄位更新 {#block-field-updates-during-list-import-from-untrusted-sources}

您可以比其他清單更信任某些清單中的資料。 有時，如果欄位空白，但現有值不存在，您便會有可疑資料想要擷取。 您可以封鎖關鍵欄位的欄位更新來達成此目的。

>[!NOTE]
>
>**需要管理權限**

## 阻止來自不受信任的源的欄位更新 {#blocking-field-updates-from-untrusted-sources}

1. 前往 **管理** 的上界。

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. 按一下 **欄位管理**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. 找到您想要的欄位，選取它，然後在 **欄位動作**，按一下 **塊欄位更新**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. 檢查 **清單導入不受信任的源** 按一下 **套用**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>您還可以檢查 **清單導入受信任的源**.

對於要避免不受信任清單的任何其他欄位，重複上述步驟。

## 運行不受信任的清單導入 {#running-an-untrusted-list-import}

1. 執行清單匯入時，請務必選取 **不受信任的** 如果您希望在上一步設定的所有欄位都安全。

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

有關導入清單的詳細說明，請參閱 [匯入人員清單](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

幹得好！ 現在，您知道如何確保密鑰欄位免受不受信任的清單的威脅。
