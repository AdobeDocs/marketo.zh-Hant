---
unique-page-id: 7504736
description: 安裝Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步驟1（共3步）-行銷檔案——產品檔案
title: 安裝Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步驟1（共3步）
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# 步驟1（共3步）

<!--Install Marketo for Dynamics 2015 On-Prem and 2016 365 On-Prem Step 1 of 3-->

您必須先在Dynamics中安裝Marketo解決方案，才能將Microsoft Dynamics 2015內部或2016(Dynamics 365)與Marketo同步。

>[!NOTE]
>
>將Market與CRM同步後，就無法將新的CRM與現有的Marketo例項同步。

>[!PREREQUISITES]
>
>如果您使用Microsoft Dynamics On-Premise，則必須配置 [Internet Facing Deployment](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD)和 [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+(ADFS)。 注意：當您按一下連結時，IFD檔案會自動下載。
>
>[開始之前，請先下載Marketo Lead Management](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Solution。

>[!NOTE]
>
>**需要動態管理權限。**
>
>您需要CRM管理員權限才能執行此同步。

1. 登入動 **態。** 按一下 **Microsoft Dynamics CRM** 下拉式功能表，並選取「 **設定」**。

   ![](assets/image2015-3-19-8-33-29.png)

1. 在「設 **定**」下，選 **取「解決方案」**。

   ![](assets/image2015-3-19-8-33-3.png)

1. 按一 **下匯入**。

   ![](assets/image2015-3-19-8-34-8.png)

1. 按一 **下「瀏覽** 」並選取您下載的 [解決方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 按一 **下「下一步**」。

   ![](assets/image2015-3-19-9-20-56.png)

1. 查看解決方案資訊，然後按一下查 **看解決方案包詳細資訊**。

   ![](assets/image2015-11-18-11-12-8.png)

1. 檢查完所有詳細資訊後，按一下「關閉」( **Close)**。

   ![](assets/step6.png)

1. 返回「解決方案資訊」頁面，按一下「下 **一步**」。

   ![](assets/image2015-3-19-9-21-50.png)

1. 請確定已選取「SDK選項」核取方塊。 按一 **下匯入**。

   ![](assets/image2015-3-19-9-19-12.png)

1. 等待匯入完成。

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

   ![](assets/image2015-3-11-11-34-9.png)

1. 下載日誌檔案（如果需要），然後按一下「 **Close（關閉）**」。

   >[!NOTE]
   >
   >您可能會看到一則訊息，指出「Marketo Lead Management已完成，但有警告」。 這完全是意料之中的。

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo Lead Management現在會顯示在「所有解決方 **案」頁面** 。

   ![](assets/image2015-3-19-8-40-38.png)

1. 選取Marketo解決方案，然後按一下「 **發佈所有自訂」**。

   ![](assets/image2015-3-19-8-41-21.png)

   擊掌！ 安裝完成。

   >[!CAUTION]
   >
   >停用任何Marketo SDK訊息處理程式將導致安裝中斷！

   >[!NOTE]
   >
   >**相關文章**
   >
   >
   >[安裝Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步驟2（共3步）](step-2-of-3-set-up.md)
