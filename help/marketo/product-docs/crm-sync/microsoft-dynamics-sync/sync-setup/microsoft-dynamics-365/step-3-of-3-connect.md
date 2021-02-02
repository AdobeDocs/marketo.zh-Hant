---
unique-page-id: 3571830
description: 第3步（共3步）-將Microsoft Dynamics與Marketo（線上）連接- Marketo Docs —— 產品檔案
title: 第3步（共3步）-將Microsoft Dynamics與Marketo連接（線上）
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# 步驟3（共3步）:將Microsoft Dynamics與Marketo連接（線上）{#step-of-connect-microsoft-dynamics-with-marketo-online}

這是同步的最後一步。 快到了！

>[!PREREQUISITES]
>
>* [步驟1（共3步）:安裝Marketo解決方案（線上）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)
   >
   >
* [步驟2（共3步）:在Dynamics中設定Marketto同步使用者](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)


>[!NOTE]
>
>**需要管理員權限**

## 輸入動態同步用戶資訊{#enter-dynamics-sync-user-information}

1. 登入Marketo，然後按一下&#x200B;**管理**。

   ![](assets/login-admin.png)

1. 按一下&#x200B;**CRM**。

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 選擇&#x200B;**Microsoft**。

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. 按一下&#x200B;**步驟1中的**&#x200B;編輯&#x200B;**:輸入憑據**。

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >請確定您的認證正確，因為我們無法在提交後回復後續的架構變更。 如果儲存的憑證不正確，您必須取得新的Marketo訂閱。

1. 輸入&#x200B;**Username**、**Password**&#x200B;和Microsoft Dynamics **URL**（客戶端ID和客戶機密碼為可選）。 完成時，按一下「保存」。****

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >Market中的使用者名稱必須符合CRM中同步使用者的使用者名稱。 格式可以是user@domain.com或DOMAIN\user。

## 選擇要同步的欄位{#select-fields-to-sync}

1. 按一下「步驟2:選擇要同步的欄位&#x200B;**。******

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 選取您要同步至Marketo的欄位，以便預先選取這些欄位。 按一下&#x200B;**保存**。

   ![](assets/image2016-8-25-15-3a6-3a11.png)

## 同步自訂篩選器的欄位{#sync-fields-for-a-custom-filter}

如果您已建立自訂篩選，請務必前往並選取要與Marketo同步的新欄位。

1. 前往「管理員」並選取「**Microsoft Dynamics**」。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下欄位同步詳細資訊上的&#x200B;**編輯**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並加以檢查。 實際名稱必須是new_synctomkto，但「顯示名稱」可以是任何內容。 按一下&#x200B;**保存**。

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 啟用同步{#enable-sync}

1. 按一下&#x200B;**步驟3中的**&#x200B;編輯&#x200B;**:啟用Sync**。

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不會針對Microsoft Dynamics同步或當您手動輸入人員或潛在客戶時自動消除重複資料。

1. 閱讀快顯視窗中的所有內容，輸入您的電子郵件地址，然後按一下「開始同步」**。**

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 第一次同步可能需要幾個小時。 完成後，您會收到電子郵件通知。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

幹得漂亮！
