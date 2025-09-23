---
description: 本機資產有效期 — Marketo檔案 — 產品檔案
title: 本地資產期限
exl-id: 603e3eee-0531-4139-a8f5-279831ad011f
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 4%

---

# 本地資產期限 {#local-asset-expiration}

設定到期日/時間，以取消發佈登陸頁面、停用觸發行銷活動或停止循環的批次行銷活動。

## 授予排程資產到期許可權 {#grant-schedule-asset-expiration-permission}

在排程資產到期之前，您的Marketo角色必須已啟用適當許可權。

>[!NOTE]
>
>**需要管理員許可權**

1. 在[!UICONTROL Admin]區域中，按一下&#x200B;**[!UICONTROL Users & Roles]**。

   ![](assets/local-asset-expiration-1.png)

1. 按一下&#x200B;**[!UICONTROL Roles]**&#x200B;標籤，選取您要授與存取許可權的使用者，然後按一下&#x200B;**[!UICONTROL Edit Role]**。

   ![](assets/local-asset-expiration-2.png)

1. 在「[!UICONTROL Access Marketing Activities]」之下，選取「**[!UICONTROL Schedule Local Asset Expiration]**」，然後按一下「**[!UICONTROL Save]**」。

   ![](assets/local-asset-expiration-3.png)

## 設定到期日 {#set-an-expiration-date}

1. 用滑鼠右鍵按一下所需的程式，然後選取&#x200B;**[!UICONTROL Set local asset expiration]**。

   ![](assets/local-asset-expiration-4.png)

1. 檢查您要設定到期日的資產，然後按一下&#x200B;**[!UICONTROL Set expiration]**。

   ![](assets/local-asset-expiration-5.png)

1. 選擇到期日。

   ![](assets/local-asset-expiration-6.png)

1. 設定時間。 您必須排程未來至少15分鐘的時間（別忘了輸入上午/下午）。 完成時，按一下&#x200B;**[!UICONTROL Confirm]**。

   ![](assets/local-asset-expiration-7.png)

>[!NOTE]
>
>* 若要編輯現有的到期日，只要檢查資產並按一下&#x200B;**[!UICONTROL Set expiration]**&#x200B;即可。
>* 資產一旦過期，就不會再出現在「過期」格線上。 網格只會顯示已發佈的登陸頁面、作用中的觸發行銷活動，以及循環的批次行銷活動。
>* 如果資產移至其他方案，則會移除已排程的過期時間。

## 移除到期日 {#remove-an-expiration-date}

1. 若要移除到期日，請檢查資產並按一下&#x200B;**[!UICONTROL Remove expiration]**。

   ![](assets/local-asset-expiration-8.png)

1. 檢閱受影響的資產，然後按一下&#x200B;**[!UICONTROL Confirm]**。

   ![](assets/local-asset-expiration-9.png)

>[!NOTE]
>
>無法移除未來15分鐘內的到期日。 若要「移除」到期日，您需要等待資產到期，然後重新核准或重新啟用資產。
