---
unique-page-id: 14352405
description: 在Sales Connect - Marketo檔案 — 產品檔案中透過SAML 2.0設定SSO
title: 在Sales Connect中通過SAML 2.0設定SSO
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# 在Sales Connect中通過SAML 2.0設定SSO {#setting-up-sso-through-saml-in-sales-connect}

我們透過SAML 2.0規格支援SSO。 不過，目前我們尚未與任何提供者直接整合。 我們需要從您的SSO提供者收集一些資訊，才能進行此設定。

>[!NOTE]
>
>這僅適用於 **Marketo Sales Connect** 客戶。 如果您沒有Sales Connect，但想要了解更多資訊，請聯繫您的客戶成功經理。

## 需求 {#requirements}

* SSO帳戶
* Marketo Sales connect訂閱
* 來自SSO帳戶的metadata.xml（問題URL、驗證的端點以及公開金鑰）

## 設定 {#setup}

來自您團隊SSO例項的metadata.xml應包含核發者URL、驗證的端點以及公開金鑰。

我們還需要您公司SSO帳戶的SSO位置為唯一網域。 例如，我們需要一個唯一的子網域，例如 `toutapp.pingidentity.com` 或類似。 若沒有這類唯一識別碼，我們就無法從控制面板設定SAML。

指派URL時，一次登入和Okta不一定會提供唯一識別碼。 如果您使用Okta或One Login，表示我們將無法從控制面板按鈕設定一次登入。 我們仍可從 [網頁應用程式](https://toutapp.com/login).

取得這些資訊後，我們會與工程團隊合作，為您的訂閱設定此資訊。
