---
description: 在Dynamics -Marketo文檔——產品文檔中刪除欄位之前，先編輯要同步的欄位
title: 在Dynamics中刪除欄位之前，先編輯欄位以進行同步
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# 在Dynamics {#editing-fields-to-sync-before-deleting-them-in-dynamics}中刪除欄位之前，先編輯欄位以進行同步

有時您可能想要刪除Dynamics中的欄位。 Marketo保留欄位清單作為同步的基礎的參考。 如果在同步啟動時在Dynamics中刪除欄位，同步可能會遇到錯誤。 在刪除任何欄位之前，請依照下列步驟進行。

1. 在Marketo，按一下&#x200B;**管理**。

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. 在「整合」下，按一下「**Microsoft Dynamics**」。

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. 按一下&#x200B;**禁用同步**。

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. 在瀏覽器的新標籤中，登入Dynamics並刪除您想要的欄位。

1. 回到Marketo，在Microsoft Dynamics下，按一下「步驟2:選擇要同步的欄位。」****

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. 檢閱欄位，然後按一下「儲存&#x200B;**」。**

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>按一下&#x200B;**Save**&#x200B;將需要保存更新的同步模式，即使未進行任何更改也是如此。

>[!NOTE]
>
>如果在刪除Dynamics中的欄位之前未停止同步，則同步可能會遇到錯誤。 如果有，同步將停止。 在繼續之前，Marketo管理員需要查看「選擇要同步的欄位」（上面討論），然後按一下&#x200B;**保存** ，以便同步接受模式更改。

請記得在儲存變更後啟用同步！
