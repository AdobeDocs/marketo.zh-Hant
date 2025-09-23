---
unique-page-id: 1146987
description: 刪除流程步驟 — Marketo檔案 — 產品檔案
title: 刪除流程步驟
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 2%

---

# 刪除流程步驟 {#delete-a-flow-step}

>[!CAUTION]
>
>移除作用中Smart Campaigns的流程步驟&#x200B;_尤其是等待步驟_，可能會產生非預期的結果。 請仔細閱讀本文。

首先，我們來介紹基本知識。 以下說明如何從Smart Campaign移除不要的流程步驟。

1. 在Smart Campaign **[!UICONTROL Flow]**&#x200B;中，按一下&#x200B;**X**&#x200B;圖示以刪除任何流程步驟。

   ![](assets/delete-a-flow-step-1.png)

1. 按一下「**[!UICONTROL Delete]**」。

   ![](assets/delete-a-flow-step-2.png)

   >[!CAUTION]
   >
   >在&#x200B;_作用中_&#x200B;行銷活動中刪除、新增和移動步驟絕對會產生非預期的結果。 考慮建立新行銷活動、測試並切換。

   您可以對作用中的行銷活動進行變更，但可能會產生無法預見的後果。 詳細資料如下：

   **批次智慧行銷活動**

   如果您的行銷活動：

   1. **從未執行**。 進行您想要的所有變更。 在您執行該行銷活動之前，這不會影響任何人。
   1. **是週期性智慧行銷活動**。 這些變更將會影響未來執行中的人，而不是先前的執行。
   1. **已在沒有等待步驟的情況下執行**。不會有任何人員受到影響，因為行銷活動在執行後處於休眠狀態。
   1. **正在執行**。 變更可能會造成非預期的行為，具體取決於刪除的時間與詳細資訊。 我們強烈建議不要編輯作用中執行的批次行銷活動。 在緊急情況下，瞭解如何[中止執行中的Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md){target="_blank"}。

   1. **已執行等待步驟。**此專案的幾個詳細資料。
當人員進入等待步驟時，人員會記下持續時間以及要返回的NUMBER STEP。 請參閱下列範例。

   **觸發智慧行銷活動**

   1. **沒有等待步驟**。 如果您刪除正常步驟，則只有未來執行促銷活動的人會受到影響。
   1. **等待步驟**。 如需批次促銷活動的相關資訊，請參閱以下範例。 適用同樣的邏輯。

   >[!NOTE]
   >
   >**範例**
   >
   >1. Smart Campaign有3個步驟。
   >    * 步驟1. 傳送電子郵件#1
   >    * 步驟2. 等待1週
   >    * 步驟3. 傳送電子郵件#2
   >
   >1. 點選&#x200B;**步驟2**&#x200B;的人員將等待1週再繼續進行&#x200B;**步驟3**。
   >1. 您在一週內刪除&#x200B;**步驟2**。
   >1. 人們將繼續等候1週（他們不會自動回到流量中）。
   >1. 當他們最終回訪時，將嘗試移至&#x200B;**步驟3**。 他們找不到。
   >1. **重要：**&#x200B;由於現在只有2個步驟，人員&#x200B;_將不會收到電子郵件#2_。
