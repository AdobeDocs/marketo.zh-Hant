---
description: 適用於Marketo Engage的Adobe Identity Management概觀，包括移轉時間、Admin Console使用者管理和設定檔層級，例如系統管理員和產品管理員。
title: Adobe Identity Management 概觀
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: c06481152e88b8760a4539842a91aea90ab07fa1
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 6%

---

# Adobe Identity Management 概觀 {#adobe-identity-management-overview}

所有新Adobe Marketo Engage訂閱（2023年7月31日或之後版本）都會與Adobe Identity Management系統整合。

對於加入Adobe身分識別的訂閱，Adobe Admin Console會用於使用者管理。 與身分識別相關的概念（例如單一登入）也可在Admin Console中管理。

* 尋找有關[Adobe Admin Console](https://helpx.adobe.com/tw/enterprise/using/admin-console.html){target="_blank"}的詳細資訊。
* 尋找與Marketo訂閱[&#128279;](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}相關的設定Adobe組織的詳細資訊。

>[!NOTE]
>
>如果您想要實作單一登入，而且您的訂閱已上線到Adobe Identity ，但未在Adobe組織中實作SSO，請提交票證至[Marketo支援](https://nation.marketo.com/){target="_blank"}，並將主題指定為「在Admin Console上實作Marketo SSO」。

## 設定檔層級 {#profile-levels}

加入Adobe Identity Management系統的Adobe Marketo Engage訂閱支援各種設定檔。 以下是與此整合相關的使用者設定檔型別。

<table>
 <tr>
  <td><strong>Adobe Admin Console系統管理員</strong></td>
  <td>負責在Adobe Admin Console中為Adobe組織和Marketo Engage產品設定身分概念。 在Adobe組織設定中授與的角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console產品管理員</strong></td>
  <td>負責在Adobe Admin Console中授與使用者Marketo Engage產品的許可權。 在Adobe Admin Console中授與的角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console產品設定檔管理員</strong></td>
  <td>負責管理產品設定檔中的使用者。 他們無法在該特定設定檔之外管理使用者。 產品設定檔管理員無法存取Marketo應用程式，除非以使用者身分新增至產品設定檔。 他們的角色仍會是標準使用者（如果有多個工作區，則為預設工作區）。
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage管理員</strong></td>
  <td>獲授具有管理許可權之Marketo Engage存取許可權的人員。 已授與Marketo Engage中的角色，而非Adobe Admin Console （在<b>編輯使用者</b>強制回應視窗中顯示為「管理員」）。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage使用者</strong></td>
  <td>獲授Marketo Engage存取許可權的人員。 沒有管理許可權。</td>
 </tr>
</table>

>[!MORELIKETHIS]
>
>* [管理員設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [新增或移除產品管理員](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-product-admin.md){target="_blank"}
>* [新增或移除使用者](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md){target="_blank"}
