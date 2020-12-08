---
unique-page-id: 2360358
description: 僅限使用者登入SSO —— 行銷人員檔案——產品檔案
title: 僅限使用者登入SSO
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# 僅限使用者登入SSO {#restrict-user-login-to-sso-only}

如果您使用 [SSO](add-single-sign-on-to-a-portal.md) ，但想要確保使用者無法略過SSO安全性，請依照下列指示進行。

>[!NOTE]
>
>**需要管理員權限**

1. 前往「管理員」並按一下「登入設定」。

![](assets/image2014-9-24-14-3a44-3a40.png)

1. 按一下「編輯保全設定」。

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. 展開進階設定，勾選「需要SSO」，然後按一下「儲存」。

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!TIP]
>
>如果您選 **取「需要SSO**」，則可以在設定角色時核取「略過單一登入 [](../../../product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md)**** 」選項，從此限制中排除使用者角色。 這可讓使用者正常登入。 例如，管理員使用者可能仍需透過登入畫面登入Marketo。

>[!CAUTION]
>
>當新使用者受到邀請時，他們會收到邀請電子郵件。 不過，如果 **選取「需要SSO** 」，則不會收到這些電子郵件，除非他們已指派至設定為「略過單一登入」的 **角色**。

就這樣！ 現在，所有使用者（具有略過單一登入權限的使用者除外）將僅限使用SSO登入。