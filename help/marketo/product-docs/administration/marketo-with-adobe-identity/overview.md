---
description: 概述 — Marketo檔案 — 產品檔案
title: 概述
hide: true
hidefromtoc: true
source-git-commit: 066ecb9fe52e9fe3f9c78815b47cf41208f396c3
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# 概述 {#overview}

如果您的AdobeMarketo Engage訂閱已布建於10/4/21年或之後，則會與AdobeIdentity Management系統整合。 AIMS可讓使用者使用通用的Marketo Engage身分登入Experience Cloud和其他Adobe應用程式。

## 設定檔層級

有三個設定檔層級。

<table>
 <tr>
  <td><strong>系統管理員</strong></td>
  <td>負責在Adobe Admin Console中設定Adobe組織和Marketo Engage產品的身分概念。</td>
 </tr>
 <tr>
  <td><strong>產品管理員</strong></td>
  <td>負責授權Adobe Admin Console中Marketo Engage產品的使用者。</td>
 </tr>
 <tr>
  <td><strong>使用者</strong></td>
  <td>已獲准訪問Marketo Engage的人。 無管理權限。</td>
 </tr>
</table>

## 常見問題集

**什麼是Adobe身分？**

AdobeIdentity Management系統包含三個元件。

* AdobeIdentity服務：處理最終用戶的驗證和驗證，包括聯合和運行時單一登錄(SSO)。

* Adobe Admin Console:Admin Console提供管理整個組織Adobe權益的集中位置。 它負責用戶管理、雲服務、案頭許可證權限、聯合配置，並提供資料丟失防護安全功能。

* Adobe使用者管理API(UMAPI):可讓組織在Adobe Admin Console中，透過API層級管理企業使用者和權益。

**Adobe產品管理員和Marketo Engage管理員之間有何差異？**

* Adobe產品管理員是Marketo平台中的新角色。
* 此角色為唯讀角色，無法從Marketo編輯或刪除。
* 其權限與標準Marketo管理員相同。

**API用戶端支援是否有任何變更？**

是。 已上線至Adobe IMS的使用者無法使用現有的Marketo使用者管理API。 他們會使用[IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html)。

**我們要聯繫誰以尋求支援？**

您可以依照聯絡[Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support)的標準程式操作。

**Marketo使用者角色（在工作區內）是否在Adobe Admin Console中管理？**

不。 使用者角色管理（在工作區內）已在Marketo中完成。

**我是Marketo管理員，無法存取Admin Console。如何獲得訪問權？**

任何系統或產品管理員只要能存取貴組織的Admin Console，就能授予您存取權。 如果您不確定組織中誰在主控台中擁有管理員權限，請聯絡[Adobe客戶服務](https://helpx.adobe.com/contact.html)。

**管理員如何將使用者新增至Marketo Sales Connect?**

雖然AC for Sales Connect中將有一張產品卡，但不應使用AC來添加/管理用戶。 以下連結可讓管理員透過Marketo Sales Connect管理使用者：[https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management)。

**我可以在何處進一步了解Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**我是否仍會前往Marketo的「管理員」區段進行帳戶變更？**

否，您需要導覽至[account.adobe.com](account.adobe.com)。

**這如何與Marketo的Universal ID搭配運作？**

已上線至Adobe身分的訂閱可透過產品的訂閱切換器，順暢地存取所有啟用IMS的訂閱。

**這適用於SSO嗎？**

是。 Marketo與Adobe IMS的整合支援通用ID使用者和SSO。 SSO現在由Adobe IMS驅動，並在Adobe Admin Console的組織層級設定。 [如需詳細資訊，請參閱](https://helpx.adobe.com/enterprise/using/set-up-identity.html)。

**裝置授權如何運作？**

Adobe IMS目前不支援任何類似Marketo裝置授權功能的功能。

**是否仍可使用「邀請使用者對話方塊中的登入」功能，讓電子郵件中的登入不重複？**

不。 當訂閱啟用IMS時，「使用者邀請」工作流程不再作用中，因此功能不再有效。 Adobe身分識別需要使用者的身分識別，由其電子郵件驅動。

**若為Adobe IMS，我們可以選擇使用Adobe ID、Enterprise ID或Federated ID?**

是，您可以決定要取得組織支援的身分類型。 更多資訊[此處](https://helpx.adobe.com/enterprise/using/identity.html)和[此處](https://helpx.adobe.com/enterprise/using/set-up-identity.html)。
