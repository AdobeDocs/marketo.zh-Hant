---
description: 安裝Marketo for [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365內部部署步驟3之3 - Marketo檔案 — 產品檔案
title: 為 [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365內部部署步驟3之3安裝Marketo
exl-id: ae801a59-8e29-479c-84c5-a18c7511f21f
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 1%

---

# 步驟3之3：連線Marketo [!DNL Dynamics] （2016年在現場/[!DNL Dynamics] 365內部部署） {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [為 [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365內部部署步驟1 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)安裝Marketo
>* [為 [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365內部部署步驟2 / 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)安裝Marketo

>[!NOTE]
>
>**需要管理員許可權**

## 輸入[!DNL Dynamics]同步使用者資訊 {#enter-dynamics-sync-user-information}

1. 登入Marketo並按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/login-admin.png)

1. 按一下「**[!UICONTROL CRM]**」。

   ![](assets/image2015-3-16-9-47-34.png)

1. 選擇「**[!DNL Microsoft]**」。

   ![](assets/image2015-3-16-9-50-6.png)

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;步驟1：輸入認證&#x200B;**中按一下**。

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >請確認您的認證正確無誤，因為提交後就無法回覆後續的結構描述變更。 如果儲存不正確的認證，您必須取得新的Marketo訂閱。

1. 輸入&#x200B;**使用者名稱**、**密碼** [!DNL Microsoft Dynamics] **URL**&#x200B;和&#x200B;**使用者端識別碼/密碼**。 完成時，按一下&#x200B;**儲存**。

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* 如果您的Marketo是在2020年10月之前布建，使用者端ID和密碼為選用欄位。 否則，這些是強制性的。 能否取得此資訊將取決於您使用的MSD版本。
   >* Marketo中的使用者名稱必須與CRM中同步處理使用者的使用者名稱相符。 格式可以是`user@domain.com`或DOMAIN\user。
   >* 如果您不知道該URL，[請在這裡瞭解如何找到它](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}。

   >[!TIP]
   >
   >不知道URL？ 我們將在此說明如何尋找您的[[!DNL Dynamics] 組織服務URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)。

## 選取要同步的欄位 {#select-fields-to-sync}

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;中按一下&#x200B;**[!UICONTROL Step 2: Select Fields to Sync]**。

   ![](assets/image2015-3-16-9-51-28.png)

1. 選取您要同步至Marketo的欄位，以便預先選取它們。 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo會儲存要同步之欄位的參考。 如果您刪除[!DNL Dynamics]中的欄位，我們建議您在停用[同步處理](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)的情況下進行刪除。 接著，編輯並儲存[選取要同步處理的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)，以重新整理Marketo中的結構描述。

## 自訂篩選器的同步欄位 {#sync-fields-for-a-custom-filter}

如果您已建立自訂篩選器，請務必前往並選取要與Marketo同步的新欄位。

1. 移至[管理]並選取&#x200B;**[!DNL Microsoft Dynamics]**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下[欄位同步處理詳細資料]上的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並進行核取。 實際名稱必須是new_synctomkto，但「顯示名稱」可以是任何內容。 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## 啟用同步 {#enable-sync}

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;中按一下&#x200B;**[!UICONTROL Step 3: Enable Sync]**。

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo不會針對[!DNL Microsoft Dynamics]同步處理或手動輸入人員自動進行重複資料刪除。

1. 閱讀快顯視窗中的所有內容，輸入您的電子郵件，然後按一下&#x200B;**[!UICONTROL Start Sync]**。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 視記錄數量而定，初始同步可能需要數小時至數天的時間。 完成後，您將會收到電子郵件通知。

   ![](assets/image2015-3-16-9-59-51.png)
