---
unique-page-id: 10100311
description: 使用通用ID登入訂閱 — Marketo檔案 — 產品檔案
title: 使用通用ID登入訂閱
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
source-git-commit: 591279dfb573853eb8781d7984c65716804120b0
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 使用通用ID登入訂閱 {#using-a-universal-id-for-subscription-login}

通用ID可讓您透過單一登入存取多個Marketo訂閱，並快速在訂閱之間切換。 不過，您也可以視需要為訂閱使用不同的登入。

有了通用ID，您仍會為每個個別訂閱建立支援票證。

使用通用ID的使用者（例如角色、權限和密碼原則）會採用訂閱層級設定。 使用者設定檔層級的變更會反映在所有訂閱中，例如名字、姓氏和電子郵件地址。

## 設定通用ID {#setting-up-a-universal-id}

您的Marketo管理員必須透過相同登入，邀請您加入每個不同的訂閱。 Marketo無法自動合併現有的登入。 啟用通用ID後，您的Marketo執行個體將最多30分鐘無法使用&#x200B;**。**&#x200B;如果您的使用者群較大，則可能會比較長。

>[!NOTE]
>
>如果您有多個訂閱登入ID，則可能還有多個社群設定檔。 請務必為您的通用ID選擇與您要使用之設定檔連線的ID，而這是用於生產執行個體，而非沙箱。

## 登入 {#logging-in}

當您使用通用ID登入以接受第二個訂閱的邀請時，將會看到選擇加入登入頁面。 您必須勾選核取方塊才能接受條款與條件。 接受後，您會看到任何後續登入的一般重設頁面，而非此頁面。 接受條款與條件後，您便可讓Marketo將您的基本設定檔資料（例如名字、姓氏和電子郵件地址）分發至托管訂閱之不同位置的資料中心。

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>除非訂閱管理員刪除，否則您不再使用的ID會保留。 建議您保留這些ID，以防萬一您有指派給自己的私人報表，而該報表僅能透過該ID存取。 在此情況下，將這些私人報表移至新的通用ID，然後刪除您現有的ID是可行的。

## 密碼 {#passwords}

透過適用於多個訂閱的通用ID,Marketo會自動強制執行最嚴格的密碼政策。 例如，如果某些訂閱需要最小密碼長度，而其他訂閱不需要，則所有訂閱將會強制執行最小密碼長度。

使用適用於多個訂閱的通用ID時，只有您可以變更密碼。

>[!NOTE]
>
>如果目前訂閱的密碼不符合第二個訂閱的密碼原則，Marketo會要求想要使用通用ID重設密碼的使用者。

## 在訂閱之間切換 {#switching-between-subscriptions}

使用通用ID，您可以查看您登入的訂閱，並選取您有登入存取權的其他訂閱。 在大多數情況下，您可以在兩者之間切換，而無須登出再登入。

![](assets/image2016-11-3-15-3a10-3a16.png)

當您登出再重新登入時，Marketo會自動將您登入您上次登入的訂閱。 然後，您可以視需要切換至不同的訂閱。

## 社群設定檔 {#community-profiles}

如果您有多個訂閱，則可能有多個社群設定檔。 建議您選擇與您最活躍的社群設定檔連結的登入。

## 行動平台 {#mobile-platform}

具有通用ID的使用者可從上次登入的訂閱，在Marketo時刻和iPad事件簽入應用程式中查看其資料。 您無法從行動平台本身變更訂閱。

>[!MORELIKETHIS]
>
>* [將單一登入新增至入口網站](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [僅限用戶登錄到SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [邀請Marketo使用者加入兩個具有通用ID的例項](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

