---
unique-page-id: 3571819
description: 步驟3之3 — 連線Marketo和Dynamics （2013內部部署） - Marketo檔案 — 產品檔案
title: 步驟3之3 — 連線Marketo和Dynamics （2013內部部署）
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# 步驟3之3：連線Marketo和[!DNL Dynamics] （2013年內部部署） {#step-of-connect-marketo-and-dynamics-on-premises}

好啦！ 我們已安裝解決方案並設定同步處理使用者。 接下來，我們需要連線Marketo和[!DNL Dynamics]。

>[!PREREQUISITES]
>
>* [步驟3之1：在 [!DNL Dynamics] （2013年內部部署）中安裝Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)
>* [步驟2之3：設定Marketo （2013內部部署）的同步使用者](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)

>[!NOTE]
>
>**需要管理員許可權**

## 輸入[!DNL Dynamics]同步使用者資訊 {#enter-dynamics-sync-user-information}

1. 登入Marketo並按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/login-admin.png)

1. 按一下&#x200B;**[!UICONTROL CRM]**。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 選擇「**[!DNL Microsoft]**」。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;中按一下&#x200B;**[!UICONTROL Step 1: Enter Credentials]**。

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >請確認您的認證正確無誤，因為提交後就無法回覆後續的結構描述變更。 如果儲存不正確的認證，您必須取得新的Marketo訂閱。

1. 輸入&#x200B;**[!UICONTROL Username]**、**[!UICONTROL Password]**&#x200B;和[!DNL Microsoft Dynamics] **URL**，然後按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* Marketo中的使用者名稱必須與CRM中同步處理使用者的使用者名稱相符。 格式可以是`user@domain.com`或DOMAIN\user。
   >* 如果您不知道該URL，[請在這裡瞭解如何找到它](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}。

## 選取要同步的欄位 {#select-fields-to-sync}

現在，我們需要選取要同步處理的欄位。

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;中按一下&#x200B;**[!UICONTROL Step 2: Select Fields to Sync]**。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 選取您要同步至Marketo的欄位，以便預先選取它們。 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2016-8-25-15-3a10-3a17.png)

   >[!NOTE]
   >
   >Marketo會儲存要同步之欄位的參考。 如果您刪除[!DNL Dynamics]中的欄位，我們建議您在停用[同步處理](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)的情況下進行刪除。 然後編輯並儲存[[!UICONTROL Select Fields to Sync]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)，以重新整理Marketo中的結構描述。

## 自訂篩選器的同步欄位 {#sync-fields-for-a-custom-filter}

如果您已建立自訂篩選器，請務必前往並選取要與Marketo同步的新欄位。

1. 移至[!UICONTROL Admin]並選取&#x200B;**[!UICONTROL Microsoft Dynamics]**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;上按一下[!UICONTROL Field Sync Details]。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並進行核取。 實際名稱必須是new_synctomkto，但「顯示名稱」可以是任何內容。 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## 啟用同步 {#enable-sync}

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;中按一下&#x200B;**[!UICONTROL Step 3: Enable Sync]**。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不會針對[!DNL Microsoft Dynamics]同步處理或手動輸入人員或潛在客戶時，自動進行重複資料刪除。

1. 閱讀快顯視窗中的所有內容，輸入您的電子郵件，然後按一下&#x200B;**[!UICONTROL Start Sync]**。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 視記錄數量而定，初始同步可能需要數小時至數天的時間。 完成後，您將會收到電子郵件通知。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

做得很好！ 您剛剛釋放了Marketo與[!DNL Microsoft Dynamics]之間的雙向同步功能。 如果您已購買[!DNL Marketo Sales Insight]，則會有更多樂趣：

>[!MORELIKETHIS]
>
>[在 [!DNL Marketo Sales Insight] 2013 [!DNL Microsoft Dynamics] 中安裝並設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
