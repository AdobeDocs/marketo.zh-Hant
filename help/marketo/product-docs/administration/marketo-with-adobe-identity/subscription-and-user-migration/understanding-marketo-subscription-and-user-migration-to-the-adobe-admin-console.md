---
description: 了解 Marketo 訂閱和使用者遷移至 Adobe Admin Console - Marketo 文件 - 產品文件
title: 了解 Marketo 訂閱和使用者遷移至 Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '1571'
ht-degree: 100%

---

# 了解 Marketo 訂閱和使用者遷移至 Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe 正在增強您管理 Adobe Marketo Engage 訂閱和使用者的方式，為您和貴組織實現更高的生產力。作為此變更的一部分，Adobe 正在將您的 Marketo Engage 訂閱與使用者遷移至 Adobe Admin Console。這是必要的遷移，並且不會影響任何行銷工作流程、內容、整合或資產。

>[!TIP]
>
>透過[企業與團隊管理指南](https://helpx.adobe.com/tw/enterprise/admin-guide.html){target="_blank"}了解如何使用 Adobe Admin Console 來管理整個組織的 Adobe 權益。

## 會有哪些變更？ {#what-is-changing}

遷移過程中，您的訂閱和使用者管理會從 Marketo 應用程式內搬移至 Adobe Admin Console。

* **系統管理員將會在 Adobe Admin Console 中管理訂閱**。在一個主控台中即可查看您的所有 Adobe 產品。

* **產品管理員將會在 Adobe Admin Console 中管理使用者及其存取權**。新增和移除所有 Adobe 訂閱的使用者。Adobe Admin Console 不支援根據使用者設定的存取過期機制。使用者如果擁有預定在遷移後到期的 Marketo Engage 存取權，仍會被遷移並獲授予不會過期的存取權。遷移後，必須在想要的過期日 (或之前) 手動進行移除。

* **使用者將使用 Adobe Identity 登入**。Adobe 會將現有的使用者遷移至 Adobe Admin Console。使用者將使用新的 Adobe Identity (Adobe ID 或 Adobe Federated ID (SSO)) 登入其 Marketo 訂閱。

* **遷移後，URL 會看起來不同**。Marketo Engage 將從 experience.adobe.com 遷移至 Adobe Experience Cloud，URL 會採用下列格式：`https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (XXX 代表 Munchkin ID，而 @tenantID 則來自您的 Adobe 組織)。您需要和 IT 團隊合作，將所有 Adobe 網域 [(在本文頂端)](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} 列入允許清單，以防止對 Marketo Engage 的存取中斷。

您的資產的 ID 號碼維持不變。而指向 engage-xx.marketo.com 網域上 Marketo Engage 資產的先前連結和書籤&#x200B;_將會_&#x200B;繼續運作。不過，您必須先登入正在瀏覽 URL 的 Marketo Engage 執行個體。例如，若要瀏覽至 Munchkin ID 為123-ABC-456 之執行個體中 Smart Campaign 的書籤，您必須先以 Munchkin ID 123-ABC-456 登入 Marketo Engage 執行個體。

雖然未規劃，但未來的開發工作可能會破壞此重新導向功能。為避免意外中斷，建議您儘早更新書籤。

## 哪些部分沒有變更？ {#what-is-not-changing}

* **您管理 Marketo Engage 應用程式內所有其他功能的方式則不會有任何改變**，包括對特性、使用者角色、工作區、功能及行為的管理。本機 (僅限 API) 使用者管理仍保留在 Marketo 管理區域的&#x200B;_使用者和角色_&#x200B;索引標籤中。

## 遷移歷程時間軸 {#migration-journey-timeline}

Adobe 會先將您的 Marketo Engage 訂閱遷移至 Adobe Admin Console，然後再遷移具有已驗證電子郵件地址的所有現有使用者。如果您是系統管理員或 Marketo 產品管理員，您將會收到引導您完成遷移歷程的電子郵件。以下是您可以期待的時間軸：

![](assets/understanding-marketo-subscription-and-user-migration-1.png){width="800" zoomable="yes"}

### 訂閱遷移完成 {#subscription-migration-complete}

訂閱遷移至 Adobe Admin Console 完成時，系統管理員即會收到電子郵件。

系統管理員可能需要在使用者遷移開始前完成一些必要步驟，以便將對 Marketo 使用者的影響降至最低：

* 如果您的 Marketo 使用者目前是使用 SSO 登入，您將需要在 Adobe Admin Console 設定 SSO，讓您的使用者可以繼續使用 SSO 登入。如果您的 Marketo 使用者目前未使用 SSO，但您想要在 Adobe Admin Console 進行設定，則可以在遷移歷程中的此階段進行。

* 如果您已在您的 Adobe Admin Console 中管理其他 Adobe 產品，Adobe 可能會尋求您的同意，以便將使用者自動遷移至您現有的主控台。按一下電子郵件中的「開始使用」按鈕，以瀏覽至同意頁面。

目前使用者管理沒有任何變更。雖然 Marketo 產品會顯示在 Admin Console 中，但 Marketo 管理員仍會繼續在 Marketo 管理員區域中管理使用者，而且使用者將繼續使用其 Marketo Identity 登入，直到完成使用者遷移為止。在此期間，直到使用者開始遷移前，都無法在 Admin Console 中管理 Marketo 產品。其中包括與訂閱相關聯的 Dynamic Chat 執行個體。

>[!NOTE]
>
>如果您目前未使用 SSO，但考慮進行實作，我們建議在使用者遷移發生前進行。如果您想要實作單一登入，而且您的訂閱已加入 Adobe Identity，但在 Adobe 組織中未實作 SSO，請提交票證至 [Marketo 支援](https://nation.marketo.com/){target="_blank"}，並將主題指定為「Admin Console 上的 Marketo，實作 SSO」。

### 排程使用者遷移 {#schedule-user-migration}

系統管理員完成上一節中所述的先決條件後，Adobe 就會自動在 30 天後排程您的使用者遷移，並和 Marketo 產品管理員溝通，以管理使用者遷移。

Marketo 產品管理員將：

* 在其排程使用者者遷移日期的 30 天 前收到電子郵件。

* 取得對位於 Marketo 管理區域中的 Marketo 遷移主控台的存取權，使用者可選擇在此變更訂閱的遷移日期。

>[!NOTE]
>
>由於遷移的複雜性，日期變更會限制為不得超過排程日期後的 30 天。如果您需要更晚的日期，請傳送電子郵件至 `marketocares@marketo.com`。

* 可查看「我的 Marketo」中的橫幅，其中會顯示「使用者遷移開始日期」的倒數計時。

* 在使用者遷移開始日期的前一天會收到提醒電子郵件。

### 為使用者準備好迎接遷移日 {#prepare-users-for-migration-day}

身為 Marketo 產品管理員，建議您確保所有使用者準備好迎接遷移日。

* 檢查 Marketo 管理區域中所有使用者的[電子郵件驗證](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"}狀態。鼓勵尚未完成其電子郵件地址驗證的使用者進行驗證，並協助使用者解決完成驗證流程時遇到的任何挑戰。

* 搜尋您的電子郵件收件匣以尋找「已鎖定」的使用者通知。建議已遭鎖定的使用者在遷移日之前重設密碼，以重新建立對 Marketo Engage 的存取權。

* 讓所有使用者準備好迎接即將進行的遷移至 Adobe Identity。

>[!IMPORTANT]
>
>如果 Marketo Engage 使用者未驗證其電子郵件地址，或在使用者遷移時遭鎖定，則不會遷移至 Adobe ID，而且在訂閱遷移完成後會失去對 Marketo 訂閱的存取權。若要重新取得存取權，Marketo 產品管理員需要將上述使用者新增為新使用者。

### 遷移日當天可能會發生什麼事 {#what-to-expect-on-migration-day}

所有採用美國時區的 Marketo 訂閱都會在遷移開始日期的太平洋標準時間午夜開始進行遷移。所有其他訂閱的使用者遷移將於訂閱指定時區的午夜開始。

**Adobe 會先自動遷移 Marketo 管理員 (具有標準管理員角色)**。當 Marketo 管理員遷移至 Adobe Identity (具有 Admin Console 產品管理員角色) 時，系統會在 Marketo 應用程式中為其指派 Adobe 產品管理員角色以及任何先前擁有的其他角色。

**如果您的 Marketo 訂閱在 Marketo 和/或 Adobe 組織**&#x200B;中都未使用 SSO，Adobe 會自動遷移您其餘的使用者。此工作流程旨在實現最高等級的自動化，以將 Adobe Marketo 使用者的負擔降至最低。您不需要採取任何動作即可執行遷移。

**如果您的 Marketo 訂閱在 Marketo 和/或 Adobe 組織中使用 SSO**，Marketo 管理員可取得對位於 Marketo 管理區域中 Marketo 遷移主控台的自助使用者遷移區域的存取權。對於在使用者遷移流程期間需要更大控制權的使用者，Marketo 管理員即可開始選取以批次方式遷移或一次性遷移所有使用者。選取使用者後，管理員可選擇「立即遷移」或在稍後日期的「排程遷移」，這讓管理員具有終極靈活度來控制要遷移的使用者及遷移時間。

>[!NOTE]
>
>在使用者遷移期間，並不會失去對產品的存取權。如果使用者在其使用者遷移期間已登入，系統會將其登出，並在遷移完成後幾分鐘內提示使用者使用 Adobe Identity 重新登入。使用者必須在成功完成遷移後，按一下權益電子郵件中的連結來接受邀請。

使用者遷移後，他們會收到來自 Adobe 的電子郵件，通知其 Marketo 登入方式的變更。使用者&#x200B;**必須**&#x200B;在首次登入時接受邀請，並使用現有的 Adobe ID 登入，或使用相同的電子郵件地址來設定新的 Adobe ID。

如需詳細資訊，請參閱[遷移至 Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}、[使用者透過 Adobe ID 登入](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}以及[Adobe Identity Management 常見問題集](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}。

## 使用者遷移完成 {#user-migration-complete}

所有管理員和使用者完成遷移後，Adobe 會透過電子郵件通知所有系統管理員和產品管理員。此時，該訂閱的所有 Marketo 使用者都可使用 Adobe Identity 登入 Marketo，而產品管理員則只能在 Adobe Admin Console 中管理使用者。

## 取得支援 {#get-support}

如需有關您的訂閱或使用者遷移的其他支援，請傳送電子郵件至 `marketocares@marketo.com`。

>[!MORELIKETHIS]
>
>* [遷移至 Adobe Identity 概觀](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [使用者透過 Adobe ID 登入](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [Adobe Identity Management 常見問題集](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
>* [遷移至 Adobe Identity Management 教學課程](https://experienceleague.adobe.com/zh-hant/docs/marketo-learn/tutorials/fundamentals/migrating-to-adobe-identity-management){target="_blank"}
