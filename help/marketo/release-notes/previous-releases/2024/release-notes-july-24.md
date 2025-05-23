---
description: 發行說明 — 2024年7月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2024 年 7 月
feature: Release Information
source-git-commit: 9087709e0572687b80022b73a1fde0dca8dc1a7e
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 3%

---

# 發行說明： 2024年7月 {#release-notes-july-24}

以下是2024年7月發行版本包含的所有功能。 檢查您的Adobe Marketo Engage版本是否有功能可用。

您可以在[&#128279;](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}找到專為Adobe Dynamic Chat的發行說明。

>[!AVAILABILITY]
>
>以星號（![星號](assets/yellow-star.png)）表示的功能是付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2024年7月26日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行功能和日期可能會有所變更。 請檢查每個功能旁的狀態。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">狀態</th>
   <th style="width:25%">檔案</th>
  </tr>
     <tr> 
   <td><strong>互動式網路研討會的參與儀表板</strong>：取得網路研討會效能檢視彙總，以及網路研討會期間每位與會者參與情況的完整檢視，以便您可以透過Marketo Engage協調工具決定要鎖定哪些潛在客戶。</td> 
    <td>已送出</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/engagement-dashboard.md" target="_blank">參與儀表板</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>互動式網路研討會的會議室管理</strong>：存取已建立的個別會議室（並視需要進行修改），以及存取內容與錄製（並視需要將其清除，以最佳化儲存空間）。</td> 
    <td>已送出</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/room-management.md" target="_blank">房間管理</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>互動式網路研討會自訂</strong>：透過使用公共會議室介面、中間熒幕（例如與會者入門熒幕背景）以及自訂視訊背景，提供統一的組織核准品牌體驗，讓網路研討會策略更容易與品牌策略保持一致。</td> 
    <td>已送出</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/customization.md" target="_blank">互動式網路研討會自訂</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Marketo REST API變更</strong>：我們即將對<a href="https://developers.marketo.com/rest-api/user-management/">使用者管理API</a>進行微幅變更。 <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">瀏覽使用者</a>和<a href="https://developers.marketo.com/rest-api/user-management/#delete_user">刪除使用者</a>端點現在都支援<a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">目標帳戶管理</a>使用者。</td> 
   <td>已送出</td>
   <td>不適用</td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **新的開發人員檔案網站**：為了持續改善Marketo Engage的使用者體驗，我們將在2024年7月將所有開發人員檔案移轉至Adobe Experience League和Adobe Developer網站。 [了解更多](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **棄用社交功能**： 2024年7月31日星期三，Marketo Engage將開始棄用產品中的下列社交功能：

   * 投票
   * 社交按鈕
   * 推薦人特賣優惠
   * 影片分享
   * 抽獎

使用者將無法再在Marketo Engage中建立、複製或嵌入任何社交功能。 現有的社交資產將持續運作至2025年1月31日。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **查詢引數棄用中的存取權杖**：未來版本將移除在Marketo EngageREST API呼叫的查詢引數中使用存取權杖的驗證支援（特定日期待定）。 現有的整合應該移轉至此處[&#128279;](https://developers.marketo.com/rest-api/authentication/){target="_blank"}說明的Authorization標頭的使用。 新開發應僅使用Authorization標頭進行Marketo Engage驗證。

* **需要重新驗證LinkedIn**： LinkedIn正在升級Marketo EngageLinkedIn整合所使用的行銷API。 這些變更需要在2024年7月26日至12月15日期間，重新驗證您&#x200B;**管理員** > **LaunchPoint**&#x200B;功能表中的所有LinkedIn LaunchPoint服務，以避免服務中斷。 您可以在[這裡找到有關Forms銷售機會主管](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"}如何完成此專案的指示，以及在[這裡找到相符對象](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}的說明。 Lead Gen Form服務的型別為「LinkedIn Lead Gen」，而Matched Audience服務的型別為「LinkedIn Matched Audiences」。 如需詳細資訊，請瀏覽[移轉常見問題集](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}。
