---
description: 第2步（共4步） — 使用資源所有者密碼控制連接設定Marketo解決方案 — Marketo文檔 — 產品文檔
title: 第2步（共4步） — 設定具有資源所有者密碼控制連接的Marketo解決方案
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
source-git-commit: 19c568cdc3d31d07e42e99eb7e48f10a017b44f9
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# 第2步（共4步）:設定具有資源所有者密碼控制連接的Marketo解決方案 {#step-2-of-4-set-up-the-marketo-solution-ropc}

讓我們通過建立用戶帳戶開始。

>[!PREREQUISITES]
>
>[第1步（共4步）:安裝具有資源所有者密碼控制連接的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)

## 建立新用戶 {#create-a-new-user}

1. 登錄到Dynamics。 按一下「設定」表徵圖，然後選擇 **高級設定**。

   ![](assets/one.png)

1. 按一下 **設定** 選擇 **安全**。

   ![](assets/two.png)

1. 按一下 **用戶**。

   ![](assets/three.png)

1. 按一下 **新建。**

   ![](assets/four.png)

1. 按一下 **添加和許可用戶** 的上界。

   ![](assets/five.png)

1. 將開啟一個新頁籤。 按一下 **管理** 頁面頂部。

   ![](assets/six.png)

1. 將開啟另一個新頁籤。 按一下 **添加用戶**。

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >同步用戶應具有對Marketo配置的讀取權限。

1. 輸入所有資訊。 完成後，按一下 **添加**。

   ![](assets/eight.png)

   >[!NOTE]
   >
   >此名稱必須是專用的同步用戶，而不是現有的CRM用戶帳戶。 它不必是實際的電子郵件地址。

1. 輸入要接收新用戶憑據的電子郵件，然後按一下 **發送電子郵件並關閉**。

   ![](assets/nine.png)

## 分配同步用戶角色 {#assign-sync-user-role}

將「Marketo同步用戶」角色僅分配給「Marketo同步」用戶。 您不需要將其分配給任何其他用戶。

>[!NOTE]
>
>這適用於Marketo4.0.0.14版及更高版本。 對於早期版本，所有用戶必須具有同步用戶角色。 要升級Marketo，請參閱 [升級MarketoMicrosoft動力解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)。

>[!IMPORTANT]
>
>同步用戶的語言設定 [應設定為英語](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)。

1. 返回「已啟用的用戶」頁籤並刷新用戶清單。

   ![](assets/ten.png)

1. 將滑鼠懸停在新建立的Marketo同步用戶旁邊，將出現一個複選框。 按一下以選擇它。

   ![](assets/eleven.png)

1. 按一下 **管理角色**。

   ![](assets/twelve.png)

1. 檢查 **Marketo同步用戶** 按一下 **確定**。

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >同步用戶在您的CRM中所做的任何更新將 **不** 同步回Marketo。

## 配置Marketo解決方案 {#configure-marketo-solution}

快到了！ 我們只剩下了通知Marketo解決方案部門有關新用戶建立的資訊。

1. 返回「高級設定」部分，然後按一下 ![](assets/image2015-5-13-15-3a49-3a19.png) 表徵圖，然後選擇 **Marketo配置**。

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果你看不到 **Marketo配置** 在「設定」菜單中，刷新頁面。 如果這行不通，盡量 [發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) 或註銷並重新登錄。

1. 按一下 **預設**。

   ![](assets/fifteen.png)

1. 按一下 **Marketo用戶** 欄位，然後選擇您建立的同步用戶。

   ![](assets/sixteen.png)

1. 按一下 ![](assets/image2015-3-13-15-3a10-3a11.png) 按鈕，將選定控制項在Tab鍵次序中下移一個位置。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 按一下 **X** 的上界。

   ![](assets/seventeen.png)

1. 按一下 ![](assets/image2015-5-13-15-3a49-3a19-1.png) 表徵圖，然後選擇 **解決方案**。

   ![](assets/eighteen.png)

1. 按一下 **發佈所有自定義項** 按鈕

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[第3步（共4步）:將Marketo解決方案與資源所有者密碼控制連接連接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)
