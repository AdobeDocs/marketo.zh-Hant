---
unique-page-id: 10100311
description: 使用通用ID進行訂閱登入——行銷檔案——產品檔案
title: 使用通用ID進行訂閱登入
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---


# 使用通用ID進行訂閱登入{#using-a-universal-id-for-subscription-login}

通用ID可讓您透過單一登入存取多個Marketo訂閱，並快速在訂閱之間切換。 不過，您可以視需要為訂閱使用不同的登入。

使用Universal ID，您仍然可以為每個個別訂閱建立支援票證。

使用通用ID的使用者會接受訂閱層級設定，例如角色、權限和密碼原則。 使用者描述檔層級的變更反映在所有訂閱中，例如名字、姓氏和電子郵件地址。

## 設定通用ID {#setting-up-a-universal-id}

您的行銷人員必須從每個個別例項，邀請您使用相同登入方式加入您的每個不同訂閱。 Marketto無法自動合併您現有的登入。 啟用Universal ID後，**您的Marketo例項最多30分鐘將無法使用**。 如果您的使用者群較大，可能會比較長。

>[!CAUTION]
>
>如果為用戶啟用了「單ID」或「通用ID」，則其角色和工作區可以在初始設定後編輯&#x200B;**not**。

>[!NOTE]
>
>如果您有多個訂閱登入ID，您也可能有多個社群設定檔。 請務必為您的通用ID選擇ID，該ID已連接至您要使用的描述檔，這是您的生產執行個體，而非您的沙盒。

## 登入{#logging-in}

當您登入以接受使用通用ID的第二個訂閱邀請時，您會看到「選擇登入」登入頁面。 您必須勾選核取方塊才能接受條款與條件。 在您接受後，您將會看到任何後續登入的正常重設頁面，而非此頁面。 接受條款與條件後，即可讓Marketer將您的基本個人檔案資料（例如名字、姓氏和電子郵件地址）散發至您托管訂閱之不同位置的資料中心。

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>除非訂閱管理員刪除您不再使用的ID，否則會保留。 我們建議您保留這些報表，以防萬一您有指派給自己的私人報表，而且只能使用該ID加以存取。 在這種情況下，將這些私人報表移至新的通用ID，然後刪除您現有的ID是有意義的。

## 密碼{#passwords}

使用適用於多個訂閱的通用ID,Marketo會自動實施最嚴格的密碼政策。 例如，如果某些訂閱需要最小密碼長度，而其他訂閱則不需要，則所有訂閱都會強制執行最小長度。

使用適用於多個訂閱的通用ID時，只有您可以變更密碼。

>[!NOTE]
>
>如果目前訂閱的密碼不符合第二個受邀訂閱的密碼政策，Marketo會要求想要使用Universal ID的使用者重設密碼。

## 在預訂之間切換{#switching-between-subscriptions}

使用通用ID，您可以看到您登入的訂閱，並選取您有登入存取權的其他訂閱。 在大多數情況下，您可以在它們之間切換，而不需要登出和重新登入。

![](assets/image2016-11-3-15-3a10-3a16.png)

當您登出並重新登入時，Marketo會自動將您登入上次登入的訂閱。 然後，如有需要，您可以切換至其他訂閱。

## 社群資料{#community-profiles}

如果您有多個訂閱，則可能有多個社群設定檔。 建議您選擇與您最活躍的社群設定檔連結的登入。

## 行動平台{#mobile-platform}

使用通用ID的使用者可從上次登入的訂閱，在Marketo Moments和iPad事件登入應用程式中查看其資料。 您無法從行動平台本身變更訂閱。

>[!MORELIKETHIS]
>
>* [將單一登入新增至入口網站](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [僅限使用者登入SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [邀請Marketo使用者使用兩個具有通用ID的例項](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

