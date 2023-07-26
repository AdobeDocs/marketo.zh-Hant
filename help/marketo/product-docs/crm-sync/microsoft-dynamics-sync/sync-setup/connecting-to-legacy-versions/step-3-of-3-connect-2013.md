---
unique-page-id: 3571819
description: 步驟3之3 — 連線Marketo和Dynamics （2013內部部署） - Marketo檔案 — 產品檔案
title: 步驟3之3 — 連線Marketo和Dynamics （2013內部部署）
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 步驟3之3：連線Marketo和Dynamics （2013內部部署） {#step-of-connect-marketo-and-dynamics-on-premises}

好啦！ 我們已安裝解決方案並設定同步處理使用者。 接下來，我們需要連線Marketo和Dynamics。

>[!PREREQUISITES]
>
>* [步驟3之1：在Dynamics中安裝Marketo解決方案（2013內部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)
>* [步驟3之2：設定Marketo的同步使用者（2013內部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)

>[!NOTE]
>
>**需要管理員許可權**

## 輸入Dynamics同步使用者資訊 {#enter-dynamics-sync-user-information}

1. 登入Marketo並按一下 **管理員**.

   ![](assets/login-admin.png)

1. 按一下 **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 選取 **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. 按一下 **編輯** 在 **步驟1：輸入認證**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >請確認您的認證正確無誤，因為提交後就無法回覆後續的結構描述變更。 如果儲存不正確的認證，您必須取得新的Marketo訂閱。

1. 輸入 **使用者名稱**， **密碼** 和Microsoft Dynamics **URL** 然後按一下 **儲存**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* Marketo中的使用者名稱必須與CRM中同步處理使用者的使用者名稱相符。 格式可以是user@domain.com或DOMAIN\user。
   >* 如果您不知道URL， [在此處瞭解如何找到它](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

## 選取要同步的欄位 {#select-fields-to-sync}

現在，我們需要選取要同步處理的欄位。

1. 按一下 **編輯** 在 **步驟2：選取要同步的欄位**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 選取您要同步至Marketo的欄位，以便預先選取它們。 按一下 **儲存**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

   >[!NOTE]
   >
   >Marketo會儲存要同步之欄位的參考。 如果您刪除Dynamics中的欄位，建議您使用 [同步已停用](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Marketo接著，透過編輯並儲存 [選取要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## 自訂篩選器的同步欄位 {#sync-fields-for-a-custom-filter}

如果您已建立自訂篩選器，請務必前往並選取要與Marketo同步的新欄位。

1. 前往「管理員」並選取「 」 **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下 **編輯** 欄位同步處理詳細資訊。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並進行核取。 實際名稱必須是new_synctomkto，但「顯示名稱」可以是任何內容。 按一下 **儲存**.

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## 啟用同步 {#enable-sync}

1. 按一下 **編輯** 在 **步驟3：啟用同步**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不會針對Microsoft Dynamics同步處理或手動輸入人員或潛在客戶時，自動進行重複資料刪除。

1. 閱讀快顯視窗中的所有內容，輸入您的電子郵件，然後按一下 **開始同步**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 第一次同步可能需要幾個小時。 完成後，您將會收到電子郵件通知。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

做得很好！ 您剛剛釋放了Marketo和Microsoft Dynamics之間的雙向同步功能。 如果您已購買Marketo Sales Insight，會覺得更有趣：

>[!MORELIKETHIS]
>
>[在Microsoft Dynamics 2013中安裝與設定Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
