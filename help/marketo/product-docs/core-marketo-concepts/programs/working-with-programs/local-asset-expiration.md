---
description: 本機資產過期 — Marketo檔案 — 產品檔案
title: 本機資產過期
exl-id: 603e3eee-0531-4139-a8f5-279831ad011f
source-git-commit: 10873ee50aca443d481117ed66c90930a1cb4b4b
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# 本機資產過期 {#local-asset-expiration}

設定到期日/時間以取消發佈登錄頁面、停用觸發促銷活動或停止循環批次促銷活動。

## 授予排程資產到期權限 {#grant-schedule-asset-expiration-permission}

您的Marketo角色必須已啟用適當權限，才能排程資產過期時間。

>[!NOTE]
>
>**需要管理權限**

1. 在 [!UICONTROL 管理] 按一下 **[!UICONTROL 使用者與角色]**.

   ![](assets/local-asset-expiration-1.png)

1. 按一下 **[!UICONTROL 角色]** 頁簽，選擇要授予訪問權限的用戶，然後按一下 **[!UICONTROL 編輯角色]**.

   ![](assets/local-asset-expiration-2.png)

1. 在 [!UICONTROL 存取行銷活動]，選取 **[!UICONTROL 排程本機資產的到期時間]** 按一下 **[!UICONTROL 儲存]**.

   ![](assets/local-asset-expiration-3.png)

## 設定到期日 {#set-an-expiration-date}

1. 按一下右鍵所需的程式並選擇 **[!UICONTROL 設定本機資產有效期]**.

   ![](assets/local-asset-expiration-4.png)

1. 檢查您要設定的到期日的資產，然後按一下 **[!UICONTROL 設定過期]**.

   ![](assets/local-asset-expiration-5.png)

1. 選擇到期日。

   ![](assets/local-asset-expiration-6.png)

1. 設定時間。 您必須安排至少15分鐘的時間（別忘了輸入上午/下午）。 按一下 **[!UICONTROL 確認]** 時才能使用。

   ![](assets/local-asset-expiration-7.png)

>[!NOTE]
>
>* 若要編輯現有的到期日，只要檢查資產並按一下 **[!UICONTROL 設定過期]**.
>* 資產一旦過期，就不會再顯示在過期格線上。 格線只會顯示已發佈的登錄頁面、作用中的觸發促銷活動，以及循環的批次促銷活動。
>* 如果資產移至其他程式，則會移除已排程的到期日。


## 移除到期日 {#remove-an-expiration-date}

1. 若要移除到期日，請檢查資產，然後按一下 **[!UICONTROL 移除過期]**.

   ![](assets/local-asset-expiration-8.png)

1. 檢閱受影響的資產，然後按一下 **[!UICONTROL 確認]**.

   ![](assets/local-asset-expiration-9.png)

>[!NOTE]
>
>未來不到15分鐘的到期日無法移除。 若要「移除」過期時間，您必須等待資產過期，然後重新核准或重新啟用。
