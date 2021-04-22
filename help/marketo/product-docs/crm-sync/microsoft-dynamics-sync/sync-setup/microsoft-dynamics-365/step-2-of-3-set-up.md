---
unique-page-id: 3571827
description: 第2步（共3步）-在Dynamics中設定Marketo同步用戶-Marketo文檔——產品文檔
title: 第2步（共3步）-在Dynamics中設定Marketo同步用戶
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# 步驟2（共3步）:在Dynamics中設定Marketo同步用戶{#step-of-set-up-marketo-sync-user-in-dynamics}

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

將「Marketo同步用戶」角色僅分配給Marketo同步用戶。 您不需要將它指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo4.0.0.14版及更新版本。 對於舊版，所有使用者都必須具有同步使用者角色。 要升級Marketo，請參閱[升級MarketoMicrosoft Dynamics解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)。

1. 返回「啟用的用戶」頁籤並刷新用戶清單。

   ![](assets/ten.png)

1. 將滑鼠指標暫留在新建立的「Marketo同步」使用者旁，就會出現核取方塊。 按一下以選取它。

   ![](assets/eleven.png)

1. 按一下&#x200B;**管理角色**。

   ![](assets/twelve.png)

1. 選中&#x200B;**Marketo同步用戶** ，然後按一下&#x200B;**確定**。

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >同步使用者在您的CRM中進行的任何更新，都會將&#x200B;**not**&#x200B;同步回Marketo。

## 配置Marketo解決方案{#configure-marketo-solution}

快到了！ 我們只剩下了將新使用者建立資訊告知Marketo解決方案。

1. 返回「Advanced Settings（高級設定）」部分，然後按一下「Settings（設定）」旁的![](assets/image2015-5-13-15-3a49-3a19.png)表徵圖，然後選擇「**Marketo配置」。**

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果您在「設定」功能表中未看到「Marketo組態&#x200B;**」，請重新整理頁面。**&#x200B;如果無法運作，請嘗試再次[發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)，或登出並重新登入。

1. 按一下&#x200B;**Default**。

   ![](assets/fifteen.png)

1. 按一下&#x200B;**Marketo用戶**&#x200B;欄位上的搜索按鈕，然後選擇您建立的同步用戶。

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
    *在Microsoft Dynamics CRM中登入「Marketo同步使用者」。

>[!MORELIKETHIS]
>
>[步驟3（共3步）:將Microsoft Dynamics與Marketo（線上）連接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md)
