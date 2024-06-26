---
description: 最新發行說明 - Marketo 文件 - 產品文件
title: 最新發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: ea9bf2a002415936cdfb5bfb723ce80723003da5
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 2%

---

# 發行說明： 2024年7月 {#release-notes-july-24}

下方提供2024年6月發行版本包含的所有功能。 檢查您的Adobe Marketo Engage版本是否有功能可用。

Adobe Dynamic Chat專屬發行說明 [可在此處找到](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>以星號(![星形](assets/yellow-star.png))為付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於以下日期開始發行 **2024年7月26日**，在接下來的幾週內分階段推出剩餘的功能。 發行功能和日期可能會有所變更。 請檢查每個功能旁的狀態。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">狀態</th>
   <th style="width:25%">檔案</th>
  </tr>
     <tr> 
   <td><strong>Marketo REST API變更</strong>：我們即將推出微幅變更 <a href="https://developers.marketo.com/rest-api/user-management/">使用者管理API</a>. 兩者 <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">瀏覽使用者</a> 和 <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">刪除使用者</a> 端點現在支援 <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">目標帳戶管理</a> 使用者。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **新的開發人員檔案網站**：為了持續改善Marketo Engage使用者體驗，我們將於2024年7月將所有開發人員檔案移轉至Adobe Experience League和Adobe Developer網站。 [瞭解更多](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **存取查詢引數中的權杖淘汰**：在未來版本中，將移除對Marketo EngageREST API呼叫的查詢引數中使用存取權杖的驗證支援（特定日期待定）。 現有的整合應移轉至授權標頭的使用 [此處說明](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. 新開發應僅使用Authorization標頭進行Marketo Engage驗證。

* **需要重新驗證LinkedIn**：LinkedIn正在升級Marketo EngageLinkedIn整合所使用的行銷API。 這些變更需要重新驗證您電腦中的所有LinkedIn LaunchPoint服務 **管理員** > **啟動點** 2024年7月26日至12月15日期間的功能表，以避免服務中斷。 您可以找到如何完成此作業的指示 [此處取得Forms銷售機會總管](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} 和 [以取得相符的對象](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. Lead Gen Form服務的型別為「LinkedIn Lead Gen」，而Matched Audience服務的型別為「LinkedIn Matched Audiences」。 如需詳細資訊，請參閱 [移轉常見問題集](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
