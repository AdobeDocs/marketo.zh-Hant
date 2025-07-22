---
unique-page-id: 7516639
description: 授予使用者簽到應用程式的存取權 — Marketo檔案 — 產品檔案
title: 授予使用者存取「簽入」應用程式的許可權
exl-id: 898ac49f-a708-4cdf-b341-58582740a45b
feature: Mobile Marketing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# 授予使用者存取「簽入」應用程式的許可權 {#grant-users-access-to-the-check-in-app}

Marketo Engage對事件簽入應用程式具有特殊使用者角色。 以下說明如何建立具有使用應用程式許可權的新角色。

>[!IMPORTANT]
>
>2023年10月2日，Adobe從所有應用程式商店移除Marketo事件應用程式。 如果您的平板電腦/行動裝置上已安裝應用程式，目前可繼續使用。 一旦您的Marketo Engage執行個體移轉至Adobe Identity以驗證Marketo，您將無法再存取應用程式。 [了解更多](https://nation.marketo.com/t5/product-discussions/marketo-events-app-and-marketo-moments-app-end-of-life/m-p/340712/highlight/true#M193869){target="_blank"}。

## 為行動裝置建立新的使用者角色 {#create-a-new-user-role-for-mobile}

1. 按一下「**[!UICONTROL Admin]**」。

   ![](assets/image2015-6-2-10-3a39-3a31.png)

1. 按一下「**[!UICONTROL Users & Roles]**」。

   ![](assets/image2015-6-2-10-3a56-3a0.png)

1. 按一下&#x200B;**[!UICONTROL Roles]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL New Role]**。

   ![](assets/image2015-6-2-11-3a3-3a23.png)

1. 輸入新角色的名稱和可選的說明。 核取&#x200B;**[!UICONTROL Access Mobile Application]**&#x200B;方塊並按一下&#x200B;**[!UICONTROL Create]**。

   ![](assets/image2015-6-2-11-3a4-3a58.png)

   邀請人員使用平板電腦應用程式時，新角色已可供指派。

## 邀請新使用者加入簽到應用程式 {#invite-new-users-for-the-check-in-app}

1. 按一下「**[!UICONTROL Users]**」標籤。

   ![](assets/image2015-6-2-11-3a10-3a42.png)

1. 按一下「**[!UICONTROL Invite New User]**」。

   ![](assets/image2015-6-2-11-3a11-3a32.png)

1. 輸入新使用者的資訊。 勾選所有適當角色的核取方塊，然後選取具有存取行動應用程式許可權的新角色。 完成時，按一下「**[!UICONTROL Invite]**」。

   ![](assets/image2015-6-2-11-3a16-3a26.png)

   >[!CAUTION]
   >
   >沒有資料庫存取許可權的使用者無法在應用程式中看到任何使用者。

   >[!TIP]
   >
   >針對現有使用者，您可以建立新角色，或將[!UICONTROL Access Mobile Application]許可權新增至目前角色。

使用者會收到電子郵件，告知他們可存取簽入應用程式。
