---
description: AdobeIdentity Management概述 — Marketo檔案 — 產品檔案
title: AdobeIdentity Management概述
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: 05377b78181d002926623268d1fdca40c7b80f46
workflow-type: tm+mt
source-wordcount: '1098'
ht-degree: 0%

---

# AdobeIdentity Management概述 {#adobe-identity-management-overview}

如果您在2022年2月15日起有新的Adobe Marketo Engage帳戶（新帳戶，而非現有帳戶的新執行個體），該帳戶可能會與AdobeIdentity Management系統整合，視購買的產品套件而定。 若要了解您是否擁有，請連絡您的Marketo管理員或帳戶的客戶成功經理。

現有Marketo訂閱將於2023年下半年開始移轉至AdobeIdentity Management系統。

>[!NOTE]
>
>Marketo支援將無法提供任何Adobe IMS移轉的更新。 您的客戶成功經理將在未來幾個月內提供預估時間表。

## 設定檔層級 {#profile-levels}

上架至AdobeIdentity Management系統的Adobe Marketo Engage訂閱支援各種設定檔。 以下是與此整合相關的使用者設定檔類型。

<table>
 <tr>
  <td><strong>Adobe Admin Console系統管理員</strong></td>
  <td>負責在Adobe Admin Console中設定Adobe組織和Marketo Engage產品的身分概念。 已在Adobe組織設定中授予角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console產品管理員</strong></td>
  <td>負責授權Adobe Admin Console中Marketo Engage產品的使用者。 授予在Adobe Admin Console的角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console產品設定檔管理員</strong></td>
  <td>負責管理產品設定檔中的使用者。 他們無法管理該特定設定檔以外的使用者。 除非以使用者身分新增至產品設定檔，否則產品設定檔管理員無法存取Marketo應用程式。 其角色仍為標準使用者（若有多個工作區，則為預設工作區）。
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage產品管理員</strong></td>
  <td>具有管理權限的Marketo Engage訪問權限的人員。 授予Marketo Engage角色，而非Adobe Admin Console。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage使用者</strong></td>
  <td>已獲准訪問Marketo Engage的人。 無管理權限。</td>
 </tr>
</table>

## 常見問題集 {#faq}

**什麼是Adobe身分？**

AdobeIdentity Management系統包含三個元件。

* AdobeIdentity服務：處理最終用戶的驗證和驗證，包括聯合和運行時單一登錄(SSO)。

* Adobe Admin Console:Admin Console提供管理整個組織Adobe權益的集中位置。 它負責用戶管理、雲服務、案頭許可證權限、聯合配置，並提供資料丟失防護安全功能。

* Adobe使用者管理API(UMAPI):可讓組織在Adobe Admin Console中，透過API層級管理企業使用者和權益。

**現有Marketo Engage訂閱何時會與IMS整合？**

今年晚些時候，現有Marketo訂閱將移轉至AdobeIdentity Management系統。 Marketo支援將無法提供任何Adobe IMS移轉的更新。 您的客戶成功經理將在未來幾個月內提供預估時間表。

**Adobe產品管理員和Marketo Engage管理員之間有何差異？**

* Adobe產品管理員是Marketo平台中的新角色。
* Adobe產品管理員角色可授予在Adobe Admin Console中新增為產品管理員的使用者
* Adobe產品管理員是唯讀角色，無法從Marketo Engage編輯或刪除。
* Adobe產品管理員與標準Marketo管理員有相同的權限。
* Marketo Engage管理員的角色仍為管理員，且已授予Marketo Engage中的使用者。

**使用者管理API用戶端支援是否有任何變更？**

是. 已上線至Adobe IMS的使用者無法使用所有現有的Marketo使用者管理API。 若為使用者邀請、更新和刪除動作，則Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html) 的URL。 對於角色管理，仍會套用Marketo使用者管理API。 除此之外，Marketo REST API用戶端支援並無其他變更。

**如果我們已與IMS整合，我們會聯絡誰以尋求支援？**

您需遵循標準程式聯絡 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support).

**如果我使用Adobe身分來存取其他Adobe應用程式，可以使用它來存取Marketo嗎？**

即使您有其他Adobe產品，除非訂閱移轉至IMS，否則您無法使用Adobe身分存取Marketo。

**Marketo使用者角色（在工作區內）是否在Adobe Admin Console中管理？**

否. 使用者角色管理（在工作區內）已在Marketo Engage中完成。

**我是IMS整合訂閱的Marketo管理員，無法存取Admin Console。 如何取得存取權？**

任何Adobe系統或產品管理員只要能存取組織的Admin Console，就能授予您存取權。 如果您不確定組織中的誰在主控台中擁有管理員權限，請聯絡 [Adobe客戶服務](https://helpx.adobe.com/contact.html).

**管理員如何將使用者新增至Marketo Sales Connect?**

雖然Sales Connect的Admin Console中會有產品卡，但不應使用Admin Console來新增/管理使用者。 以下連結可讓管理員透過Marketo Sales Connect管理使用者： [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**我可以在何處進一步了解Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**我是否仍會前往Marketo的「管理員」區段，為我的帳戶變更使用者帳戶？**

否，您需要導覽至 [account.adobe.com](https://account.adobe.com).

**這如何與Marketo的Universal ID搭配運作？**

已上線至Adobe身分的訂閱可透過產品的訂閱切換器，順暢地存取所有啟用IMS的訂閱。

**這適用於SSO嗎？**

是. Marketo與Adobe IMS的整合支援通用ID使用者和SSO。 SSO現在由Adobe IMS驅動，並在Adobe Admin Console的組織層級設定。 [如需詳細資訊，請前往這裡](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**裝置授權如何運作？**

Adobe IMS目前不支援任何類似Marketo裝置授權功能的功能。

**是否仍可使用「在邀請使用者對話方塊中登入」功能，讓使用者的登入從其電子郵件中變得唯一？**

否. 當訂閱啟用IMS時，「使用者邀請」工作流程不再作用中，因此功能不再有效。 Adobe身分識別需要使用者的身分識別，由其電子郵件驅動。

**若為Adobe IMS，我們可以選擇使用Adobe ID、Enterprise ID或Federated ID?**

是，您可以決定要取得組織支援的身分類型。 如需詳細資訊，請前往： [身分概述](https://helpx.adobe.com/enterprise/using/identity.html) 和此處： [設定身分](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**Adobe Admin Console支援哪些產品卡？**

支援的產品卡包括：Marketo Engage、Marketo Measure、Marketo動態聊天、Marketo Sales Connect和Marketo Sales Insight Actions。

>[!MORELIKETHIS]
>
>* [管理設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [新增或移除產品管理員](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [新增或移除使用者](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

