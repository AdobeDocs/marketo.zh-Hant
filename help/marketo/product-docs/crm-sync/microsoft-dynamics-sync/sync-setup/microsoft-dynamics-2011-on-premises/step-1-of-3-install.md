---
unique-page-id: 3571805
description: 第1步（共3步）-安裝Marketo解決方案（2011年內部部署）-Marketo文檔——產品文檔
title: 第1步（共3步）-安裝Marketo解決方案（2011年內部部署）
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 步驟1（共3步）:安裝Marketo解決方案（2011年內部部署）{#step-of-install-the-marketo-solution-on-premises}

在同步Microsoft Dynamics On-On-Promess和Marketo之前，您必須先在Dynamics中安裝Marketo解決方案。

>[!NOTE]
>
>將Marketo同步至CRM後，您無法在沒有取代例項的情況下執行新同步。

>[!PREREQUISITES]
>
>您必須配置[ Internet Facing Deployment](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701)(IFD)和[ Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0、2.1或3.0(ADFS)。 **注意**:當您按一下連結時，IFD檔案會自動下載。
>
>[開始之前，請先下載Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 銷售機會管理解決方案。

>[!NOTE]
>
>**需要動態管理權限。**
>
>您需要CRM管理員權限才能執行此同步。

1. 登入&#x200B;**Dynamics**，在左下角的選單中選擇&#x200B;**Settings**。

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. 在樹中選擇&#x200B;**Solutions**。

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. 按一下&#x200B;**Import**。

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. 按一下&#x200B;**瀏覽**。 選擇您[downloaded](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)的Marketo銷售線索管理解決方案。 按一下&#x200B;**Next**。

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. 查看解決方案資訊，然後按一下&#x200B;**查看解決方案包詳細資訊**。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 檢查完所有詳細資訊後，按一下&#x200B;**關閉**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回「解決方案資訊」頁，按一下&#x200B;**Next**。

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. 請確定已勾選SDK訊息選項核取方塊。 按一下&#x200B;**Next**。

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

1. 現在，請等待匯入完成。 起來，做些伸展。

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. 按一下&#x200B;**關閉**。

   >[!NOTE]
   >
   >您可能會看到一則訊息，指出「Marketo銷售線索管理已完成並發出警告」。 這完全是意料之中的。

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketo銷售機會管理現在會顯示在&#x200B;**所有解決方案**&#x200B;頁面上。

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. 選擇「Marketo銷售線索管理」，然後按一下「發佈所有定制」。****

   ![](assets/image2015-4-2-11-3a48-3a21.png)

不是太糟吧？ 來吧，我會一直帶你過去。

>[!CAUTION]
>
>停用任何MarketoSDK傳訊程式將導致安裝中斷！

>[!MORELIKETHIS]
>
>[步驟2（共3步）:在Dynamics中設定Marketo同步使用者（2011年內部）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)
