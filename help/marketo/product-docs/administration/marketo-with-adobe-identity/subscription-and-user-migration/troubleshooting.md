---
description: Adobe IMS使用者移轉疑難排解指南 — Marketo檔案 — 產品檔案
title: Adobe IMS使用者移轉疑難排解指南
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: 31af9ceaaa63b8a286c660ab4e37f9ad40be85f5
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# Adobe IMS使用者移轉疑難排解指南 {#adobe-ims-user-migration-troubleshooting-guide}

在IMS使用者移轉程式中，會針對每個要移轉的Adobe使用者建立一個Marketo Engage使用者（除非該使用者已存在相同電子郵件地址）。 有時不會建立它，這可能歸因於使用者在Active Directory中的記錄或電子郵件地址有問題。

本文針對執行自行移轉的使用者，列出您在自行移轉主控台狀態列位中看到的每個錯誤訊息。

>[!NOTE]
>
>目錄/網域相關錯誤可由另一個已設定目錄信任或已宣告網域的org/Admin Console觸發。

## 錯誤訊息 {#error-messages}

首先，判斷使用者是否需要移轉，因為這將影響要遵循的解決步驟。

使用右側的「在此頁面上」區段，直接跳至特定錯誤。

### Gmail無效字元 {#gmail-invalid-character}

**根本原因**：根據Adobe安全性原則，Gmail電子郵件地址中不允許字元`.`和`+`。 非Gmail電子郵件地址中允許使用這兩個字元。

**解析度**：

_如果使用者需要移轉_ — 電子郵件地址必須在Marketo Engage中更新，以符合Adobe安全性原則並復原。 Marketo管理員，接著從移轉控制檯為此使用者重新執行使用者移轉。

_如果使用者&#x200B;**不**需要移轉_ - Marketo Engage管理員在移轉主控台中略過該使用者。 「移轉完成」按鈕會在移轉或略過以說明所有使用者時出現。 按一下按鈕，結束使用者移轉程式。

### 使用者不在目錄中 {#user-not-in-directory}

**根本原因**：使用者不存在於Active Directory (AD)中。 對於已啟用AD同步的SSO組織，僅允許透過身分提供者(IdP)建立使用者。 因此，無法在使用者移轉期間透過Admin Console新增使用者。

**解析度**：

_如果使用者需要移轉_ — 系統管理員必須將該使用者新增到Active Directory，並擁有適當的許可權。 Marketo Engage管理員，接著從移轉控制檯為此使用者重新執行使用者移轉。

_如果使用者&#x200B;**不**需要移轉_ - Marketo Engage管理員在移轉主控台中略過該使用者。 「移轉完成」按鈕會在移轉或略過以說明所有使用者時出現。 按一下按鈕，結束使用者移轉程式。

### 非作用中的使用者 {#inactive-user}

**根本原因**： AD同步已啟用，而且使用者的同盟帳戶存在，但處於非作用中/停用狀態。

**解析度**：

_如果需要移轉使用者_ — 系統管理員必須還原使用者的狀態和適當的許可權。 Marketo Engage管理員，接著從移轉控制檯為此使用者重新執行使用者移轉。

_如果使用者&#x200B;**不**需要移轉_ - Marketo Engage管理員在移轉主控台中略過該使用者。 「移轉完成」按鈕會在移轉或略過以說明所有使用者時出現。 按一下按鈕，結束使用者移轉程式。

### 無效的網域 {#invalid-domain}

**根本原因**： Admin Console中已啟用網域強制執行。 但是，使用者電子郵件地址的網域不是允許的網域之一，或已在另一個組織/Admin Console中要求該網域。

**解析度**：

_如果使用者需要移轉_ （而且移轉的組織已啟用網域強制執行） — 必須在Marketo Engage中更新電子郵件地址，以符合網域強制執行(DE)原則。 或者，系統管理員可以[將網域](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"}移至另一個已停用的網域強制執行(DE)目錄，或[建立不在DE原則下的新目錄](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}。 Marketo Engage管理員，接著從移轉控制檯為此使用者重新執行使用者移轉。

_如果使用者需要移轉_ （且已在其他組織啟用網域強制執行） — 已宣告網域的組織的系統管理員需要將使用者的電子郵件地址新增至例外清單。 Marketo Engage管理員，接著從移轉控制檯為此使用者重新執行使用者移轉。

_如果使用者&#x200B;**不**需要移轉_ - Marketo Engage管理員在移轉主控台中略過該使用者。 「移轉完成」按鈕會在移轉或略過以說明所有使用者時出現。 按一下按鈕，結束使用者移轉程式。

### Type2E失敗 {#type2e-failure}

**根本原因**：如果為組織設定了同盟帳戶(T3)，而且使用者的個別帳戶(T1)已經存在，則任何建立（如果適用）並將僅授權帳戶(T2e)連結至同盟帳戶的嘗試都將失敗，錯誤碼為FAILED_TO_CREATE_TYPE2E_USER。

**解析度**：

1. 從Adobe組織中移除該個別使用者。 _請注意：使用者將會失去所有產品的存取權，並需要稍後重新獲得授權。 如果這樣不好，請聯絡Adobe支援。_
1. 重新執行使用者移轉，以便為此使用者建立同盟使用者帳戶。
1. 將僅建立權益帳戶（如果適用）並連結至Federated帳戶作為其驗證帳戶。

**了解更多**
* [設定身分而不使用單一登入](https://helpx.adobe.com/enterprise/using/set-up-identity.html#:~:text=Set%20up%20identity%20without%20Single%20Sign%2DOn)
* [以單一登入設定身分](https://helpx.adobe.com/enterprise/using/set-up-identity.html#:~:text=Set%20up%20identity%20with%20Single%20Sign%2DOn)

### Pendo移轉失敗 {#pendo-migration-failed}

**根本原因**：使用者的同盟帳戶為非作用中/已停用，或是Active Directory (AD)中遺失。

**解析度**：

_如果需要移轉使用者_

1. 系統管理員必須還原使用者的帳戶狀態和許可權。

1. 對於具有AD同步的SSO組織：

   * 透過身分提供者(IdP)建立使用者。
   * 將使用者資料與AD同步。

1. 對於沒有SSO/AD同步的組織：

   * 重新建立Managed帳戶以還原狀態。
   * 組織管理員必須重新指派角色和許可權。

1. Marketo Engage管理員會在移轉控制檯中重新執行移轉。

1. 如果主控台無法存取，請連絡[Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support)以重新執行移轉。

_如果使用者&#x200B;**不**需要移轉_

* Marketo Engage管理員應在移轉控制檯中略過使用者。
* 移轉或略過所有使用者後，按一下&#x200B;**[!UICONTROL Migration Complete]**&#x200B;以完成。
* 如果錯誤持續發生，請將包含相關詳細資料的支援案例提交至[Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support)。


### 使用者建立失敗 {#user-creation-failed}

[請參閱下文](#failed)

### Marketo權益失敗 {#marketo-entitlement-failed}

[請參閱下文](#failed)

### 使用者資料移轉失敗 {#user-data-migration-failed}

[請參閱下文](#failed)

### 產品資料同步失敗 {#product-data-sync-failed}

[請參閱下文](#failed)

### Adobe權益失敗 {#adobe-entitlement-failed}

[請參閱下文](#failed)

### 使用者登出失敗 {#user-sign-out-failed}

[請參閱下文](#failed)

### Adobe ID建立失敗 {#adobe-id-creation-failed}

[請參閱下文](#failed)

### 失敗 {#failed}

**根本原因**：這些錯誤可能是由於後端中的各種原因所造成。

**解析度**：

提交支援案例，包含[Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}的相關詳細資料。
