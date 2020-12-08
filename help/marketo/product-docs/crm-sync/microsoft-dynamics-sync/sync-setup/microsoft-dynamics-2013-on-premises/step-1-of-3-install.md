---
unique-page-id: 3571813
description: 第1步（共3步）-在Dynamics（2013年內部部署）中安裝Marketo解決方案——行銷檔案——產品檔案
title: 第1步（共3步）-在Dynamics中安裝Marketo解決方案（2013年內部部署）
translation-type: tm+mt
source-git-commit: ce8b67b8549d23ff4ddd1d341632c6c5ff33990d
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# 步驟1（共3步）:在Dynamics中安裝Marketo解決方案（2013年內部部署） {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

在同步Microsoft Dynamics On-On-Promess和Marketo之前，您必須先在Dynamics中安裝Marketo解決方案。

>[!NOTE]
>
>將Market與CRM同步後，若不取代例項，就無法執行新同步。

>[!NOTE]
>
>**必要條件**
>
>您必須已 [配置Active Directory Federation Services](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) 2.0、2.1或3.0(ADFS)的Internet Packing Deployment [](https://msdn.microsoft.com/en-us/library/bb897402.aspx) (IFD)。 注意：當您按一下連結時，IFD檔案會自動下載。
>
>[開始之前，請先下載Marketo Solution](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 。

>[!NOTE]
>
>**需要動態管理權限。**
>
>您需要CRM管理員權限才能執行此同步。

1. 登入 **Dynamics**。 按一下 **Microsoft Dynamics CRM** 下拉式功能表，並選取「 **設定」**。

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. 在「設 **定**」下，選 **擇「解決方案」**。

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. 按一 **下匯入**。

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. 按一 **下「瀏覽** 」並選取下 [載的解決方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 按一 **下「下一步**」。

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. 查看解決方案資訊，然後按一下查 **看解決方案包詳細資訊**。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 檢查完所有詳細資訊後，按一下「關閉」( **Close)**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回「解決方案資訊」頁面，按一下「下 **一步**」。

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. 請確定已勾選SDK選項。 按一 **下匯入**。

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. 等待匯入完成。

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. 下載日誌檔案（如果需要），然後按一下「 **Close（關閉）**」。

   >[!NOTE]
   >
   >您可能會看到一則訊息，指出「Marketo Lead Management已完成，但有警告」。 這完全是意料之中的。

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo Lead Management現在會顯示在「所有解決方 **案」頁面** 。

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. 選取Marketo解決方案，然後按一下「 **發佈所有自訂」**。

   ![](assets/image2014-12-11-10-3a41-3a32.png)

不是太糟吧？ 來吧，我會一直帶你過去。

>[!CAUTION]
>
>停用任何Marketo SDK訊息處理程式將導致安裝中斷！

>[!NOTE]
>
>**相關文章**
>
>* [步驟2（共3步）:為Marketo設定同步使用者（2013年內部部署）](step-2-of-3-configure.md)

>



