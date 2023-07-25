---
unique-page-id: 2360335
description: 從不受信任的來源匯入清單期間封鎖欄位更新 — Marketo檔案 — 產品檔案
title: 從不受信任的來源匯入清單期間封鎖欄位更新
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# 從不受信任的來源匯入清單期間封鎖欄位更新 {#block-field-updates-during-list-import-from-untrusted-sources}

某些清單中的資料較其他清單中的資料更值得信任。 有時候，您會有可疑的資料，並且如果欄位為空白就想要取得，但現有值時則不行。 您可以封鎖關鍵欄位的欄位更新來完成此操作。

>[!NOTE]
>
>**需要管理員許可權**

## 封鎖來自不受信任來源的欄位更新 {#blocking-field-updates-from-untrusted-sources}

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. 按一下 **[!UICONTROL 欄位管理]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. 找到所需的欄位，選取該欄位，然後在 **[!UICONTROL 欄位動作]**，按一下 **[!UICONTROL 封鎖欄位更新]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Check **[!UICONTROL 清單匯入不受信任的來源]** 並按一下 **[!UICONTROL 套用]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>您可以透過檢查來確保所有清單中受信任和未受信任的欄位的安全 **[!UICONTROL 清單匯入信任的來源]**.

針對您想要防止不受信任清單影響的任何其他欄位，重複上述步驟。

## 執行不受信任的清單匯入 {#running-an-untrusted-list-import}

1. 執行清單匯入時，請務必選取 **[!UICONTROL 不受信任]** 如果您希望在上一步中設定的所有欄位都是安全的。

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

如需匯入清單的詳細說明，請參閱 [匯入人員清單](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

做得很好！現在您知道如何保護金鑰欄位免受不受信任清單的侵擾。
