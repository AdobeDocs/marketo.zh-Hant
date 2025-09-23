---
unique-page-id: 14352405
description: 透過 [!DNL Sales Connect] 中的SAML 2.0設定SSO- Marketo檔案 — 產品檔案
title: 透過 [!DNL Sales Connect]中的SAML 2.0設定SSO
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# 透過[!DNL Sales Connect]中的SAML 2.0設定SSO {#setting-up-sso-through-saml-in-sales-connect}

我們透過SAML 2.0規格支援SSO。 不過，我們目前沒有任何提供者直接整合。 我們需要從您的SSO提供者收集一些資訊，才能進行此設定。

>[!NOTE]
>
>這僅適用於&#x200B;**Marketo Sales Connect**&#x200B;使用者。 如果您沒有Sales Connect但想深入瞭解，請聯絡Adobe客戶團隊（您的客戶經理）。

## 需求 {#requirements}

* SSO帳戶
* Marketo Sales Connect訂閱
* 來自SSO帳戶的Metadata.xml （問題URL、驗證的端點和公開金鑰）

## 設定 {#setup}

來自您團隊之SSO執行個體的metadata.xml應包含簽發者URL、驗證的端點以及公開金鑰。

我們還需要貴公司的SSO帳戶的SSO位置為唯一網域。 例如，我們需要像`toutapp.pingidentity.com`或類似的唯一子網域。 若沒有這類唯一識別碼，我們將無法從儀表板設定SAML。

指派URL時，單一登入和Okta不一定會提供唯一識別碼。 如果您使用Okta或單次登入，表示我們無法透過控制面板按鈕設定單次登入。 我們仍可透過[網頁應用程式](https://toutapp.com/login)上的[單一登入]按鈕進行設定。

取得這些資訊後，我們會與工程團隊合作，為您訂閱完成此項設定。
