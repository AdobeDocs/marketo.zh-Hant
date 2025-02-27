---
description: Adobe IMS疑難排解指南 — Marketo檔案 — 產品檔案
title: Adobe IMS疑難排解指南
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e5c6ac7df0f8f6e7726de1ced598d390a6cf1deb
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Adobe IMS疑難排解指南 {#adobe-ims-troubleshooting-guide}

在IMS使用者移轉程式中，會為每個要移轉的Adobe使用者建立一個Marketo Engage使用者。 有時不會建立它（由於各種原因，如使用者在Active Directory中的記錄或電子郵件地址問題）。 發生此情況時，Marketo Engage管理員會在自行移轉主控台的使用者移轉狀態列位中檢視原因。 請參閱以下說明如何解決各種Adobe使用者建立問題。

## 錯誤訊息 {#error-messages}

* <a href="#not-in-directory">不在目錄</a>中
* <a href="#gmail-invalid-character">Gmail無效的字元</a>
* <a href="#inactive-user">非使用中的使用者</a>
* <a href="#not-in-domain">不在網域</a>中
* <a href="#create-failure">建立失敗</a>
* <a href="#type2e-user-failure">Type2e使用者失敗</a>

<table>
<thead>
  <tr>
    <th style="width:20%">錯誤訊息</th>
    <th style="width:40%">根本原因</th>
    <th style="width:40%">解析度</th>
  </tr>
  </thead>
<tbody>
  <tr>
    <td><i><a id="not-in-directory">不在目錄中</a></i></td>
    <td>使用者不存在於Active Directory (AD)中。 對於任何已啟用AD同步的SSO組織，僅允許透過身分提供者(IdP)建立使用者。 因此，無法在使用者移轉期間透過Admin Console新增使用者。</td>
    <td>移轉 — 使用者需要以適當的許可權新增至Active Directory。 Marketo管理員可從移轉主控台為此使用者重新執行使用者移轉。 
    <br>不移轉 — Marketo管理員在移轉主控台中略過使用者。 若移轉或略過已說明所有使用者，就會顯示「移轉完成」按鈕。 按一下以結束使用者移轉程式。</td>
  </tr>
  <tr>
    <td><i><a id="gmail-invalid-character">Gmail無效字元</a></i></td>
    <td>根據Adobe的安全性原則，「。」 只有Gmail網域的電子郵件地址不允許和'+'符號  
    <br>非Gmail網域電子郵件地址中允許兩個特殊字元。 </td>
    <td>移轉 — 電子郵件地址需要在Marketo Engage中更新，以符合Adobe的安全性政策。 Marketo管理員可從移轉主控台為此使用者重新執行使用者移轉。<br>不移轉 — Marketo管理員在移轉主控台中略過使用者。 若移轉或略過已說明所有使用者，就會顯示「移轉完成」按鈕。 按一下以結束使用者移轉程式。</td>
  </tr>
  <tr>
    <td><i><a id="inactive-user">非作用中的使用者</a></i></td>
    <td>AD同步已啟用，使用者的同盟帳戶已存在，但處於非作用中/停用狀態。</td>
    <td>移轉 — 需要還原使用者的狀態和適當許可權。 Marketo管理員可從移轉主控台為此使用者重新執行使用者移轉。
    <br>不移轉 — Marketo管理員在移轉主控台中略過使用者。 若移轉或略過已說明所有使用者，就會顯示「移轉完成」按鈕。 按一下以結束使用者移轉程式。</td>
  </tr>
  <tr>
    <td><i><a id="not-in-domain">不在網域中</a></i></td>
    <td>Admin Console已啟用網域強制執行，但使用者電子郵件地址的網域不是允許的網域之一。 
    <br>在目錄層級設定網域執行原則。</td>
    <td>移轉 — 電子郵件地址需要在Marketo Engage中更新以符合網域執行原則，或者系統管理員可以<a href="https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories"> 
    將網域移至另一個網域強制執行(DE)停用的目錄</a>或<a href="https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html">建立不在DE原則下的新目錄</a>。 Marketo管理員可從移轉主控台為此使用者重新執行使用者移轉。 <br>不移轉 — Marketo管理員在移轉主控台中略過使用者。 若移轉或略過已說明所有使用者，就會顯示「移轉完成」按鈕。 按一下以結束使用者移轉程式。</td>
  </tr>
  <tr>
    <td><i><a id="create-failure">建立失敗</a></i></td>
    <td>後端有各種原因。</td>
    <td>請提交支援案例。</td>
  </tr>
  <tr>
    <td><i><a id="type2e-user-failure">Type2e使用者失敗</a></i></td>
    <td>後端有各種原因。</td>
    <td>請提交支援案例。</td>
  </tr>
</tbody>
</table>
