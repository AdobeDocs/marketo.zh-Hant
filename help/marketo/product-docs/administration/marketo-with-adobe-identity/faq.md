---
description: AdobeIdentity Management常見問題集 — Marketo檔案 — 產品檔案
title: AdobeIdentity Management常見問題集
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: eca77d8426c8f696dc35dbfb9e20abcb46e53127
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 1%

---

# AdobeIdentity Management常見問題集 {#adobe-identity-management-faq}

**什麼是Adobe身分？**

AdobeIdentity Management系統包含三個元件。

* [!DNL Adobe Identity Service]：處理一般使用者的驗證和驗證，包括同盟和執行階段單一登入(SSO)。

* Adobe Admin Console：此Admin Console提供一個中央位置，用於管理整個組織的Adobe權益。 它會處理使用者管理、雲端服務、案頭授權權益、同盟設定，並提供資料遺失預防安全性功能。

* Adobe使用者管理API (UMAPI)：可讓組織在Adobe Admin Console中透過API層級管理企業使用者和權益。

**現有的Marketo Engage訂閱何時會與IMS整合？**

現有的Marketo訂閱將在今年晚些時候移轉至Adobe的Identity Management系統。 Marketo支援將無法提供有關Adobe IMS移轉的任何更新。 Adobe客戶團隊將在未來幾個月提出預估時間表。

**Adobe產品管理員和Marketo Engage管理員有何不同？**

* Adobe產品管理員是Marketo平台的新角色。
* Adobe產品管理員角色已授與在Adobe Admin Console中新增為產品管理員的使用者
* Adobe產品管理員是唯讀角色，無法編輯或從Marketo Engage刪除。
* Adobe產品管理員具有與標準Marketo管理員相同的許可權和許可權。
* Marketo Engage管理員的角色仍然是管理員，並授予使用者Marketo Engage。

**使用者管理API使用者端支援是否有任何變更？**

有。已上線Adobe IMS的使用者無法使用所有現有的Marketo使用者管理API。 對於使用者邀請、更新和刪除動作，Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} 該使用。 若是角色管理，仍會套用Marketo User Management API。 除此之外，Marketo REST API使用者端支援沒有其他變更。

**如果我們已與IMS整合，需要聯絡誰來取得支援？**

您會遵循標準程式來聯絡 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

**如果我使用Adobe身分來存取其他Adobe應用程式，可以使用該身分來存取Marketo嗎？**

即使您有其他Adobe產品，在訂閱移轉至IMS之前，您無法使用Adobe身分存取Marketo。

**Marketo的使用者角色（位於工作區中）是否在Adobe Admin Console中進行管理？**

否. 使用者角色管理（在工作區中）在Marketo Engage中完成。

**我是IMS整合式訂閱的Marketo管理員，無法存取Admin Console。 如何取得存取權？**

任何可存取貴組織Admin Console的Adobe系統或產品管理員都可以為您提供存取權。 如果您不確定貴組織中的哪些人擁有主控台中的管理員許可權，請聯絡 [Adobe客戶服務](https://helpx.adobe.com/contact.html){target="_blank"}.

**管理員如何將使用者新增至Marketo [!DNL Sales Connect]？**

雖然Admin Console中會有產品卡 [!DNL Sales Connect]，Admin Console不應用於新增/管理使用者。 下列連結可讓管理員透過Marketo管理使用者 [!DNL Sales Connect]： [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**我可以在何處進一步瞭解Adobe Admin Console？**

[https://helpx.adobe.com/tw/enterprise/admin-guide.html](https://helpx.adobe.com/tw/enterprise/admin-guide.html){target="_blank"}.

**我仍要移至Marketo的「管理員」區段，針對我的帳戶變更使用者帳戶嗎？**

否，您需要導覽至 [account.adobe.com](https://account.adobe.com){target="_blank"}.

**這如何與Marketo的通用ID搭配運作？**

已上線Adobe身分的訪客可透過產品中的訂閱切換器，順暢存取所有啟用IMS的訂閱。

**這是否適用於SSO？**

有。Marketo與Adobe IMS的整合可支援通用ID使用者和SSO。 SSO現在由Adobe IMS驅動，並在Adobe Admin Console中的組織層級設定。 [在此處瞭解更多](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**裝置授權如何運作？**

Adobe IMS目前不支援Marketo的裝置授權功能之類的功能。

**是否仍可使用「在邀請使用者對話方塊中登入」功能，讓使用者的登入在電子郵件中是唯一的？**

否. 訂閱啟用IMS時，使用者邀請工作流程不再有效，因此功能不再有效。 Adobe身分需要使用者的身分由其電子郵件驅動。

**對於Adobe IMS，我們是否可選擇使用Adobe ID、Enterprise ID或Federated ID？**

可以，您可以決定要獲得組織支援的身分型別。 如需詳細資訊，請前往此處： [身分概述](https://helpx.adobe.com/enterprise/using/identity.html) 以及此處： [設定身分](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Adobe Admin Console支援哪些產品卡？**

支援的產品卡包括：Marketo Engage、Marketo Measure、Marketo Dynamic Chat、Marketo Sales Connect和Marketo Sales Insight Actions。

**如果我移轉至Adobe身分時，使用者登入與電子郵件不符，該怎麼辦？**

目前登入與電子郵件地址不同的Marketo使用者，在移轉至Adobe身分識別後，將不再使用該認證登入。 Adobe身分一律使用使用者的電子郵件地址進行驗證。

**如果我的訂閱使用IP限制設定，則Adobe身分移轉後會發生什麼事？**

當訂閱上線至Adobe身分時，IP限制設定不會移轉至Adobe Admin Console。 Marketo的IP限制設定包括僅允許從特定IP位址存取，以及封鎖特定IP位址的存取。 目前，Adobe Identity Management系統不支援IP限制功能。

Adobe Identity Management System將於2024年推出一項功能，僅支援允許特定IP位址，以支援目前使用此功能的Marketo使用者的轉換。 目前使用此功能的使用者在功能發行前不會進行使用者移轉。 交付功能後，使用者將會收到排程其移轉的通知。 我們會在有需要時提供有關功能的詳細資訊。

目前使用IP限制以封鎖特定位址存取的使用者，在移轉至Adobe身分識別後將無法再使用此功能，因為AdobeIdentity Management系統不支援此功能。

**如果我的使用者具有「略過單一登入」的選項，則Adobe身分移轉後會發生什麼事？**

當訂閱上架到Adobe身分時，單一登入(SSO)是在Adobe組織層級為所有使用者設定。 設定SSO時，將會對該Adobe組織中的所有Marketo使用者/所有Marketo執行個體強制執行。之前，Marketo支援將使用者角色設定為可選用「略過單一登入」。 Adobe Identity Management系統不支援此功能。

**我有多個訂閱，但並非所有訂閱都啟用單一登入。 Adobe身分移轉之後會發生什麼事？**

當訂閱上架到Adobe身分時，單一登入(SSO)會在Adobe組織層級設定。 這表示SSO適用於Adobe組織中的所有產品執行個體。SSO設定後，將套用至該Adobe組織中的所有Marketo執行個體。之前，Marketo在執行個體層級支援此設定。 Adobe Identity Management系統不支援此功能。
