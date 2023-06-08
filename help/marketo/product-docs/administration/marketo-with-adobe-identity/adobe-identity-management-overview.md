---
description: AdobeIdentity Management概述 — Marketo檔案 — 產品檔案
title: AdobeIdentity Management概觀
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 0%

---

# AdobeIdentity Management概觀 {#adobe-identity-management-overview}

如果您在2022年2月15日擁有具有Adobe Marketo Engage的新帳戶（新帳戶，而不僅僅是現有帳戶的新執行個體），則根據購買的產品套件，它可能與AdobeIdentity Management系統整合。 若要確認您是否擁有該軟體，請聯絡Adobe客戶團隊（您的客戶經理）。

現有的Marketo訂閱將於2023年下半年開始移轉至AdobeIdentity Management系統。

>[!NOTE]
>
>Marketo支援將無法提供有關Adobe IMS移轉的任何更新。 Adobe客戶團隊將在未來幾個月提出預估時間表。

## 設定檔層級 {#profile-levels}

Adobe Marketo Engage訂閱上線至AdobeIdentity Management系統可支援各種設定檔。 以下是與此整合相關的使用者設定檔型別。

<table>
 <tr>
  <td><strong>Adobe Admin Console系統管理員</strong></td>
  <td>負責在Adobe Admin Console中設定Adobe組織和Marketo Engage產品的身分概念。 在Adobe組織設定時授與的角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console產品管理員</strong></td>
  <td>負責在Adobe Admin Console中授予使用者Marketo Engage產品的權利。 在Adobe Admin Console中授與的角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console產品設定檔管理員</strong></td>
  <td>負責管理產品設定檔中的使用者。 他們無法在該特定設定檔之外管理使用者。 除非以使用者身分新增至產品設定檔，否則產品設定檔管理員無法存取Marketo應用程式。 他們的角色仍會是標準使用者（如果有多個工作區，則為預設工作區）。
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage產品管理員</strong></td>
  <td>獲授具有管理許可權之Marketo Engage存取許可權的人員。 已授與Marketo Engage中的角色，而非Adobe Admin Console。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage使用者</strong></td>
  <td>被授與Marketo Engage存取許可權的人員。 沒有管理許可權。</td>
 </tr>
</table>

## 常見問題集 {#faq}

**什麼是Adobe身分？**

AdobeIdentity Management系統包含三個元件。

* [!DNL Adobe Identity Service]：處理一般使用者的驗證和驗證，包括同盟和執行階段單一登入(SSO)。

* Adobe Admin Console：此Admin Console提供一個中央位置，用於管理整個組織的Adobe權益。 它會處理使用者管理、雲端服務、案頭授權權益、同盟設定，並提供資料遺失預防安全性功能。

* Adobe使用者管理API (UMAPI)：可讓組織在Adobe Admin Console中透過API層級管理企業使用者和權益。

**現有的Marketo Engage訂閱何時會與IMS整合？**

現有的Marketo訂閱將在今年晚些時候移轉至AdobeIdentity Management系統。 Marketo支援將無法提供有關Adobe IMS移轉的任何更新。 Adobe客戶團隊將在未來幾個月提出預估時間表。

**Adobe產品管理員和Marketo Engage管理員有何不同？**

* Adobe產品管理員是Marketo平台中的新角色。
* Adobe產品管理員角色已授與在Adobe Admin Console中新增為產品管理員的使用者
* Adobe產品管理員為唯讀角色，無法編輯或從Marketo Engage刪除。
* Adobe產品管理員的許可權和許可權與標準Marketo管理員相同。
* Marketo Engage管理員的角色仍然是管理員，並授予使用者Marketo Engage。

**使用者管理API使用者端支援是否有任何變更？**

是. 已上線至Adobe IMS的使用者無法使用所有現有的Marketo使用者管理API。 對於使用者邀請、更新和刪除動作，Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} 應該使用。 對於角色管理，Marketo使用者管理API仍適用。 除此之外，Marketo REST API使用者端支援沒有其他變更。

**如果與IMS整合，我們會聯絡誰尋求支援？**

若要聯絡，請遵循標準程式 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

**如果我使用Adobe身分來存取其他Adobe應用程式，可以使用該身分來存取Marketo嗎？**

即使您有其他Adobe產品，在訂閱移轉至IMS之前，您無法使用Adobe身分識別存取Marketo。

**Marketo使用者角色（位於工作區內）是否在Adobe Admin Console中管理？**

否. 使用者角色管理（在工作區中）已在Marketo Engage中完成。

**我是IMS整合式訂閱的Marketo管理員，無法存取Admin Console。 如何取得存取權？**

任何有權存取貴組織Admin Console的Adobe系統或產品管理員都可以授予您存取權。 如果您不確定貴組織中的哪些人擁有主控台的管理員許可權，請聯絡 [Adobe客戶服務](https://helpx.adobe.com/contact.html){target="_blank"}.

**管理員如何將使用者新增至Marketo [!DNL Sales Connect]？**

雖然Admin Console中會有產品卡 [!DNL Sales Connect]，Admin Console不應用於新增/管理使用者。 下列連結可讓管理員透過Marketo管理使用者 [!DNL Sales Connect]： [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**我可以在何處進一步瞭解Adobe Admin Console？**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html){target="_blank"}.

**我是否仍會前往Marketo中的「管理員」區段，對我的帳戶進行使用者帳戶變更？**

否，您需要導覽至 [account.adobe.com](https://account.adobe.com){target="_blank"}.

**這如何與Marketo的通用ID搭配運作？**

已上線Adobe身分識別的使用者可透過產品中的訂閱切換器，順暢地存取所有啟用IMS的訂閱。

**這是否適用於SSO？**

是. Marketo與Adobe IMS的整合可支援通用ID使用者和SSO。 SSO現在由Adobe IMS驅動，並在Adobe Admin Console中的組織層級設定。 [在此處瞭解更多](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**裝置授權如何運作？**

Adobe IMS目前不支援Marketo的裝置授權功能之類的功能。

**是否仍可使用「在邀請使用者對話方塊中登入」功能，讓使用者的登入在其電子郵件中是唯一的？**

否. 訂閱啟用了IMS時，使用者邀請工作流程不再有效，因此功能不再有效。 Adobe身分需要使用者的身分由其電子郵件驅動。

**對於Adobe IMS，我們是否可選擇使用Adobe ID、Enterprise ID或Federated ID？**

可以，您可以決定要獲得組織支援的身分型別。 如需詳細資訊，請前往此處： [身分概述](https://helpx.adobe.com/enterprise/using/identity.html) 以及此處： [設定身分](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Adobe Admin Console支援哪些產品卡？**

支援的產品卡包括：Marketo Engage、Marketo Measure、Marketo Dynamic Chat、Marketo Sales Connect和Marketo Sales Insight Actions。

>[!MORELIKETHIS]
>
>* [管理員設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [新增或移除產品管理員](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [新增或移除使用者](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
