---
unique-page-id: 2953384
description: 為自訂實體啟用同步 — Marketo檔案 — 產品檔案
title: 為自訂實體啟用同步
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: d522950af40c5e3e702a6522101ebe9550432be5
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# 為自訂實體啟用同步 {#enable-sync-for-a-custom-entity}

如果您需要來自Dynamics的自訂實體資料才能在Marketo Engage中使用，以下說明如何為其啟用同步。

>[!NOTE]
>
>**需要管理員許可權**

>[!NOTE]
>
>* 當您啟用自訂實體的同步時，Marketo會執行初始同步以引入自訂物件的所有資料。
>* 行銷清單和行銷清單成員為 _不支援_ 此時。

>[!IMPORTANT]
>
>Marketo同步使用者需要自訂物件的讀取存取權，才能列出該物件並對其執行同步。

1. 前往 **[!UICONTROL 管理員]** 區段。

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. 選取 **[!UICONTROL Microsoft Dynamics]** 並按一下 **[!UICONTROL 停用同步]**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >您必須暫時停用全域同步才能啟用或停用自訂實體。

1. 在資料庫管理底下，按一下 **[!UICONTROL Dynamics實體同步]**.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. 按一下 **[!UICONTROL 同步結構描述]**.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. 選取要同步的實體，然後按一下 **[!UICONTROL 啟用同步]**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. 選取您要同步或做為使用的欄位 [限制](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) 和/或觸發器(針對新增的記錄， _非_ 更新)。 完成後，按一下 **[!UICONTROL 啟用同步]**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >在同步處理期間，您可能會注意到&quot;[!UICONTROL 動態實體同步]「專案會從導覽樹狀結構中消失。 這是預期行為，同步完成後將會重新出現。

1. 該實體現在有綠色核取記號。

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. 別忘了重新啟用全域同步處理！

   ![](assets/enable-sync-for-a-custom-entity-8.png)
