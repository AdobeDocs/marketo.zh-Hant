---
unique-page-id: 3571827
description: 第2步（共3步）-在Dynamics中設定Marketo Sync User - Marketo Docs —— 產品檔案
title: 步驟2（共3步）-在Dynamics中設定Marketo同步使用者
translation-type: tm+mt
source-git-commit: 9d8a6d9880de5d2af211906c2410f2057c1f454d
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---


# 步驟2（共3步）:在Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}中設定Marketo同步使用者

讓我們先建立使用者帳戶。

>[!PREREQUISITES]
>
>[步驟1（共3步）:安裝Marketo解決方案（線上）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)

## 建立新用戶{#create-a-new-user}

1. 登入Dynamics。 按一下「設定」圖示，然後選取「**進階設定」**。

   ![](assets/one.png)

1. 按一下&#x200B;**Settings**&#x200B;並選擇&#x200B;**Security**。

   ![](assets/two.png)

1. 按一下&#x200B;**用戶**。

   ![](assets/three.png)

1. 按一下&#x200B;**新建。**

   ![](assets/four.png)

1. 在新視窗中按一下「新增及授權使用者」。****

   ![](assets/five.png)

1. 隨即開啟新的標籤。 按一下頁面頂端的&#x200B;**管理**。

   ![](assets/six.png)

1. 另一個新標籤隨即開啟。 按一下&#x200B;**添加用戶**。

   ![](assets/seven.png)

1. 輸入您的所有資訊。 完成後，按一下&#x200B;**添加**。

   ![](assets/eight.png)

   >[!NOTE]
   >
   >此名稱必須是專用的同步使用者，而非現有CRM使用者帳戶。 它不需要是實際的電子郵件地址。

1. 輸入要接收新用戶憑據的電子郵件，然後按一下&#x200B;**發送電子郵件並關閉**。

   ![](assets/nine.png)

## 分配同步用戶角色{#assign-sync-user-role}

將「Marketo同步使用者」角色僅指派給「Marketto同步使用者」。 您不需要將它指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo 4.0.0.14版及更新版本。 對於舊版，所有使用者都必須具有同步使用者角色。 若要升級Marketo，請參閱[Upgrade Marketo Solution for Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)。

1. 返回「啟用的用戶」頁籤並刷新用戶清單。

   ![](assets/ten.png)

1. 將滑鼠指標暫留在新建立的Marketo Sync使用者旁，就會出現核取方塊。 按一下以選取它。

   ![](assets/eleven.png)

1. 按一下&#x200B;**管理角色**。

   ![](assets/twelve.png)

1. 勾選「**Marketo Sync User**」，然後按一下「確定&#x200B;**OK**」。

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >同步使用者在您的CRM中進行的任何更新，都會將&#x200B;**not**&#x200B;同步回行銷人員。

## 設定Marketo解決方案{#configure-marketo-solution}

快到了！ 我們只剩下通知Marketo Solution有關新使用者建立的資訊。

1. 返回「進階設定」區段，然後按一下「設定」旁的![](assets/image2015-5-13-15-3a49-3a19.png)圖示，然後選取「行銷人員設定」**。**

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果您在「設定」功能表中未看到「行銷人員設定」，請重新整理頁面。 ****&#x200B;如果無法運作，請嘗試再次[發佈Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)，或登出並重新登入。

1. 按一下&#x200B;**Default**。

   ![](assets/fifteen.png)

1. 按一下&#x200B;**Marketo User**&#x200B;欄位上的搜尋按鈕，並選取您建立的同步使用者。

   ![](assets/sixteen.png)

1. 按一下右下角的![](assets/image2015-3-13-15-3a10-3a11.png)圖示以儲存變更。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 按一下右上方的&#x200B;**X**&#x200B;以關閉畫面。

   ![](assets/seventeen.png)

1. 按一下「設定」旁的![](assets/image2015-5-13-15-3a49-3a19-1.png)圖示，然後選取「解決方案」**。**

   ![](assets/eighteen.png)

1. 按一下&#x200B;**「發佈所有自定義」**&#x200B;按鈕。

   ![](assets/nineteen.png)

## 繼續執行步驟3 {#before-proceeding-to-step}之前

    *如果您想要限制同步的記錄數，請立即[設定自訂同步篩選](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
    *執行[驗證Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)程式。它會驗證您的初始設定是否正確完成。
    *在Microsoft Dynamics CRM中登入Marketo同步使用者。

>[!MORELIKETHIS]
>
>[步驟3（共3步）:將Microsoft Dynamics與Marketo連結（線上）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md)
