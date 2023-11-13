---
description: 瞭解Marketo訂閱和使用者移轉至Adobe Admin Console - Marketo檔案 — 產品檔案
title: 瞭解Marketo訂閱和使用者移轉至Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: 094a11f9544e0dba75167de229d78e8ff50cf6e8
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 0%

---

# 瞭解Marketo訂閱和使用者移轉至Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe可強化您管理Adobe Marketo Engage訂閱和使用者的方式，為您和您的組織帶來更高的生產力。 作為此變更的一部分，Adobe正在將您的Marketo Engage訂閱和使用者移轉至Adobe Admin Console。 這是必要的移轉，不會影響任何行銷工作流程、內容、整合或資產。

瞭解如何使用Adobe Admin Console透過管理整個組織的Adobe權益 [企業和團隊管理指南](https://helpx.adobe.com/tw/enterprise/admin-guide.html){target="_blank"}.

## 有什麼改變？ {#what-is-changing}

移轉過程中，您的訂閱和使用者管理將從Marketo應用程式內移至Adobe Admin Console。

* **系統管理員將管理Adobe Admin Console上的訂閱**. 在一個主控台中檢視您的所有Adobe產品。

* **產品管理員將管理Adobe Admin Console的使用者及其存取權**. 新增和移除所有Adobe訂閱的使用者。

* **使用者將使用Adobe身分登入**. Adobe會將現有使用者移轉至Adobe Admin Console。 使用者將使用其新的Adobe身分登入其Marketo訂閱 — Adobe ID或AdobeFederated ID(SSO)。

* **您管理所有其他功能的方式不會變更** 在Marketo Engage應用程式本身中，包括功能、使用者角色、工作區、功能和行為的管理。

## 移轉歷程時間表 {#migration-journey-timeline}

Adobe會先將您的Marketo Engage訂閱移轉至Adobe Admin Console，然後移轉具有已驗證電子郵件地址的所有現有使用者。 如果您是系統管理員或Marketo產品管理員，您將會收到引導您完成移轉歷程的電子郵件。 以下是您可以期待的時間表：

### 訂閱移轉完成 {#subscription-migration-complete}

當訂閱移轉至Adobe Admin Console完成時，系統管理員將會收到電子郵件。

系統管理員可能需要在使用者移轉開始前完成一些必要步驟，以將對Marketo使用者的影響降至最低：

* 如果您的Marketo使用者目前是以SSO登入，您將需要在Adobe Admin Console上設定SSO，讓您的使用者可以繼續以SSO登入。 如果您的Marketo使用者目前未使用SSO，但您想要在Adobe Admin Console上加以設定，則可以在移轉歷程的此階段進行。

* 如果您已在Adobe Admin Console中管理其他Adobe產品，Adobe可能會要求您同意自動將使用者移轉至您現有的主控台。 按一下電子郵件中的「開始使用」按鈕以瀏覽至同意頁面。

目前使用者管理沒有變更。 Marketo管理員將繼續在Marketo管理區中管理使用者，而使用者將繼續使用其Marketo身分登入，直到完成其使用者移轉為止。

### 排程使用者移轉 {#schedule-user-migration}

系統管理員完成上一節所述的先決條件後，Adobe會自動排程提前30天移轉使用者，並與Marketo產品管理員溝通以管理使用者移轉。

Marketo產品管理員將：

* 在30天前收到含有其排程使用者移轉開始日期的電子郵件。

* 取得位於Marketo管理區域中的Marketo移轉主控台的存取權，使用者可選擇在此變更訂閱的移轉日期。

>[!NOTE]
>
>由於移轉的複雜性，日期變更限制在排定日期後30天內有效。 傳送電子郵件至 `marketocares@marketo.com` 如果您需要更晚的日期。

* 檢視「我的Marketo」中的橫幅，其中顯示「使用者移轉開始日期」的倒數計時。

* 在使用者移轉開始日期的前一天收到提醒電子郵件。

### 準備使用者進行移轉日 {#prepare-users-for-migration-day}

身為Marketo產品管理員，建議您確保所有使用者準備好進行移轉日作業。

* 檢查 [電子郵件驗證](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} Marketo管理區域中所有使用者的狀態。 鼓勵尚未驗證電子郵件地址的使用者進行驗證，並幫助使用者解決完成驗證流程時遇到的任何挑戰。

* 為所有使用者準備即將移轉至Adobe身分識別。

>[!NOTE]
>
>當使用者移轉時，他們會收到Adobe的電子郵件，通知他們登入Marketo的方式已變更。 使用者將獲邀接受邀請，以使用Adobe身分識別首次登入，方法為使用現有Adobe ID登入，或使用相同的電子郵件地址設定新帳戶。

>[!IMPORTANT]
>
>如果Marketo Engage使用者未驗證其電子郵件地址，則不會移轉至Adobe ID，而且會在移轉訂閱完成後無法存取Marketo訂閱。 若要重新取得存取權，Marketo產品管理員需要將使用者新增為新使用者。

### 移轉當天的期望 {#what-to-expect-on-migration-day}

所有採用美國時區的Marketo訂閱將會從移轉開始日期的太平洋標準時間午夜開始移轉。 所有其他訂閱的使用者移轉將於訂閱的指定時區午夜開始。

**Adobe將會先自動移轉Marketo管理員**. Marketo管理員移轉至Adobe身分識別後，將會在Marketo應用程式中獲得Adobe產品管理員角色，以及先前擁有的任何其他角色。

**如果您的Marketo訂閱使用者少於75名**，Adobe會自動移轉其餘的使用者。 此工作流程旨在提供最高等級的自動化，以儘量降低AdobeMarketo使用者的額外負荷。 您不需要採取任何動作即可執行移轉。

**如果您的Marketo訂閱有超過75位使用者**，Marketo產品管理員將可存取Marketo移轉主控台的「自助使用者移轉」區域(位於Marketo管理區域)。 若在使用者移轉程式期間需要加強控制，Marketo產品管理員將能一次選取或分批移轉的使用者。 選取使用者後，管理員可選取「立即移轉」或「排程移轉」以供稍後使用，讓管理員在移轉使用者時擁有最大的彈性和控制權。

>[!NOTE]
>
>使用者移轉期間，不會失去對產品的存取權。 如果使用者在其使用者移轉期間登入，則會在移轉完成後在幾分鐘內，使用Adobe身分識別提示使用者重新登入。

使用者移轉後，會收到Adobe的電子郵件，通知他們登入Marketo的方式有所變更。 使用者將獲邀接受邀請，以使用Adobe身分識別首次登入，方法為使用現有Adobe ID登入，或使用相同的電子郵件地址設定新的Adobe ID。

如需詳細資訊，請參閱 [使用Adobe登入的使用者](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"} and [Adobe Identity Management FAQ](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## 使用者移轉完成 {#user-migration-complete}

所有管理員和使用者遷移後，Adobe會透過電子郵件通知所有系統管理員和產品管理員。 此時，該訂閱的所有Marketo使用者都會使用Adobe身分登入Marketo，而產品管理員將僅管理Adobe Admin Console上的使用者。

## 取得支援 {#get-support}

如需訂閱或使用者移轉的其他相關支援，請傳送電子郵件至 `marketocares@marketo.com`.
