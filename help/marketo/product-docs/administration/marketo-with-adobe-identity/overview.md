---
description: 概述 — Marketo文檔 — 產品文檔
title: 概述
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: 7eff888c0fdebf31da4706f70d1e99e8327807ca
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 概述 {#overview}

如果您在2022年2月15日擁有了具有AdobeMarketo Engage的新帳戶（新帳戶，而不僅僅是現有帳戶的新實例），則它可能會與AdobeIdentity Management系統整合，具體取決於購買的產品包。 要瞭解您是否擁有它，請聯繫您的Marketo管理員或您帳戶的客戶成功經理。

現有的Marketo訂戶將從今年晚些時候遷入AdobeIdentity Management系統。

>[!NOTE]
>
>Marketo支援將無法提供有關Adobe IMS遷移的任何更新。 您的客戶成功經理將在未來幾個月內與預計時間表聯繫。

## 配置檔案級別

AdobeMarketo Engage訂閱登入AdobeIdentity Management系統支援各種配置檔案。 以下是與此整合相關的用戶配置檔案類型。

<table>
 <tr>
  <td><strong>Adobe Admin Console系統管理</strong></td>
  <td>負責為Adobe Admin Console的Adobe組織和Marketo Engage產品設定身份概念。 在Adobe組織設定中授予的角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console產品管理</strong></td>
  <td>負責在Adobe Admin Console授權用戶購買Marketo Engage產品。 被授予在Adobe Admin Console的角色。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage產品管理</strong></td>
  <td>已授予具有管理權限的Marketo Engage訪問權限的人員。 在Marketo Engage，而不是Adobe Admin Console。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage用戶</strong></td>
  <td>一個被允許接觸Marketo Engage的人。 無管理權限。</td>
 </tr>
</table>

## 常見問題

**什麼是Adobe身份？**

AdobeIdentity Management系統由三部分組成。

* Adobe身份服務：處理最終用戶的驗證和驗證，包括聯合和運行時單一登錄(SSO)。

* Adobe Admin Console:該Admin Console為管理整個組織的Adobe權利提供了一個中心位置。 它處理用戶管理、雲服務、案頭許可證權利、聯合配置，並提供資料丟失預防安全功能。

* Adobe用戶管理API(UMAPI):允許組織在API級別管理Adobe Admin Console的企業用戶和權利。

**現有Marketo Engage訂購何時與IMS整合？**

現有Marketo訂戶將於今年晚些時候遷入AdobeIdentity Management系統。 Marketo支援將無法提供有關Adobe IMS遷移的任何更新。 您的客戶成功經理將在未來幾個月內與預計時間表聯繫。

**Adobe產品管理員和Marketo Engage管理員之間有何區別？**

* Adobe產品管理是Marketo平台中的新角色。
* Adobe產品管理員角色授予在Adobe Admin Console添加為產品管理員的用戶
* Adobe產品管理是只讀角色，無法從Marketo Engage中編輯或刪除。
* Adobe產品管理員與標準Marketo管理員具有相同的權限和權限。
* Marketo Engage管理員的角色仍為管理員，並授予Marketo Engage中的用戶。

**用戶管理API客戶端支援是否有任何更改？**

是的。 已加入Adobe IMS的用戶不能利用所有現有的Marketo用戶管理API。 對於用戶邀請、更新和刪除操作，Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html) 應使用。 對於角色管理，Marketo用戶管理API仍然適用。 除此之外，對MarketoREST API客戶端支援沒有其他更改。

**如果我們與IMS整合，我們將聯繫誰以獲得支援？**

您將按照標準程式聯繫 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support)。

**Marketo用戶角色（在工作區內）是否在Adobe Admin Console管理？**

不。 用戶角色管理（在工作區內）在Marketo Engage中完成。

**我是IMS整合訂閱的Marketo管理員，無權訪問Admin Console。 如何獲得訪問權？**

任何Adobe系統或產品管理員都可以訪問您組織的Admin Console。 如果您不確定組織中的哪些人在控制台中具有管理員權限，請與 [Adobe客戶關懷](https://helpx.adobe.com/contact.html)。

**管理員如何將用戶添加到Marketo銷售連接？**

雖然Admin Console中將有一張產品卡用於Sales Connect ，但不應使用Admin Console來添加/管理用戶。 以下連結將允許管理員通過Marketo銷售連接管理用戶： [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management)。

**哪裡可以瞭解更多關於Adobe Admin Console的資訊？**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html)。

**我是否仍然會轉到Marketo的「管理」部分來更改我的帳戶的用戶帳戶？**

不，你需要導航到 [account.adobe.com](https://account.adobe.com)。

**這與Marketo的通用ID有什麼關係？**

那些被接入Adobe標識的用戶可以通過產品中的訂閱切換器無縫地訪問所有支援IMS的訂閱。

**這與SSO配合使用嗎？**

是的。 Marketo與Adobe IMS的整合支援通用ID用戶和SSO。 目前，SSO由Adobe IMS驅動，在Adobe Admin Console的組織級別設定。 [在此處瞭解更多資訊](https://helpx.adobe.com/enterprise/using/set-up-identity.html)。

**設備授權如何工作？**

Adobe IMS目前不支援任何類似Marketo設備授權功能的功能。

**是否仍可以使用「在邀請用戶對話框中登錄」功能，使用戶的登錄在其電子郵件中唯一？**

不。 當訂閱啟用IMS時，「用戶邀請」工作流不再處於活動狀態，因此該功能不再有效。 Adobe身份要求用戶的身份由其電子郵件驅動。

**對於Adobe IMS，我們是否可以選擇使用Adobe ID、Enterprise ID或Federated ID?**

是，您確定要獲得組織支援的身份類型。 更多資訊可在以下位置找到： [身份概述](https://helpx.adobe.com/enterprise/using/identity.html) 這裡： [設定標識](https://helpx.adobe.com/enterprise/using/set-up-identity.html)。

>[!MORELIKETHIS]
>
>* [管理設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [添加或刪除產品管理員](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [添加或刪除用戶](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

