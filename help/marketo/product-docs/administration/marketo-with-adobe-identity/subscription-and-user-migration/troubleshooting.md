---
description: Adobe IMS疑難排解指南 — Marketo檔案 — 產品檔案
title: Adobe IMS疑難排解指南
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: a2186f054e7b7a780098157927651a084e353bd8
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Adobe IMS疑難排解指南 {#adobe-ims-troubleshooting-guide}

在IMS使用者移轉程式中，會為每個要移轉的Adobe使用者建立一個Marketo Engage使用者。 有時不會建立它（由於各種原因，如使用者在Active Directory中的記錄或電子郵件地址問題）。 發生此情況時，Marketo Engage管理員會在自行移轉主控台上的使用者移轉狀態列位中看到原因。

## 錯誤訊息 {#error-messages}

使用右側的「在此頁面上」一節，直接跳至特定錯誤並瞭解如何解決它。

### 不在目錄中 {#not-in-directory}

_根本原因_：使用者不存在於Active Directory (AD)中。 對於已啟用AD同步的SSO組織，僅允許透過身分提供者(IdP)建立使用者。 因此，無法在使用者移轉期間透過Admin Console新增使用者。

_解析度_：

移轉前 — Marketo可在移轉控制檯中讓管理員略過使用者。 「移轉完成」按鈕會在移轉或略過以說明所有使用者時出現。 按一下按鈕，結束使用者移轉程式。

移轉後 — 必須將使用者新增到Active Directory，並擁有適當的許可權。 Marketo Engage管理員，接著從移轉主控台為此使用者重新執行使用者移轉。

### Gmail無效字元 {#gmail-invalid-character}

_根本原因_：根據Adobe安全性原則，Gmail電子郵件地址中不允許字元`.`和`+`。 這兩個字元僅允許在非Gmail電子郵件地址中使用。

_解析度_：

移轉前 — Marketo可在移轉控制檯中讓管理員略過使用者。 「移轉完成」按鈕會在移轉或略過以說明所有使用者時出現。 按一下按鈕，結束使用者移轉程式。

移轉後 — 電子郵件地址必須在Marketo Engage中更新，以符合Adobe的安全性政策。 Marketo管理員可從移轉主控台為此使用者重新執行使用者移轉。

### 非作用中的使用者 {#inactive-user}

_根本原因_： AD同步已啟用，而且使用者的同盟帳戶存在，但處於非作用中/停用狀態。

_解析度_：

移轉前 — Marketo可在移轉控制檯中讓管理員略過使用者。 「移轉完成」按鈕會在移轉或略過以說明所有使用者時出現。 按一下按鈕，結束使用者移轉程式。

移轉後 — 必須還原使用者的狀態和適當許可權。 Marketo Engage管理員，接著從移轉主控台為此使用者重新執行使用者移轉。

### 不在網域中 {#not-in-domain}

_根本原因_：已在Admin Console中啟用網域強制執行，但使用者電子郵件地址的網域不是允許的網域之一。

_解析度_：

移轉前 — Marketo可在移轉控制檯中讓管理員略過使用者。 「移轉完成」按鈕會在移轉或略過以說明所有使用者時出現。 按一下按鈕，結束使用者移轉程式。

移轉後 — 電子郵件地址必須在Marketo Engage中更新，以符合網域強制(DE)政策。 或者，系統管理員可以[將網域](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"}移至另一個已停用的網域強制執行(DE)目錄，或[建立不在DE原則下的新目錄](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}。 Marketo Engage管理員，接著從移轉主控台為此使用者重新執行使用者移轉。

### 建立失敗 {#create-failure}

_根本原因_：這個錯誤可能是由後端中的各種原因所造成。

_解析度_：

移轉前 — 請針對尚未移轉的[提交支援案例](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。

移轉後 — 請針對已移轉的[提交支援案例](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}。

### Type2e使用者失敗 {#type2e-user-failure}

_根本原因_：這個錯誤可能是由後端中的各種原因所造成。

_解析度_：

移轉前 — 請針對尚未移轉的[提交支援案例](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。

移轉後 — 請針對已移轉的[提交支援案例](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}。
