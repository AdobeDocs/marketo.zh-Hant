---
unique-page-id: 3571809
description: 第3步（共3步）-將Microsoft Dynamics與Marketo（2011年內部部署）-行銷人員檔案——產品檔案
title: 第3步（共3步）-將Microsoft Dynamics與Marketo連接（2011年內部部署）
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# 步驟3（共3步）:將Microsoft Dynamics與Marketo連接（2011年內部部署） {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

好吧！ 我們安裝瞭解決方案並配置了同步用戶。 接下來，我們需要將Marketo和Dynamics連結在一起。

>[!PREREQUISITES]
>
>* [步驟1（共3步）:安裝Marketo解決方案（2011年內部部署）](step-1-of-3-install.md)
>* [步驟2（共3步）:在Dynamics中設定Marketto同步使用者（2011年內部部署）](step-2-of-3-set-up.md)


>[!NOTE]
>
>**需要管理員權限**

## 輸入動態同步用戶資訊 {#enter-dynamics-sync-user-information}

1. 登入Marketo，然後按一下「管 **理員**」。

   ![](assets/login-admin.png)

1. 按一下 **CRM**。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 按一 **下Microsoft**。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. 按一 **下步驟** 1 **中的編輯：輸入憑據。**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >請確定您的認證正確，因為我們無法在提交後回復後續的架構變更。 如果儲存的憑證不正確，您必須取得新的Marketo訂閱。

1. 輸入 **Username**、 **Password** 和CRM **URL** ，然 **後按一下Save** Reactive Rel。

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >Market中的使用者名稱必須符合CRM中同步使用者的使用者名稱。 格式可以是 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#a0d5d3c5d2e0c4cfcdc1c9ce8ec3cfcd) 或DOMAIN\user。

   >[!TIP]
   >
   >不知道網址嗎？ 我們將示範如何在此處尋 [找Dynamics Organization Service URL](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) 。

## 選擇要同步的欄位 {#select-fields-to-sync}

現在，我們需要選取要同步的欄位。

1. 按一 **下**&#x200B;步驟&#x200B;**2中的編輯：選擇要同步的欄位。**

   ![](assets/image2015-3-16-9-51-28a.png)

1. 有預先選取的欄位將會同步。 視需要新增更多，然後按一下「 **儲存**」。

   ![](assets/image2016-8-25-13-3a26-3a14.png)

## 同步自訂篩選器的欄位 {#sync-fields-for-a-custom-filter}

如果您已建立自訂篩選，請務必前往並選取要與Marketo同步的新欄位。

1. 前往「管理員」並選 **取Microsoft Dynamics**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下 **欄位同步** 「詳細資訊」上的「編輯」。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並加以檢查。 實際名稱必須是new_synctomkto，但「顯示名稱」可以是任何內容。 按一下 **儲存**。

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## 啟用同步 {#enable-sync}

1. 按一 **下步驟** 3 **中的編輯：啟用同步**。

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo不會針對Microsoft Dynamics同步或當您手動輸入人員或潛在客戶時自動消除重複資料。

1. 閱讀快顯視窗中的所有內容，輸入您的電子郵件，然後按一下「開 **始同步」**。

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 第一次同步可能需要幾個小時。 完成後，您會收到電子郵件通知。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   幹得漂亮！
