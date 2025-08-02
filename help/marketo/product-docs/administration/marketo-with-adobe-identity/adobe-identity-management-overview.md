---
description: Adobe Identity Management概觀 — Marketo檔案 — 產品檔案
title: Adobe Identity Management概觀
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Adobe Identity Management概觀 {#adobe-identity-management-overview}

所有新Adobe Marketo Engage訂閱（2023年7月31日或之後版本）都會與Adobe Identity Management系統整合。 現有的Marketo Engage訂閱目前正在任何銷售活動後移轉至Adobe Identity Management系統，包括續約、重新合約活動及/或增補專案。 自2024年10月起，支援銷售活動以外的移轉。 如果計畫將訂閱移轉至銷售活動以外，Marketo管理員將提前2-4週收到通知。

>[!NOTE]
>
>Marketo支援無法提供任何有關Adobe IMS移轉的更新。 Adobe客戶團隊將在未來幾個月提出預估時間表。 如需詳細資訊，請參閱[本文](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"}及[常見問題](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}。

對於加入Adobe身分識別的訂閱，Adobe Admin Console會用於使用者管理。 身分相關概念（例如單一登入）也可在Admin Console中管理。

* 尋找有關[Adobe Admin Console](https://helpx.adobe.com/tw/enterprise/using/admin-console.html){target="_blank"}的詳細資訊。
* 尋找與Marketo訂閱[相關的](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}設定Adobe組織的詳細資訊。

>[!NOTE]
>
>如果您想要實作單一登入，而且您的訂閱已上線到Adobe Identity而未在Adobe組織中實作SSO，請提交票證至[Marketo支援](https://nation.marketo.com/){target="_blank"}，並將主題指定為「在Admin Console上實作Marketo SSO」。

## 設定檔層級 {#profile-levels}

上線至Adobe Identity Management系統的Adobe Marketo Engage訂閱支援各種設定檔。 以下是與此整合相關的使用者設定檔型別。

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
  <td>負責管理產品設定檔中的使用者。 他們無法在該特定設定檔之外管理使用者。 產品設定檔管理員無法存取Marketo應用程式，除非以使用者身分新增至產品設定檔。 他們的角色仍將是標準使用者（如果有多個工作區，則為預設工作區）。
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage管理員</strong></td>
  <td>獲授具有管理許可權之Marketo Engage存取許可權的人員。 已在Marketo Engage中授與角色，而非Adobe Admin Console （在<b>編輯使用者</b>強制回應視窗中顯示為「管理員」）。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage使用者</strong></td>
  <td>獲授Marketo Engage存取許可權的人員。 沒有管理許可權。</td>
 </tr>
</table>

## 常見問題集 {#faq}

常見問題集[可在此找到](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}。

>[!MORELIKETHIS]
>
>* [管理員設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [新增或移除產品管理員](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [新增或移除使用者](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
