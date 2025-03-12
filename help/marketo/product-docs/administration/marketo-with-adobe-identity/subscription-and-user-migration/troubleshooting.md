---
description: Adobe IMS使用者移轉疑難排解指南 — Marketo檔案 — 產品檔案
title: Adobe IMS使用者移轉疑難排解指南
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e96bc8676a73694ec60f46bb045f2a6ea5d8069c
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Adobe IMS使用者移轉疑難排解指南 {#adobe-ims-user-migration-troubleshooting-guide}

在IMS使用者移轉程式中，會針對每個要移轉的Adobe使用者建立一個Marketo Engage使用者（除非該使用者已存在相同電子郵件地址）。 有時不會建立它，這可能歸因於使用者在Active Directory中的記錄或電子郵件地址有問題。 發生此情況時，Marketo Engage管理員會在自行移轉主控台中的使用者移轉狀態列位中看到原因。

## 錯誤訊息 {#error-messages}

首先，判斷使用者是否需要移轉，因為這將影響要遵循的解決步驟。

使用右側的「在此頁面上」區段，直接跳至特定錯誤。

### 不在目錄中 {#not-in-directory}

**根本原因**：使用者不存在於Active Directory (AD)中。 對於已啟用AD同步的SSO組織，僅允許透過身分提供者(IdP)建立使用者。 因此，無法在使用者移轉期間透過Admin Console新增使用者。

**解析度**：

_如果使用者不需要移轉_ - Marketo Engage管理員在移轉主控台中略過該使用者。 「移轉完成」按鈕會在移轉或略過以說明所有使用者時出現。 按一下按鈕，結束使用者移轉程式。

_如果使用者確實需要移轉_ — 系統管理員必須將該使用者新增到Active Directory，並擁有適當的許可權。 Marketo Engage管理員，接著從移轉控制檯為此使用者重新執行使用者移轉。

### Gmail無效字元 {#gmail-invalid-character}

**根本原因**：根據Adobe安全性原則，Gmail電子郵件地址中不允許字元`.`和`+`。 非Gmail電子郵件地址中允許使用這兩個字元。

**解析度**：

_如果使用者不需要移轉_ - Marketo Engage管理員在移轉主控台中略過該使用者。 「移轉完成」按鈕會在移轉或略過以說明所有使用者時出現。 按一下按鈕，結束使用者移轉程式。

_如果使用者確實需要移轉_ — 電子郵件地址必須在Marketo Engage中更新，以符合Adobe的安全性原則並復原。 Marketo管理員，接著從移轉控制檯為此使用者重新執行使用者移轉。

### 非作用中的使用者 {#inactive-user}

**根本原因**： AD同步已啟用，而且使用者的同盟帳戶存在，但處於非作用中/停用狀態。

**解析度**：

_如果使用者不需要移轉_ - Marketo Engage管理員在移轉主控台中略過該使用者。 「移轉完成」按鈕會在移轉或略過以說明所有使用者時出現。 按一下按鈕，結束使用者移轉程式。

_如果使用者確實需要移轉_ — 必須還原使用者的狀態和適當的許可權。 Marketo Engage管理員，接著從移轉控制檯為此使用者重新執行使用者移轉。

### 不在網域中 {#not-in-domain}

**根本原因**：已在Admin Console中啟用網域強制執行，但使用者電子郵件地址的網域不是允許的網域之一。

**解析度**：

_如果使用者不需要移轉_ - Marketo Engage管理員在移轉主控台中略過該使用者。 「移轉完成」按鈕會在移轉或略過以說明所有使用者時出現。 按一下按鈕，結束使用者移轉程式。

_如果使用者確實需要移轉_ — 電子郵件地址必須在Marketo Engage中更新以符合網域強制(DE)原則。 或者，系統管理員可以[將網域](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"}移至另一個已停用的網域強制執行(DE)目錄，或[建立不在DE原則下的新目錄](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}。 Marketo Engage管理員，接著從移轉控制檯為此使用者重新執行使用者移轉。

### 建立失敗 {#create-failure}

**根本原因**：這個錯誤可能是由後端中的各種原因所造成。

**解析度**：

提交支援案例，包含[Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}的相關詳細資料。

### Type2e使用者失敗 {#type2e-user-failure}

**根本原因**：這個錯誤可能是由後端中的各種原因所造成。

**解析度**：

提交支援案例，包含[Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}的相關詳細資料。
