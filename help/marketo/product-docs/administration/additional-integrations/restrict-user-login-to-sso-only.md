---
unique-page-id: 2360358
description: 將使用者登入限製為僅限SSO - Marketo檔案 — 產品檔案
title: 限制使用者只可透過 SSO 登入
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 8%

---

# 限制使用者只可透過 SSO 登入 {#restrict-user-login-to-sso-only}

如果您正在[使用SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)，並且想要確保使用者無法略過SSO安全性，請遵循這些指示。

>[!IMPORTANT]
>
>本文不適用於[已啟用IMS的Adobe &#x200B;](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Marketo訂閱。

>[!NOTE]
>
>**需要管理員許可權**

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. 按一下「**[!UICONTROL Login Settings]**」。

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. 按一下「**[!UICONTROL Edit Security Settings]**」。

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. 展開&#x200B;**[!UICONTROL Advanced]**&#x200B;設定，核取&#x200B;**[!UICONTROL Require SSO]**，然後按一下&#x200B;**[!UICONTROL Save]**。

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>最佳實務建議邀請使用者並接受邀請。 _在_&#x200B;接受邀請後，管理員應將邀請設為&quot;[!UICONTROL Require SSO]&quot;。

>[!TIP]
>
>若您選取&#x200B;**[!UICONTROL Require SSO]**，則可在設定角色時勾選[選項，將](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md)使用者角色&#x200B;**[!UICONTROL Bypass Single Sign-On]**&#x200B;從此限制中排除。 這可讓使用者正常登入。 例如，管理員使用者可能仍需要透過登入畫面登入Marketo。 如果SSO和通用ID皆已啟用，您必須設定「略過單一登入」許可權以在訂閱之間切換。

>[!CAUTION]
>
>邀請新使用者時，他們會收到邀請電子郵件。 但是，如果選取&#x200B;**[!UICONTROL Require SSO]**，除非指派給設定為&#x200B;**[!UICONTROL Bypass Single Sign-On]**&#x200B;的角色，否則不會收到這些電子郵件。

完成了！現在，所有使用者（具有略過單一登入許可權的使用者除外）將限製為僅使用SSO登入。

>[!MORELIKETHIS]
>
>* [新增單一登入至入口網站](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [使用通用識別碼進行訂閱登入](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [邀請Marketo使用者使用兩個具有通用ID的執行個體](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
