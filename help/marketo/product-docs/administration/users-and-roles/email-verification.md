---
description: 電子郵件驗證 — Marketo檔案 — 產品檔案
title: 電子郵件驗證
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: 7b64e6e9bbd282b1e27f4c9c862df07642e9a35b
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# 電子郵件驗證 {#email-verification}

Adobe Marketo Engage訂閱需要所有非API的使用者(包括Marketo Engage管理員)驗證其電子郵件地址。

## 為什麼要引入此功能 {#why-this-feature-was-introduced}

Marketo Engage正在繼續推出電子郵件驗證，以準備將客戶移轉至Adobe Business Platform，包括使用者移轉至AdobeID。 此功能可增強現有Marketo Engage使用者帳戶的安全性。 為了確保Marketo Engage使用者與適當的Adobe ID相關聯，現有Marketo Engage使用者必須驗證其電子郵件地址。 Marketo Engage使用者必須擁有經過驗證的電子郵件地址，才能移轉至Adobe ID。 如果Marketo Engage使用者未驗證其電子郵件地址，則無法將他們移轉至Adobe ID，而且當使用者移轉訂閱完成後，將無法存取Marketo訂閱。

## 使用者邀請 {#user-invite}

當管理員邀請使用者時，該使用者在按一下邀請連結後即會自動驗證。

>[!IMPORTANT]
>
>上述的例外情況是&#x200B;_在僅限SSO的訂閱_&#x200B;中，管理員會收到新的使用者邀請，但非管理員使用者則不會。 不是管理員的使用者仍需完成電子郵件驗證程式，以確保移轉其記錄。 使用者可以按一下[設定檔]圖示並移至&#x200B;**我的帳戶** > **帳戶設定**，然後按一下&#x200B;**重新傳送驗證**，以傳送電子郵件驗證連結給自己。

![](assets/email-verification-1.png)

## 驗證電子郵件 {#verification-email}

當為訂閱啟用電子郵件驗證，或由管理員/使用者觸發時，使用者將收到以下電子郵件。

電子郵件驗證成功需要有效的使用者工作階段。 使用者必須先使用身分提供者(IdP) URL登入其Marketo訂閱。 工作階段建立後，他們會&#x200B;_然後_&#x200B;按一下電子郵件中的&#x200B;**驗證電子郵件地址**&#x200B;連結。

![](assets/email-verification-2.png)

>[!TIP]
>
>若要將驗證電子郵件重新傳送給未驗證的使用者，只要選取其記錄並按一下&#x200B;**[!UICONTROL 驗證電子郵件]**&#x200B;按鈕即可。

## 變更電子郵件地址 {#changing-an-email-address}

使用者的電子郵件地址變更後，即會變成未驗證。 他們將會收到電子郵件，以便重新驗證。 使用者可以按一下&#x200B;**[!UICONTROL 重新傳送驗證]**，以手動方式重新傳送該電子郵件。

![](assets/email-verification-3.png)

![](assets/email-verification-4.png)

## 使用者和角色 {#users-and-roles}

在&#x200B;**[!UICONTROL 管理員]** > **[!UICONTROL 使用者與角色]**&#x200B;中，[電子郵件狀態]欄會顯示每個使用者的驗證狀態。

![](assets/email-verification-5.png)

## 多個使用者登入ID {#multiple-user-login-ids}

只有一個使用者帳戶可以與單一電子郵件地址建立關聯。 如果有多個使用者帳戶與單一電子郵件地址關聯，則Marketo Engage需要解決衝突，並顯示與電子郵件地址關聯的所有使用者登入，以及三個解決選項：

* 使用目前的電子郵件作為目前的使用者登入ID
* 使用新電子郵件作為目前的使用者登入ID
* 延遲決定至下次登入

  ![](assets/email-verification-6.png)

>[!NOTE]
>
>雖然使用者帳戶必須與單一地址相關聯，但使用者帳戶可透過通用ID用於許多訂閱。
