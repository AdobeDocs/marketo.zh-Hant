---
description: 本機資產有效期 — Marketo檔案 — 產品檔案
title: 本機資產有效期
exl-id: 603e3eee-0531-4139-a8f5-279831ad011f
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# 本機資產有效期 {#local-asset-expiration}

設定到期日/時間，以取消發佈登入頁面、停用觸發程式行銷活動，或停止循環的批次行銷活動。

## 授予排程資產到期許可權 {#grant-schedule-asset-expiration-permission}

在排程資產到期之前，您的Marketo角色必須啟用適當的許可權。

>[!NOTE]
>
>**需要管理員許可權**

1. 在 [!UICONTROL 管理員] 區域，按一下 **[!UICONTROL 使用者和角色]**.

   ![](assets/local-asset-expiration-1.png)

1. 按一下 **[!UICONTROL 角色]** 索引標籤中，選取您要授與存取許可權的使用者，然後按一下 **[!UICONTROL 編輯角色]**.

   ![](assets/local-asset-expiration-2.png)

1. 下 [!UICONTROL 存取行銷活動]，選取 **[!UICONTROL 排程本機資產到期日]** 並按一下 **[!UICONTROL 儲存]**.

   ![](assets/local-asset-expiration-3.png)

## 設定到期日 {#set-an-expiration-date}

1. 以滑鼠右鍵按一下所需的程式，然後選取 **[!UICONTROL 設定本機資產有效期]**.

   ![](assets/local-asset-expiration-4.png)

1. 勾選您要設定到期日的資產，然後按一下 **[!UICONTROL 設定有效期]**.

   ![](assets/local-asset-expiration-5.png)

1. 選擇到期日。

   ![](assets/local-asset-expiration-6.png)

1. 設定時間。 您必須排程未來至少15分鐘的時間（別忘了輸入上午/下午）。 按一下 **[!UICONTROL 確認]** 完成時。

   ![](assets/local-asset-expiration-7.png)

>[!NOTE]
>
>* 若要編輯現有到期日，只要檢查資產並按一下 **[!UICONTROL 設定有效期]**.
>* 資產一旦過期，就不會再出現在「過期」格線上。 此網格只會顯示已發佈的登陸頁面、作用中觸發行銷活動，以及循環的批次行銷活動。
>* 如果資產移至其他方案，則會移除已排程的到期日。

## 移除到期日 {#remove-an-expiration-date}

1. 若要移除到期日，請核取資產並按一下 **[!UICONTROL 移除到期日]**.

   ![](assets/local-asset-expiration-8.png)

1. 檢閱受影響的資產，然後按一下 **[!UICONTROL 確認]**.

   ![](assets/local-asset-expiration-9.png)

>[!NOTE]
>
>無法移除未來15分鐘內的到期日。 若要「移除」到期日，您需要等待資產過期，然後重新核准或重新啟用資產。
