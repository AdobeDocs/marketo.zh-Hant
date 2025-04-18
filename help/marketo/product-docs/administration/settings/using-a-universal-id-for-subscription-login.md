---
unique-page-id: 10100311
description: 使用通用ID進行訂閱登入 — Marketo檔案 — 產品檔案
title: 使用通用ID進行訂閱登入
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
feature: Administration
source-git-commit: 5a8ea3c5356cb370b4e502b23eea8a457bfc97f1
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# 使用通用ID進行訂閱登入 {#using-a-universal-id-for-subscription-login}

通用ID可讓您透過單一登入存取多個Marketo訂閱，並在訂閱之間快速切換。 不過，您可以視需求對訂閱使用不同的登入。

使用通用ID，您仍可為每個個別訂閱建立支援票證。

使用通用ID的使用者（例如角色、許可權和密碼原則）會遵循訂閱層級設定。 使用者設定檔層級變更會反映在所有訂閱中，例如名字、姓氏和電子郵件地址。

## 設定通用ID {#setting-up-a-universal-id}

所有Marketo訂閱都隨附選用的通用ID功能。 在每個個別執行個體中，您的Marketo管理員必須使用相同的登入邀請您加入每個不同的訂閱。 Marketo無法自動合併您現有的登入。

>[!NOTE]
>
>如果您有多個訂閱登入ID，您也可能有多個社群設定檔。 請務必選擇通用ID的ID，此通用ID已連線至您要使用的設定檔，而且適用於您的生產執行個體，而非您的沙箱。

## 登入 {#logging-in}

當您使用通用ID登入以接受第二個訂閱的邀請時，您會看到選擇加入登入頁面。 您必須勾選核取方塊以接受條款與條件。 接受後，您將會看到後續登入的正常重設頁面，而非此頁面。 接受條款與條件後，您就可以讓Marketo將基本設定檔資料（例如名字、姓氏及電子郵件地址）發佈至託管訂閱的不同位置資料中心。

![](assets/using-a-universal-id-for-subscription-login-1.png)

>[!TIP]
>
>您不再使用的ID會保留，除非訂閱管理員將其刪除。 建議您保留這些資料，以防（舉例來說）您擁有指派給自己的私人報告，但僅可使用該ID存取。 在此情況下，將這些私人報表移至新的通用ID，然後刪除現有的ID是可行的做法。

## 密碼 {#passwords}

透過適用於多個訂閱的通用ID，Marketo會自動實施最嚴格的密碼政策。 例如，如果某些訂閱需要最小密碼長度，而其他訂閱則不需要，則所有訂閱都將強制使用最小長度。

使用適用於多個訂閱的通用ID，只有您可以變更密碼。

>[!NOTE]
>
>如果目前的訂閱密碼不符合邀請他們使用的第二個訂閱的密碼原則，Marketo會要求想要使用通用ID的使用者重設密碼。

## 在訂閱之間切換 {#switching-between-subscriptions}

使用通用ID，您可以檢視已登入的訂閱，並選取您有登入存取權的其他訂閱。 在大多數情況下，您無需登出再重新登入，即可在兩者之間切換。

如果[單一登入](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)和通用ID皆已啟用，您必須設定「略過單一登入」許可權才能在訂閱之間切換。

![](assets/using-a-universal-id-for-subscription-login-2.png)

當您登出再登入時，Marketo會自動將您登入上次登入的訂閱。 如有必要，您可以切換至其他訂閱。

## 社群設定檔 {#community-profiles}

如果您有多個訂閱，則可能有多個社群設定檔。 建議您選擇連結至最活躍社群設定檔的登入。

>[!MORELIKETHIS]
>
>* [新增單一登入至入口網站](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md){target="_blank"}
>* [僅將使用者登入限製為SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [邀請Marketo使用者使用兩個具有通用ID的執行個體](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}
