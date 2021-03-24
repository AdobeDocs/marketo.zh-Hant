---
unique-page-id: 7504744
description: 安裝Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步驟3（共3步）-行銷檔案——產品檔案
title: 安裝Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步驟3（共3步）
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---


# 步驟3（共3步）:Connect Marketo Dynamics（2015 On-Prem和2016 365 On-Prem）{#step-of-connect-marketo-dynamics-on-premises-and-365}

>[!PREREQUISITES]
>
>* [安裝Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步驟1（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)
>* [安裝Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步驟2（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**需要管理員權限**

## 輸入動態同步用戶資訊{#enter-dynamics-sync-user-information}

1. 登入Marketo，然後按一下&#x200B;**管理**。

   ![](assets/login-admin.png)

1. 按一下&#x200B;**CRM**。

   ![](assets/image2015-3-16-9-47-34.png)

1. 選擇&#x200B;**Microsoft**。

   ![](assets/image2015-3-16-9-50-6.png)

1. 按一下&#x200B;**步驟1中的**&#x200B;編輯&#x200B;**:輸入憑據**。

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >請確定您的認證正確，因為我們無法在提交後回復後續的架構變更。 如果儲存的憑證不正確，您必須取得新的Marketo訂閱。

1. 輸入&#x200B;**Username**、**Password**&#x200B;和&#x200B;**Microsoft Dynamics** URL **，以及Client Id/Secret**。 完成時，按一下「保存」。****

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* 如果您的Marketo在2020年10月之前已布建，則「用戶端ID」和「密碼」是選填欄位。 否則，就是強制性的。 獲取此資訊將取決於您使用的MSD版本。
   >* Market中的使用者名稱必須符合CRM中同步使用者的使用者名稱。 格式可以是`user@domain.com`或DOMAIN\user。
   >* 如果您不知道URL，請[學習如何在這裡找到](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)。


   >[!TIP]
   >
   >不知道網址嗎？ 我們將向您展示如何在此處找到[Dynamics Organization Service URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)。

## 選擇要同步的欄位{#select-fields-to-sync}

1. 按一下「步驟2:選擇要同步的欄位&#x200B;**。******

   ![](assets/image2015-3-16-9-51-28.png)

1. 選取您要同步至Marketo的欄位，以便預先選取這些欄位。 按一下&#x200B;**保存**。

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo儲存要同步之欄位的參考。 如果您刪除Dynamics中的欄位，我們建議您在[sync disabled](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)下執行此動作。 然後，編輯並儲存[選擇要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)，以重新整理Marketo中的架構。

## 同步自訂篩選器的欄位{#sync-fields-for-a-custom-filter}

如果您已建立自訂篩選，請務必前往並選取要與Marketo同步的新欄位。

1. 前往「管理員」並選取「**Microsoft Dynamics**」。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下欄位同步詳細資訊上的&#x200B;**編輯**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並加以檢查。 實際名稱必須是new_synctomkto，但「顯示名稱」可以是任何內容。 按一下&#x200B;**保存**。

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## 啟用同步{#enable-sync}

1. 按一下&#x200B;**步驟3中的**&#x200B;編輯&#x200B;**:啟用Sync**。

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo不會針對Microsoft Dynamics同步或手動輸入人員時自動消除重複資料。

1. 閱讀快顯視窗中的所有內容，輸入您的電子郵件，然後按一下「開始同步」**。**

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 第一次同步可能需要幾個小時。 完成後，您會收到電子郵件通知。

   ![](assets/image2015-3-16-9-59-51.png)

幹得漂亮！
