---
unique-page-id: 3571819
description: 第3步（共3步）-連接Marketo和動態（2013年內部部署）-Marketo文檔——產品文檔
title: 第3步（共3步）-連接Marketo和動力（2013年內部部署）
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 步驟3（共3步）:連接Marketo和動力（2013年內部部署）{#step-of-connect-marketo-and-dynamics-on-premises}

好吧！ 我們安裝瞭解決方案並配置了同步用戶。 接下來，我們需要將Marketo和動態公司聯繫起來。

>[!PREREQUISITES]
>
>* [步驟1（共3步）:在Dynamics中安裝Marketo解決方案（2013年內部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)
>* [步驟2（共3步）:為Marketo配置同步用戶（2013年內部）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-2-of-3-configure.md)


>[!NOTE]
>
>**需要管理員權限**

## 輸入動態同步用戶資訊{#enter-dynamics-sync-user-information}

1. 登入Marketo，然後按一下「管理員」。****

   ![](assets/login-admin.png)

1. 按一下&#x200B;**CRM**。

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. 選擇&#x200B;**Microsoft**。

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. 按一下&#x200B;**步驟1中的**&#x200B;編輯&#x200B;**:輸入憑據**。

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >請確定您的認證正確，因為我們無法在提交後回復後續的架構變更。 如果儲存的憑證不正確，您必須取得新的Marketo訂閱。

1. 輸入&#x200B;**Username**、**Password**&#x200B;和Microsoft Dynamics **URL**，然後按一下&#x200B;**Save**。

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* Marketo的使用者名稱必須符合CRM中同步使用者的使用者名稱。 格式可以是user@domain.com或DOMAIN\user。
   >* 如果您不知道URL，請[學習如何在這裡找到](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)。


## 選擇要同步的欄位{#select-fields-to-sync}

現在，我們需要選取要同步的欄位。

1. 按一下「步驟2:選擇要同步的欄位&#x200B;**。******

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 選擇您要同步至Marketo的欄位，以便預先選取欄位。 按一下&#x200B;**保存**。

   ![](assets/image2016-8-25-15-3a10-3a17.png)

   >[!NOTE]
   >
   >Marketo儲存要同步的欄位參考。 如果您刪除Dynamics中的欄位，我們建議您在[sync disabled](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)下執行此動作。 然後，通過編輯和保存[選擇要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)來刷新Marketo的模式。

## 同步自訂篩選器的欄位{#sync-fields-for-a-custom-filter}

如果您已建立自訂篩選，請務必前往並選取要與Marketo同步的新欄位。

1. 前往「管理員」並選取「**Microsoft Dynamics**」。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下欄位同步詳細資訊上的&#x200B;**編輯**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並加以檢查。 實際名稱必須是new_synctomkto，但「顯示名稱」可以是任何內容。 按一下&#x200B;**保存**。

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## 啟用同步{#enable-sync}

1. 按一下&#x200B;**步驟3中的**&#x200B;編輯&#x200B;**:啟用Sync**。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不會針對Microsoft Dynamics同步或手動輸入人員或銷售線索時自動消除重複資料。

1. 閱讀快顯視窗中的所有內容，輸入您的電子郵件，然後按一下「開始同步」**。**

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 第一次同步可能需要幾個小時。 完成後，您會收到電子郵件通知。

   ![](assets/image2014-12-11-11-3a55-3a15.png)

幹得漂亮！ 您剛剛釋放了Marketo和微軟動態公司之間雙向同步的力量。 如果您已購買Marketo銷售分析，則有更多樂趣：

>[!MORELIKETHIS]
>
>[在Microsoft Dynamics 2013中安裝和設定Marketo銷售分析](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
