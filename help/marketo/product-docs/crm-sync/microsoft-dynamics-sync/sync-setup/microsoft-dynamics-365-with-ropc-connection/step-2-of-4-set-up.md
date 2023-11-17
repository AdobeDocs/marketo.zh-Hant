---
description: 步驟4之2 — 使用資源擁有者密碼控制連線設定Marketo解決方案 — Marketo檔案 — 產品檔案
title: 步驟4之2 — 使用資源擁有者密碼控制連線設定Marketo解決方案
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
feature: Microsoft Dynamics
source-git-commit: 2eb61d43f2f470d42e1b50ab8edc99e4e25c23cf
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# 步驟4之2：使用資源擁有者密碼控制連線設定Marketo解決方案 {#step-2-of-4-set-up-the-marketo-solution-ropc}

讓我們從建立使用者帳戶開始。

>[!PREREQUISITES]
>
>[步驟4之1：安裝具有資源擁有者密碼控制連線的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}

## 建立新使用者 {#create-a-new-user}

1. 登入Dynamics。 按一下「設定」圖示並選取 **[!UICONTROL 進階設定]**.

   ![](assets/one.png)

1. 按一下 **[!UICONTROL 設定]** 並選取 **[!UICONTROL 安全性]**.

   ![](assets/two.png)

1. 按一下 **[!UICONTROL 使用者]**.

   ![](assets/three.png)

1. 按一下 **[!UICONTROL 新增]**.

   ![](assets/four.png)

1. 按一下 **[!UICONTROL 新增並授權使用者]** 在新視窗中。

   ![](assets/five.png)

1. 新標籤隨即開啟。 按一下 **[!UICONTROL 管理員]** ，位於頁面頂端。

   ![](assets/six.png)

1. 另一個新標籤隨即開啟。 按一下 **[!UICONTROL 新增使用者]**.

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >同步使用者應該要有Marketo設定的讀取許可權。

1. 輸入您的所有資訊。 完成後，按一下 **[!UICONTROL 新增]**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >此名稱必須是專用的同步處理使用者，而非現有的CRM使用者帳戶。 它不需要是實際的電子郵件地址。

1. 輸入電子郵件以接收新的使用者認證，然後按一下 **[!UICONTROL 傳送電子郵件並關閉]**.

   ![](assets/nine.png)

## 指派同步使用者角色 {#assign-sync-user-role}

僅將Marketo同步使用者角色指派給Marketo同步使用者。 您不需要將其指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo 4.0.0.14版和更新版本。 對於舊版，所有使用者都必須擁有同步使用者角色。 若要升級Marketo，請參閱 [升級Microsoft Dynamics的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>同步處理使用者的語言設定 [應該設定為英文](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. 返回 **[!UICONTROL 啟用的使用者]** 標籤並重新整理使用者清單。

   ![](assets/ten.png)

1. 將游標暫留在新建立的Marketo Sync使用者旁，核取方塊隨即出現。 按一下以選取它。

   ![](assets/eleven.png)

1. 按一下 **[!UICONTROL 管理角色]**.

   ![](assets/twelve.png)

1. 檢查 **[!UICONTROL Marketo同步使用者]** 並按一下 **[!UICONTROL 確定]**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >同步使用者在您的CRM中所做的任何更新都將 _非_ 已同步回Marketo。

## 設定Marketo解決方案 {#configure-marketo-solution}

即將完成！ 我們只剩下通知Marketo解決方案有關建立的新使用者。

1. 返回「進階設定」區段，然後按一下 ![](assets/image2015-5-13-15-3a49-3a19.png) 圖示並選取「 」 **[!UICONTROL Marketo設定]**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果您沒有看到 **[!UICONTROL Marketo設定]** 在「設定」功能表中，重新整理頁面。 如果這樣無法解決問題，請嘗試 [發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"} 再次登出並重新登入。

1. 按一下 **[!UICONTROL 預設]**.

   ![](assets/fifteen.png)

1. 按一下 **[!UICONTROL Marketo使用者]** 欄位並選取您建立的同步使用者。

   ![](assets/sixteen.png)

1. 按一下 ![](assets/image2015-3-13-15-3a10-3a11.png) 圖示以儲存變更。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 按一下 **X** 以關閉熒幕。

   ![](assets/seventeen.png)

1. 按一下 ![](assets/image2015-5-13-15-3a49-3a19-1.png) 圖示並選取「 」 **[!UICONTROL 解決方案]**.

   ![](assets/eighteen.png)

1. 按一下 **[!UICONTROL 發佈所有自訂]** 按鈕。

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[步驟4之3：使用資源擁有者密碼控制連線來連線Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}
