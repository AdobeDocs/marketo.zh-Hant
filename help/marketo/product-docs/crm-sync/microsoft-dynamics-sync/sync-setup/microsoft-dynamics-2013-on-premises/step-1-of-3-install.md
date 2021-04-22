---
unique-page-id: 3571813
description: 第1步（共3步）-在Dynamics中安裝Marketo解決方案（2013年內部部署）-Marketo文檔——產品文檔
title: 第1步（共3步）-在Dynamics中安裝Marketo解決方案（2013年內部部署）
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 步驟1（共3步）:在Dynamics中安裝Marketo解決方案（2013年內部部署）{#step-of-install-the-marketo-solution-in-dynamics-on-premises}

在同步Microsoft Dynamics On-On-Promess和Marketo之前，您必須先在Dynamics中安裝Marketo解決方案。

>[!NOTE]
>
>將Marketo同步至CRM後，您無法在沒有取代例項的情況下執行新同步。

>[!PREREQUISITES]
>
>您必須配置[ Internet Facing Deployment](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701)(IFD)和[ Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0、2.1或3.0(ADFS)。 注意：當您按一下連結時，IFD檔案會自動下載。
>
>[開始之前先下](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 載Marketo解決方案。

>[!NOTE]
>
>**需要動態管理權限。**
>
>您需要CRM管理員權限才能執行此同步。

1. 登入&#x200B;**Dynamics**。 按一下&#x200B;**Microsoft Dynamics CRM**&#x200B;下拉菜單並選擇&#x200B;**設定**。

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. 在&#x200B;**Settings**&#x200B;下，選擇&#x200B;**Solutions**。

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. 按一下&#x200B;**Import**。

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. 按一下&#x200B;**瀏覽**&#x200B;並選擇[下載的解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 按一下&#x200B;**Next**。

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. 查看解決方案資訊，然後按一下&#x200B;**查看解決方案包詳細資訊**。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 檢查完所有詳細資訊後，按一下&#x200B;**關閉**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回「解決方案資訊」頁，按一下&#x200B;**Next**。

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. 請確定已勾選SDK選項。 按一下&#x200B;**Import**。

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. 等待匯入完成。

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. 下載日誌檔案（如果需要），然後按一下&#x200B;**Close**。

   >[!NOTE]
   >
   >您可能會看到一則訊息，指出「Marketo銷售線索管理已完成並發出警告」。 這完全是意料之中的。

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo銷售機會管理現在會顯示在&#x200B;**所有解決方案**&#x200B;頁面上。

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. 選擇Marketo解決方案，然後按一下「發佈所有定制」。****

   ![](assets/image2014-12-11-10-3a41-3a32.png)

不是太糟吧？ 來吧，我會一直帶你過去。

>[!CAUTION]
>
>停用任何MarketoSDK傳訊程式將導致安裝中斷！

>[!MORELIKETHIS]
>
>[步驟2（共3步）:為Marketo配置同步用戶（2013年內部）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-2-of-3-configure.md)
