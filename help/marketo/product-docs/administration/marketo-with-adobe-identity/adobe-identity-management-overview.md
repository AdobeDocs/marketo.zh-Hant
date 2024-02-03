---
description: AdobeIdentity Management概觀 — Marketo檔案 — 產品檔案
title: AdobeIdentity Management概觀
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 6f9790c2243407f2622970d228c9de6be7697df6
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# AdobeIdentity Management概觀 {#adobe-identity-management-overview}

所有新Adobe Marketo Engage訂閱（2023年7月31日或以上）都與AdobeIdentity Management System整合。 現有的Marketo訂閱目前正在續約和/或重新合約事件時移轉至Adobe的Identity Management系統。 目前不支援續約或重新合約事件以外的移轉。

>[!NOTE]
>
>Marketo支援無法提供任何有關Adobe IMS移轉的更新。 Adobe客戶團隊將在未來幾個月提出預估時間表。 如需詳細資訊，請參閱 [本文](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"}, and the [Frequently Asked Questions](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

對於上架到Adobe身分的訂閱，Adobe Admin Console會用於使用者管理。 身分相關概念（例如單一登入）也會在Admin Console中管理。

* 尋找更多關於 [Adobe Admin Console](https://helpx.adobe.com/tw/enterprise/using/admin-console.html){target="_blank"}.
* 尋找更多關於以下內容的資訊： [設定與您的Marketo訂閱相關的Adobe組織](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>如果您想要實作單一登入，而且您的訂閱已上線到Adobe身分識別，而未在Adobe組織中實作SSO，請提交票證至 [Marketo支援](https://nation.marketo.com/){target="_blank"} 並將主題指定為「Admin Console上的Marketo，實作SSO」。

## 設定檔層級 {#profile-levels}

加入Identity Management系統Adobe的Adobe Marketo Engage訂閱支援各種設定檔。 以下是與此整合相關的使用者設定檔型別。

<table>
 <tr>
  <td><strong>Adobe Admin Console系統管理員</strong></td>
  <td>負責在Adobe Admin Console中為Adobe組織和Marketo Engage產品設定身分概念。 在Adobe組織設定時授與的角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console產品管理員</strong></td>
  <td>負責在Adobe Admin Console中授與使用者Marketo Engage產品的權利。 在Adobe Admin Console中授與的角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console產品設定檔管理員</strong></td>
  <td>負責管理產品設定檔中的使用者。 他們無法在該特定設定檔之外管理使用者。 產品設定檔管理員無法存取Marketo應用程式，除非以使用者身分新增至產品設定檔。 他們的角色仍將是標準使用者（如果有多個工作區，則為預設工作區）。
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage產品管理員</strong></td>
  <td>獲授具有管理許可權之Marketo Engage存取許可權的人員。 已在Marketo Engage中授與角色，而非Adobe Admin Console。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage使用者</strong></td>
  <td>獲授Marketo Engage存取許可權的人員。 沒有管理許可權。</td>
 </tr>
</table>

## 常見問題集 {#faq}

常見問題 [可在此處找到](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [管理員設定](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [新增或移除產品管理員](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [新增或移除使用者](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
