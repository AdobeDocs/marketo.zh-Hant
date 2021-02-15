---
unique-page-id: 14352405
description: 在Sales Connect —— 行銷人員檔案——產品檔案中透過SAML 2.0設定SSO
title: 在Sales Connect中透過SAML 2.0設定SSO
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# 在Sales Connect {#setting-up-sso-through-saml-in-sales-connect}中透過SAML 2.0設定SSO

我們透過SAML 2.0規格支援SSO。 不過，我們目前並未與任何供應商直接整合。 我們必須向您的SSO提供者收集一些資訊，才能取得此設定。

>[!NOTE]
>
>這僅適用於&#x200B;**Marketo Sales Connect**&#x200B;客戶。 如果您沒有Sales Connect但想要瞭解更多資訊，請聯絡您的客戶成功經理。

## 要求{#requirements}

* SSO帳戶
* Marketo Sales connect訂閱
* 來自SSO帳戶的Metadata.xml（期刊URL、驗證的端點和公開金鑰）

## 設定{#setup}

您團隊的SSO例項中的metadata.xml應包含發行者URL、驗證的端點和公開金鑰。

我們也需要您公司SSO帳戶的SSO位置，才能成為唯一網域。 例如，我們需要一個唯一的子網域，如`toutapp.pingidentity.com`或類似網域。 若沒有此類型的唯一識別碼，我們將無法從控制面板設定SAML。

指派URL時，「單一登入」和「Okta」並不一律提供唯一識別碼。 如果您使用Okta或One Login，表示我們無法從控制面板按鈕設定一次登入。 我們仍能從[Web應用程式](https://toutapp.com/login)上的「單一登入」按鈕設定它。

一旦我們取得該資訊，我們將與我們的工程團隊合作，為您的訂閱設定此資訊。
