---
description: 在Dynamics - Marketo檔案 — 產品檔案中刪除欄位之前先編輯要同步的欄位
title: 在Dynamics中刪除欄位之前，請先編輯要同步的欄位
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# 在[!DNL Dynamics]中刪除欄位之前，請先編輯要同步的欄位 {#editing-fields-to-sync-before-deleting-them-in-dynamics}

有時您可能會想要刪除[!DNL Dynamics]中的欄位。 Marketo會保留欄位清單，作為同步作業基礎的參考。 如果在同步處理開啟時在[!DNL Dynamics]中刪除欄位，同步處理可能會發生錯誤。 在刪除任何欄位之前，請遵循下列步驟。

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. 在[!UICONTROL Integration]底下，按一下&#x200B;**[!UICONTROL Microsoft Dynamics]**。

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. 按一下「**[!UICONTROL Disable Sync]**」。

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. 在瀏覽器的新索引標籤中，登入[!DNL Dynamics]並刪除所需的欄位。

1. 返回Marketo，在[!DNL Microsoft Dynamics]底下，按一下「**[!UICONTROL Edit]**」旁的[!UICONTROL Step 2: Select Fields to Sync]。

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. 檢閱欄位並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>必須按一下&#x200B;**[!UICONTROL Save]**&#x200B;才能儲存更新的結構描述以進行同步，即使未進行任何變更亦然。

>[!NOTE]
>
>如果在刪除[!DNL Dynamics]中的欄位之前未停止同步，則同步可能會發生錯誤。 如果是，同步將會停止。 在繼續之前，Marketo管理員需要檢閱「[!UICONTROL Select Fields to Sync]」（如上所述）並按一下&#x200B;**[!UICONTROL Save]**，同步才能接受結構描述變更。

請記得在儲存變更後啟用同步處理！
