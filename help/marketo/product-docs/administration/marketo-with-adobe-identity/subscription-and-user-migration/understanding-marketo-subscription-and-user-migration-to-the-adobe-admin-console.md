---
description: 瞭解Marketo訂閱和使用者移轉至Adobe Admin Console - Marketo檔案 — 產品檔案
title: 瞭解Marketo訂閱和使用者移轉至Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: d6cf2b994f56a0fa4f2118fb3da3fd874644d8ae
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 0%

---

# 瞭解Marketo訂閱和使用者移轉至Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe正在改善您管理Adobe Marketo Engage訂閱和使用者的方式，為您和您的組織帶來更高的生產力。 作為此變更的一部分，Adobe正在將您的Marketo Engage訂閱和使用者移轉至Adobe Admin Console。 這是必要的移轉，不會影響任何行銷工作流程、內容、整合或資產。

>[!TIP]
>
>透過[企業和團隊管理指南](https://helpx.adobe.com/tw/enterprise/admin-guide.html){target="_blank"}，瞭解如何使用Adobe Admin Console在整個組織中管理您的Adobe權益。

## 有什麼改變？ {#what-is-changing}

移轉過程中，您的訂閱和使用者管理將從Marketo應用程式內移至Adobe Admin Console。

* **系統管理員將會在Adobe Admin Console**&#x200B;上管理訂閱。 在一個主控台中檢視您的所有Adobe產品。

* **產品管理員將會在Adobe Admin Console**&#x200B;上管理使用者及其存取權。 新增和移除所有Adobe訂閱的使用者。 Adobe Admin Console不支援以使用者為基礎的存取到期機制。 如果使用者擁有排定在移轉後到期的Marketo Engage存取權，仍會移轉並授予不會到期的存取權。 移轉後，必須在所要的到期日（或之前）手動移除這些專案。

* **使用者將使用Adobe身分識別登入**。 Adobe會將現有使用者移轉至Adobe Admin Console。 使用者將使用新的Adobe Identity (Adobe ID或Adobe Federated ID (SSO))登入其Marketo訂閱。

* 移轉後&#x200B;**個URL看起來會不同**。 移轉後，Marketo Engage會從experience.adobe.com改用Adobe Experience Cloud。 您必須與IT團隊合作，將所有Adobe網域加入允許清單（列於本文頂端[） ](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"}，以防止對Marketo Engage存取的中斷。

資產的ID號碼維持不變。 而且engage-xx.marketo.com網域&#x200B;_上Marketo Engage資產的先前連結和書籤將會_&#x200B;繼續運作。 不過，您必須先登入要導覽至的URL的Marketo Engage執行個體。 例如，若要導覽至Munchkin ID為123-ABC-456之執行個體中Smart Campaign的書籤，您必須先以Munchkin ID 123-ABC-456登入Marketo Engage執行個體。

## 哪些部分沒有改變？ {#what-is-not-changing}

* **您管理Marketo Engage應用程式本身所有其他功能的方式並無改變**，包括功能、使用者角色、工作區、功能及行為的管理。

## 移轉歷程時間表 {#migration-journey-timeline}

Adobe會先將您的Marketo Engage訂閱移轉至Adobe Admin Console，然後移轉具有已驗證電子郵件地址的所有現有使用者。 如果您是系統管理員或Marketo產品管理員，您將會收到引導您完成移轉歷程的電子郵件。 以下是您可以期待的時間表：

![](assets/understanding-marketo-subscription-and-user-migration-1.png){width="800" zoomable="yes"}

### 訂閱移轉完成 {#subscription-migration-complete}

當訂閱移轉至Adobe Admin Console完成時，系統管理員將會收到電子郵件。

系統管理員可能需要在使用者移轉開始前完成一些必要步驟，以將對Marketo使用者的影響降至最低：

* 如果您的Marketo使用者目前是以SSO登入，您將需要在Adobe Admin Console上設定SSO，讓您的使用者可以繼續以SSO登入。 如果您的Marketo使用者目前未使用SSO，但您想要在Adobe Admin Console上加以設定，則可以在移轉歷程的此階段進行。

* 如果您已在您的Adobe Admin Console中管理其他Adobe產品，Adobe可能會尋求您的同意，以自動將使用者移轉至您現有的主控台。 按一下電子郵件中的「開始使用」按鈕以瀏覽至同意頁面。

目前使用者管理沒有變更。 雖然Marketo產品會顯示在Admin Console中，但Marketo管理員仍會繼續在Marketo管理員區域中管理使用者，而且使用者將繼續使用其Marketo身分登入，直到完成使用者移轉為止。 在此期間，在使用者開始移轉之前，無法在Admin Console中管理Marketo產品。 其中包括與訂閱相關聯的Dynamic Chat執行個體。

>[!NOTE]
>
>如果您目前未使用SSO，但考慮實施，我們建議在使用者移轉發生之前實施。 如果您想要實作單一登入，而且您的訂閱已上線到Adobe Identity而未在Adobe組織中實作SSO，請向[Marketo支援](https://nation.marketo.com/){target="_blank"}提交票證，並將主題指定為「在Admin Console上實作Marketo SSO」。

### 排程使用者移轉 {#schedule-user-migration}

系統管理員完成上一節所述的先決條件後，Adobe會自動排程您的使用者提前30天移轉，並與Marketo產品管理員溝通以管理使用者移轉。

Marketo產品管理員將：

* 在30天前收到含有其排程使用者移轉開始日期的電子郵件。

* 取得位於Marketo管理區域中的Marketo移轉主控台的存取權，使用者可選擇在此變更訂閱的移轉日期。

>[!NOTE]
>
>由於移轉的複雜性，日期變更限制在排定日期後30天內有效。 如果您需要較晚的日期，請傳送電子郵件給`marketocares@marketo.com`。

* 檢視「我的Marketo」中的橫幅，其中顯示「使用者移轉開始日期」的倒數計時。

* 在使用者移轉開始日期的前一天收到提醒電子郵件。

### 準備使用者進行移轉日 {#prepare-users-for-migration-day}

身為Marketo產品管理員，建議您確保所有使用者準備好進行移轉日作業。

* 檢查Marketo管理區域中所有使用者的[電子郵件驗證](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"}狀態。 鼓勵尚未驗證電子郵件地址的使用者進行驗證，並幫助使用者解決完成驗證流程時遇到的任何挑戰。

* 搜尋您的電子郵件收件匣以尋找「已鎖定」的使用者通知。 建議已鎖定的使用者在移轉日之前重設密碼，以重新建立Marketo Engage的存取權。

* 為所有使用者準備即將移轉至Adobe Identity。

>[!IMPORTANT]
>
>如果Marketo Engage使用者未驗證其電子郵件地址，或在使用者移轉時鎖定，則不會移轉到Adobe ID，而且會在移轉訂閱完成後無法存取Marketo訂閱。 若要重新取得存取權，Marketo產品管理員需要將使用者新增為新使用者。

### 移轉當天的期望 {#what-to-expect-on-migration-day}

所有採用美國時區的Marketo訂閱將會從移轉開始日期的太平洋標準時間午夜開始移轉。 所有其他訂閱的使用者移轉將於訂閱的指定時區午夜開始。

**Adobe將會先自動移轉Marketo管理員**。 Marketo管理員移轉至Adobe Identity時，會在Marketo應用程式中獲得Adobe產品管理員角色，以及先前擁有的任何其他角色。

**如果您的Marketo訂閱使用者少於75名，且在Marketo和/或Adobe組織**&#x200B;中沒有SSO，Adobe會自動移轉其餘的使用者。 此工作流程旨在提供最高等級的自動化，以儘量降低Adobe Marketo使用者的額外負荷。 您不需要採取任何動作即可執行移轉。

**如果您的Marketo訂閱擁有超過75名使用者，或在Marketo和/或Adobe組織**&#x200B;中擁有SSO，Marketo產品管理員將可存取Marketo管理區域內Marketo移轉主控台的「自助使用者移轉」區域。 若在使用者移轉程式期間需要加強控制，Marketo產品管理員將能一次選取或分批移轉的使用者。 選取使用者後，管理員可選取「立即移轉」或「排程移轉」以供稍後使用，讓管理員在移轉使用者時擁有最大的彈性和控制權。

>[!NOTE]
>
>使用者移轉期間，不會失去對產品的存取權。 如果使用者在其使用者移轉期間登入，則會在移轉完成後在幾分鐘內，使用Adobe身分識別提示使用者重新登入。 使用者必須在成功的使用者移轉結束時，按一下軟體權利檔案電子郵件中的連結，以接受邀請。

使用者移轉後，會收到Adobe的電子郵件，通知使用者已變更Marketo登入方式。 使用者&#x200B;**必須**&#x200B;接受第一次使用Adobe身分登入的邀請，方法是使用現有的Adobe ID登入，或使用相同的電子郵件地址設定新的Adobe ID。

如需詳細資訊，請參閱[移轉至Adobe身分識別](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}、[使用Adobe登入的使用者](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}以及[Adobe Identity Management常見問題集](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}。

## 使用者移轉完成 {#user-migration-complete}

所有管理員和使用者完成移轉後，Adobe會透過電子郵件通知所有系統管理員和產品管理員。 此時，該訂閱的所有Marketo使用者都會使用Adobe身分登入Marketo，而產品管理員僅能在Adobe Admin Console上管理使用者。

## 取得支援 {#get-support}

如需有關您的訂閱或使用者移轉的其他支援，請傳送電子郵件至`marketocares@marketo.com`。

>[!MORELIKETHIS]
>
>* [移轉至Adobe身分識別總覽](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [使用Adobe登入的使用者](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [Adobe Identity Management常見問題集](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
>* [移轉至Adobe Identity Management教學課程](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/fundamentals/migrating-to-adobe-identity-management){target="_blank"}
