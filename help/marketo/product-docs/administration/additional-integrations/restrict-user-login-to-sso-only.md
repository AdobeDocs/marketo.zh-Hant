---
unique-page-id: 2360358
description: 僅限使用者登入SSO —— 行銷人員檔案——產品檔案
title: 僅限使用者登入SSO
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# 僅限SSO用戶登錄{#restrict-user-login-to-sso-only}

如果您[使用SSO](add-single-sign-on-to-a-portal.md)，並想要確保使用者無法略過SSO安全性，請依照下列指示進行。

>[!NOTE]
>
>**需要管理員權限**

1. 前往&#x200B;**Admin**，然後按一下「登入設定」。****

![](assets/image2014-9-24-14-3a44-3a40.png)

1. 按一下&#x200B;**編輯安全設定**。

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. 展開「Advanced settings（高級設定）」 ，選中「Require SSO（需要SSO）」 ，然後按一下「Save（保存）」。********

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!TIP]
>
>如果選擇&#x200B;**要求SSO**，則可以通過選中&#x200B;**在設定角色時繞過單一登錄**&#x200B;選項，從此限制中排除[用戶角色](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md)。 這可讓使用者正常登入。 例如，管理員使用者可能仍需透過登入畫面登入Marketo。

>[!CAUTION]
>
>當新使用者受到邀請時，他們會收到邀請電子郵件。 不過，如果選取「需要SSO」(**Require SSO**)，則不會收到這些電子郵件，除非他們已指派至設定為「略過單一登入」(Bypass Single Sign-On)的角色。****

就這樣！ 現在，所有使用者（具有略過單一登入權限的使用者除外）將僅限使用SSO登入。
