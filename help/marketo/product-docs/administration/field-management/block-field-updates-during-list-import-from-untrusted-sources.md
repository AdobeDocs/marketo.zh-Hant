---
unique-page-id: 2360335
description: 從不受信任的來源匯入清單期間封鎖欄位更新 — Marketo檔案 — 產品檔案
title: 清單匯入期間封鎖來自不信任來源的欄位更新
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 13%

---

# 清單匯入期間封鎖來自不信任來源的欄位更新 {#block-field-updates-during-list-import-from-untrusted-sources}

某些清單中的資料比其他清單中的資料更可信。 有時候，您會有可疑的資料，如果欄位為空白，您會想要取得，但如果現有值則不然。 您可以封鎖主要欄位的欄位更新來完成此操作。

>[!NOTE]
>
>**需要管理員許可權**

## 封鎖來自不受信任來源的欄位更新 {#blocking-field-updates-from-untrusted-sources}

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. 按一下「**[!UICONTROL Field Management]**」。

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. 找到您要的欄位，選取它，然後在&#x200B;**[!UICONTROL Field Actions]**&#x200B;下按一下&#x200B;**[!UICONTROL Block Field Updates]**。

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. 檢查&#x200B;**[!UICONTROL List Import untrusted source]**&#x200B;並按一下&#x200B;**[!UICONTROL Apply]**。

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>您可以透過檢查&#x200B;**[!UICONTROL List Import trusted source]**&#x200B;來防止所有清單中的欄位受到信任和不受信任。

針對您想要防止未受信任清單出現的任何其他欄位，重複上述步驟。

## 執行不受信任的清單匯入 {#running-an-untrusted-list-import}

1. 執行清單匯入時，如果您希望在上一步中設定的所有欄位都安全，請務必選取&#x200B;**[!UICONTROL Untrusted]**。

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

如需匯入清單的詳細說明，請參閱[匯入人員清單](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)。

做得很好！現在您知道如何保護金鑰欄位免受不受信任清單的影響。
