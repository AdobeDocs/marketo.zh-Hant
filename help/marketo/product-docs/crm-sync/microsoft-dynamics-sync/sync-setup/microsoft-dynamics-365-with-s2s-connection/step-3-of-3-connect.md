---
unique-page-id: 3571830
description: 第3步（共3步） — 將Marketo解決方案與S2S連線連線 — Marketo檔案 — 產品檔案
title: 第3步（共3步） — 使用S2S連線連接Marketo解決方案
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
source-git-commit: 8b4d86f2dd5f19abb56451403cd2638b1a852d79
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# 第3步（共3步）:將Marketo解決方案與S2S連線連線 {#step-3-of-3-connect-microsoft-dynamics-with-marketo-solution-s2s}

這是同步的最後一步。 快到了！

>[!PREREQUISITES]
>
>* [第1步（共3步）:安裝具S2S連線的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)
>* [第2步（共3步）:使用S2S連線設定Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)


>[!NOTE]
>
>**需要管理權限**

## 輸入Dynamics同步用戶資訊 {#enter-dynamics-sync-user-information}

1. 登入Marketo，按一下 **管理**.

   ![](assets/login-admin.png)

1. 按一下 **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 選擇 **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. 按一下 **編輯** in **步驟1:輸入憑據**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >請確定您的憑證正確，因為提交後，我們無法還原後續的架構變更。 如果儲存的憑證不正確，您必須取得新的Marketo訂閱。

1. 輸入 **使用者名稱**, **密碼**，和Microsoft Dynamics **URL**. 按一下 **儲存** 時才能使用。

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >* 如果您的Marketo是在2020年10月之前布建，用戶端ID和密碼為選用欄位。 否則，它們是強制性的。 獲取此資訊取決於您使用的MSD版本。
   >* Marketo中的使用者名稱必須符合CRM中同步使用者的使用者名稱。 格式可為 `user@domain.com` 或域\用戶。
   >* 如果您不知道URL, [在這裡了解如何找到](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## 選擇要同步的欄位 {#select-fields-to-sync}

1. 按一下 **編輯** in **步驟2:選擇要同步的欄位**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 選取您要同步至Marketo的欄位，以便預先選取這些欄位。 按一下 **儲存**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo會儲存要同步之欄位的參考。 如果您刪除Dynamics中的欄位，建議您使用 [已禁用同步](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). 然後編輯並儲存Marketo中的結構，以重新整理 [選擇要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## 同步自訂篩選器的欄位 {#sync-fields-for-a-custom-filter}

如果您已建立自訂篩選器，請務必前往並選取要與Marketo同步的新欄位。

1. 前往「管理」並選取 **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下 **編輯** 在欄位同步詳細資訊上。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並加以檢查。 實際名稱必須為new_synctomkto，但「顯示名稱」可以是任何值。 按一下 **儲存**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 啟用同步 {#enable-sync}

1. 按一下 **編輯** in **步驟3:啟用同步**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不會針對Microsoft Dynamics同步或當您手動輸入人員或銷售機會時自動消除重複資料。

1. 閱讀快顯視窗中的所有內容，輸入您的電子郵件地址，然後按一下 **開始同步**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 第一次同步可能需要數小時。 完成後，您會收到電子郵件通知。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

幹得好！
