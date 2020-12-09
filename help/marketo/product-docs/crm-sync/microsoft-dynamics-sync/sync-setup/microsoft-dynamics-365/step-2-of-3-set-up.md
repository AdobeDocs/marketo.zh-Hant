---
unique-page-id: 3571827
description: 第2步（共3步）-在Dynamics中設定Marketo Sync User - Marketo Docs —— 產品檔案
title: 步驟2（共3步）-在Dynamics中設定Marketo同步使用者
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---


# 步驟2（共3步）:在Dynamics中設定Marketto同步使用者 {#step-of-set-up-marketo-sync-user-in-dynamics}

讓我們先建立使用者帳戶。

>[!PREREQUISITES]
>
>[步驟1（共3步）:安裝Marketo解決方案（線上）](step-1-of-3-install.md)

## 建立新使用者 {#create-a-new-user}

1. 登入Dynamics。 按一下「設定」圖示，然後選取「 **進階設定」**。

   ![](assets/one.png)

1. 按一下**設定**，然後選取「安 **全性**」。

   ![](assets/two.png)

1. 按一下「 **使用者**」。

   ![](assets/three.png)

1. 按一下 **新增。**

   ![](assets/four.png)

1. 在新 **視窗中按一下「新增及授權使用者** 」。

   ![](assets/five.png)

1. 隨即開啟新的標籤。 按一 **下頁面頂** 端的「管理員」。

   ![](assets/six.png)

1. 另一個新標籤隨即開啟。 按一 **下新增使用者**。

   ![](assets/seven.png)

1. 輸入您的所有資訊。 完成後，按一下「新 **增」**。

   ![](assets/eight.png)

   >[!NOTE]
   >
   >此名稱必須是專用的同步使用者，而非現有CRM使用者帳戶。 它不需要是實際的電子郵件地址。

1. 輸入要接收新用戶憑據的電子郵件，然後按一下「 **發送電子郵件並關閉**」。

   ![](assets/nine.png)

## 指派同步使用者角色 {#assign-sync-user-role}

將「Marketo同步使用者」角色僅指派給「Marketto同步使用者」。 您不需要將它指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo 4.0.0.14版及更新版本。 對於舊版，所有使用者都必須具有同步使用者角色。 若要升級Marketo，請參 [閱Upgrade Marketo Solution for Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md)。

1. 返回「啟用的用戶」頁籤並刷新用戶清單。

   ![](assets/ten.png)

1. 將滑鼠指標暫留在新建立的Marketo Sync使用者旁，就會出現核取方塊。 按一下以選取它。

   ![](assets/eleven.png)

1. 按一下 **管理角色**。

   ![](assets/twelve.png)

1. 勾選「 **Marketto同步使用者」** ，然後按一 **下「確定」**。

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >同步使用者在您的CRM中進行的任何更新都 **不會** 同步回Marketo。

## 設定Marketo解決方案 {#configure-marketo-solution}

快到了！ 我們只剩下通知Marketo Solution有關新使用者建立的資訊。

1. 返回「進階設定」區段，然後按一下「設 ![](assets/image2015-5-13-15-3a49-3a19.png)定」旁的圖示，並選取「行 **銷人員設定」**。

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果您在「設定」功能表 **中未看到Marketo Config** ，請重新整理頁面。 如果無法運作，請嘗試 [再次發佈Marketo Solution](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations)[](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) ，或登出並重新登入。

1. 按一下 **預設**。

   ![](assets/fifteen.png)

1. 按一下「Marketto使用者」欄位上 **的搜尋按鈕** ，並選取您建立的同步使用者。

   ![](assets/sixteen.png)

1. 按一 ![](assets/image2015-3-13-15-3a10-3a11.png)下右下角的圖示以儲存變更。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 按一 **下右** 上方的X以關閉畫面。

   ![](assets/seventeen.png)

1. 按一下「 ![](assets/image2015-5-13-15-3a49-3a19-1.png)設定」旁的圖示，然後選取「解決 **方案」**。

   ![](assets/eighteen.png)

1. 按一下「 **發佈所有自訂** 」按鈕。

   ![](assets/nineteen.png)

## 繼續步驟3之前 {#before-proceeding-to-step}

    *如果您想要限制同步的記錄數，請立即[設定自訂同步篩選](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
    *執行[驗證Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)程式。 它會驗證您的初始設定是否正確完成。
    *在Microsoft Dynamics CRM中登入Marketo同步使用者。

>[!NOTE]
>
>**相關文章**
>
>
>[步驟3（共3步）:將Microsoft Dynamics與Marketo連結（線上）](step-3-of-3-connect.md)
