---
unique-page-id: 2360358
description: 僅限使用者登入SSO - Marketo檔案 — 產品檔案
title: 僅限用戶登錄到SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
source-git-commit: 5dcaf886c488e5e1b7fd1c4caa5f869e70c6fb18
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# 僅限用戶登錄到SSO {#restrict-user-login-to-sso-only}

如果你 [使用SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) 並且要確保用戶無法繞過SSO安全，請按照以下說明操作。

>[!IMPORTANT]
>
>本文不適用於 [Adobe IMS已啟用](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Marketo訂閱。

>[!NOTE]
>
>**需要管理權限**

1. 前往 **管理** 按一下 **登入設定**.

   ![](assets/image2014-9-24-14-3a44-3a40.png)

1. 按一下 **編輯安全設定**.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. 展開進階設定，勾選 **需要SSO**，然後按一下 **儲存**.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!NOTE]
>
>最佳實務是邀請使用者並接受邀請。 _之後_ 接受邀請後，管理員應將邀請設為「需要SSO」。

>[!TIP]
>
>如果您選取 **需要SSO**，您可以排除 [使用者角色](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) 通過檢查 **略過單一登入** 選項。 這可讓使用者正常登入。 例如，管理員使用者可能仍需透過登入畫面登入Marketo。

>[!CAUTION]
>
>新使用者受邀時，會收到邀請電子郵件。 但若 **需要SSO** 選取，則不會收到這些電子郵件，除非這些電子郵件已指派給已設為的角色 **略過單一登入**.

就這樣！ 現在，所有使用者（具有略過單一登入權限的使用者除外）將僅限使用SSO登入。

>[!MORELIKETHIS]
>
>* [將單一登入新增至入口網站](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [使用通用ID登入訂閱](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [邀請Marketo使用者加入兩個具有通用ID的例項](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

