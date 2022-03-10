---
unique-page-id: 2360358
description: 限制用戶僅登錄SSO -Marketo文檔 — 產品文檔
title: 僅限用戶登錄SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
source-git-commit: a21db1586166b7530bbbb18759752ef834cdc46a
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# 僅限用戶登錄SSO {#restrict-user-login-to-sso-only}

如果你 [使用SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) 並希望確保用戶無法繞過SSO安全，請按照以下說明操作。

>[!IMPORTANT]
>
>本文不適用於 [啟用Adobe IMS](/help/marketo/product-docs/administration/marketo-with-adobe-identity/overview.md) Marketo訂閱。

>[!NOTE]
>
>**需要管理權限**

1. 轉到 **管理** 按一下 **登錄設定**。

   ![](assets/image2014-9-24-14-3a44-3a40.png)

1. 按一下 **編輯安全設定**。

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. 展開「高級」設定，選中 **需要SSO**，然後按一下 **保存**。

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!NOTE]
>
>最佳做法是邀請用戶並接受邀請。 _之後_ 接受邀請後，管理員應將其設定為「需要SSO」。

>[!TIP]
>
>如果選擇 **需要SSO**，您可以 [用戶角色](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) 通過檢查 **繞過單一登錄** 的子菜單。 這將允許用戶正常登錄。 例如，管理員用戶可能仍需要通過登錄螢幕登錄Marketo。

>[!CAUTION]
>
>當新用戶被邀請時，他們會收到邀請電子郵件。 但是，如果 **需要SSO** 選中，除非將這些電子郵件分配給設定為的角色，否則它們將不會接收這些電子郵件 **繞過單一登錄**。

就這樣！ 現在，所有用戶（除了具有繞過單一登錄權限的用戶）將僅限於使用SSO登錄。

>[!MORELIKETHIS]
>
>* [將單一登錄添加到門戶](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [使用通用ID進行訂閱登錄](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [邀請Marketo用戶訪問兩個具有通用ID的實例](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

