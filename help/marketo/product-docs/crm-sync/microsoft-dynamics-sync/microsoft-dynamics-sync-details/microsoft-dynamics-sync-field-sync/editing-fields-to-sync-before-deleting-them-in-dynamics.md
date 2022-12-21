---
description: 在Dynamics - Marketo檔案 — 產品檔案中編輯欄位以同步再加以刪除
title: 在Dynamics中刪除欄位之前編輯要同步的欄位
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# 在Dynamics中刪除欄位之前編輯要同步的欄位 {#editing-fields-to-sync-before-deleting-them-in-dynamics}

有時您可能想要刪除Dynamics中的欄位。 Marketo會保留欄位清單作為同步的基礎參考。 如果在同步開啟時在Dynamics中刪除了欄位，同步可能會遇到錯誤。 刪除任何欄位之前，請遵循下列步驟。

1. 在Marketo中，按一下 **管理**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. 在整合下方，按一下 **Microsoft Dynamics**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. 按一下 **禁用同步**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. 在瀏覽器的新索引標籤中，登入Dynamics並刪除您想要的欄位。

1. 返回Marketo，在Microsoft Dynamics底下，按一下 **編輯** 在「步驟2:選擇要同步的欄位。」

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. 檢閱欄位，然後按一下 **儲存**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>按一下 **儲存** 即使未進行任何變更，仍需要儲存更新的架構以進行同步。

>[!NOTE]
>
>如果在刪除Dynamics中的欄位之前未停止同步，則同步可能會遇到錯誤。 如果有，同步將停止。 繼續之前，Marketo管理員需要檢閱「選取要同步的欄位」（如上所述），然後按一下 **儲存** 以便同步接受架構更改。

請記得在儲存變更後啟用同步！
