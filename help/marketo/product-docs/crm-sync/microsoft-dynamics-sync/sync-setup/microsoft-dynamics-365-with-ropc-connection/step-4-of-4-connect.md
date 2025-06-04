---
description: 步驟4之4 — 使用資源所有者密碼控制連線來連線Marketo解決方案 — Marketo檔案 — 產品檔案
title: 步驟4之4 — 使用資源擁有者密碼控制連線來連線Marketo解決方案
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
feature: Microsoft Dynamics
source-git-commit: 2d3264ab75d2327f9226373aad383e7a51508589
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 步驟4之4：使用資源擁有者密碼控制連線來連線Marketo解決方案 {#step-4-of-4-connect-the-marketo-solution-ropc}

這是同步的最後一個步驟。 您即將完成！

>[!PREREQUISITES]
>
>* [步驟4之1：安裝具有資源擁有者密碼控制連線的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [步驟2之4：使用資源擁有者密碼控制連線設定Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}
>* [步驟4之3：在MS Dynamics上設定使用者端應用程式](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}

>[!NOTE]
>
>**需要管理員許可權**

>[!NOTE]
>
>如果您正在從基本驗證升級為OAuth，您可以使用[此文章](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"}來重新設定您的驗證。

## 輸入Dynamics同步使用者資訊 {#enter-dynamics-sync-user-information}

1. 登入Marketo並按一下&#x200B;**A分鐘**。

   ![](assets/login-admin.png)

1. 按一下「**[!UICONTROL CRM]**」。

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 選擇「**[!UICONTROL Microsoft]**」。

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. 在&#x200B;**[!UICONTROL Enter Credentials]**&#x200B;中按一下&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >請確認您的組織URL正確無誤，因為提交後即無法回覆後續的結構描述變更。 如果使用錯誤的組織URL，您必須取得新的Marketo訂閱。 如果您不知道該URL，[請在這裡瞭解如何找到它](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}。

   >[!NOTE]
   >
   >輸入新認證之前，您可以[在此驗證認證](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}。

1. 輸入&#x200B;**[!UICONTROL Username]**、**[!UICONTROL Password]**、Microsoft Dynamics **URL**、**[!UICONTROL Client ID]**&#x200B;和&#x200B;**[!UICONTROL Client Secret]**。 完成時，按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >Marketo中的使用者名稱必須與CRM中同步處理使用者的使用者名稱相符。 格式可以是`user@domain.com`或DOMAIN\user。

## 選取要同步的欄位 {#select-fields-to-sync}

1. 在&#x200B;**[!UICONTROL Select Fields to Sync]**&#x200B;中按一下&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 選取您要同步至Marketo的欄位，以便預先選取它們。 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo會儲存要同步之欄位的參考。 如果您刪除Dynamics中的欄位，我們建議您在停用[同步處理](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}的情況下進行刪除。 接著，編輯並儲存[選取要同步處理的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}，以重新整理Marketo中的結構描述。

## 自訂篩選器的同步欄位 {#sync-fields-for-a-custom-filter}

如果您已建立自訂篩選器，請務必前往並選取要與Marketo同步的新欄位。

1. 移至[管理]並選取&#x200B;**[!DNL Microsoft Dynamics]**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下[欄位同步處理詳細資料]上的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並進行核取。 實際名稱必須是new_synctomkto，但「顯示名稱」可以是任何內容。 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 啟用同步 {#enable-sync}

1. 在&#x200B;**[!UICONTROL Enable Sync]**&#x200B;中按一下&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不會針對Microsoft Dynamics同步處理或手動輸入人員或潛在客戶時，自動進行重複資料刪除。

1. 讀取快顯視窗中的所有內容，輸入您的電子郵件地址，然後按一下&#x200B;**[!UICONTROL Start Sync]**。

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 視記錄數量而定，初始同步可能需要數小時至數天的時間。 完成後，您將會收到電子郵件通知。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

>[!MORELIKETHIS]
>
>[重新設定Dynamics驗證方法](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"}
