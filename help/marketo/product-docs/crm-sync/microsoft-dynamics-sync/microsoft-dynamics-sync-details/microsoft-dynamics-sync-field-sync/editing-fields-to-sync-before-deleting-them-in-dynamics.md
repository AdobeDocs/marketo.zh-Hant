---
description: 在Dynamics - Marketo檔案 — 產品檔案中刪除欄位之前先編輯要同步的欄位
title: 在Dynamics中刪除欄位之前，請先編輯要同步的欄位
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# 在Dynamics中刪除欄位之前，請先編輯要同步的欄位 {#editing-fields-to-sync-before-deleting-them-in-dynamics}

有時您可能會想要刪除Dynamics中的欄位。 Marketo Engage會保留欄位清單，作為同步作業基礎的參考。 如果在同步處理開啟時在Dynamics中刪除欄位，同步處理可能會發生錯誤。 在刪除任何欄位之前，請遵循下列步驟。

1. 在Marketo中，按一下&#x200B;**[!UICONTROL 管理員]**。

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. 在[整合]下，按一下&#x200B;**[!UICONTROL Microsoft Dynamics]**。

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. 按一下&#x200B;**[!UICONTROL 停用同步]**。

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. 在瀏覽器的新索引標籤中，登入Dynamics並刪除所需的欄位。

1. 返回Marketo，在Microsoft Dynamics底下，按一下「步驟2：選取要同步的欄位」旁的&#x200B;**[!UICONTROL 編輯]**。

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. 檢閱欄位並按一下&#x200B;**[!UICONTROL 儲存]**。

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>需要按一下[儲存]****，才能儲存更新的結構描述以進行同步處理，即使未進行任何變更亦然。

>[!NOTE]
>
>如果在刪除Dynamics中的欄位之前未停止同步，則同步可能會遇到錯誤。 如果是，同步將會停止。 在繼續之前，Marketo管理員需要檢閱「選取要同步的欄位」（如上所述）並按一下「**[!UICONTROL 儲存]**」，同步才能接受結構描述變更。

請記得在儲存變更後啟用同步處理！
