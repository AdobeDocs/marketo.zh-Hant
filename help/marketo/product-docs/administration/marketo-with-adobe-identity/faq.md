---
description: Adobe Identity Management 常見問題集 — Marketo 文件 — 產品文件
title: Adobe Identity Management 常見問題集
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 95ed91736b7276dd7a5b9e09958c1f09832ae719
workflow-type: ht
source-wordcount: '1579'
ht-degree: 100%

---

# Adobe Identity Management 常見問題集 {#adobe-identity-management-faq}

**什麼是 Adobe Identity？**

Adobe Identity Management 系統包含三個元件。

* [!DNL Adobe Identity Service]：處理終端使用者的驗證與確認，包括同盟和執行階段單一登入 (SSO)。

* Adobe Admin Console：Admin Console 可提供用於管理整個組織 Adobe 權益的中央位置。其會處理使用者管理、雲端服務、桌面授權權益、同盟設定，並提供資料遺失防護安全性功能。

* Adobe User Management API (UMAPI)：可讓組織在 API 層級的 Adobe Admin Console 中管理企業使用者和權益。

**現有的 Marketo Engage 訂閱何時會和 IMS 整合？**

現有的 Marketo Engage 訂閱目前會在任何銷售事件發生時遷移到 Adob&#x200B;&#x200B;e IMS，包括續訂、重新簽約事件和/或增補條款。自 2024 年 10 月起，可支援銷售事件以外的遷移。

**遷移之後，Marketo Engage URL 是否將維持不變？**

不會。遷移後，URL 將會以下列格式顯示：`https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (XXX 代表 Munchkin ID，而 @tenantID 則來自您的 Adobe 組織)。

**為了準備 URL 變更，我們是否需要做什麼？**

是的。遷移完成後，Adobe Marketo Engage 的服務位置會由 experience.adobe.com 遷移至 Adobe Experience Cloud。您需要和 IT 團隊合作，將所有 Adobe 網域 [(在本文頂端)](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} 列入允許清單，以防止對 Marketo Engage 的存取中斷。

指向 engage-xx.marketo.com 網域上 Marketo Engage 資產的先前連結和書籤&#x200B;_將會_&#x200B;繼續運作。不過，您必須先登入正在瀏覽 URL 的 Marketo Engage 執行個體。例如，若要瀏覽至 Munchkin ID 為123-ABC-456 之執行個體中 Smart Campaign 的書籤，您必須先以 Munchkin ID 123-ABC-456 登入 Marketo Engage 執行個體。

雖然未規劃，但未來的開發工作可能會破壞此重新導向功能。為避免意外中斷，建議您儘早更新書籤。

**這是否適用於 SSO？**

是的。與 Adobe IMS 的整合可支援通用 ID 使用者和 SSO。SSO 現在由 Adobe IMS 驅動，並會在 Adobe Admin Console 中的組織層級設定。不過，Marketo Engage IdP 起始的支援與 Adobe SP 起始的支援有所不同 ([在這裡了解更多](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"})。如果您在遷移至 Admin Console 後需要有關 SSO 差異的說明，請和 [Adobe 客戶服務](https://helpx.adobe.com/tw/contact.html){target="_blank"}聯絡。

**Adobe 產品管理員和 Marketo Engage 管理員之間有何差異？**

* Adobe 產品管理員是 Marketo 平台的新角色。
* 系統已將 Adobe 產品管理員角色授予在 Adobe Admin Console 中新增為產品管理員的使用者
* Adobe 產品管理員是唯讀角色，無法從 Marketo Engage 進行編輯或刪除。
* Adobe 產品管理員擁有與標準 Marketo 管理員相同的權利和權限。
* Marketo Engage 管理員的角色仍為管理員，且該角色已授予 Marketo Engage 中的使用者。
* 只有具有 Marketo 預設管理員角色的使用者才會在 Admin Console 中獲指派為 Marketo 產品管理員。

**User Management API 用戶端支援是否有任何變更？**

是的。已加入 Adobe IMS 的使用者無法利用所有現有的 Marketo User Management API。若是使用者邀請、更新及刪除動作，則應使用 Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"}。若是角色管理，則仍會套用 Marketo User Management API。除此之外，Marketo REST API 用戶端支援沒有其他任何變更。

**如果我們已和 IMS 整合，我們應和誰聯絡來尋求支援？**

* 使用者遷移前：請在 [Marketing Nation 社群](https://nation.marketo.com/t5/support/ct-p/Support)中提交支援案例或寄送電子郵件至 `customercare@marketo.com`。

* 使用者遷移後：請在 [Marketing Nation 社群](https://nation.marketo.com/t5/support/ct-p/Support)中提交支援案例或寄送電子郵件至 `customercare@marketo.com`。

* 支援遷移完成後：產品支援管理員可透過 Experience League 支援入口網站提交案例。

如果您有 Ultimate Success，即可存取 Admin Console 遷移白手套服務。請聯繫 Adobe 客戶團隊 (您的客戶經理) 以尋求協助。

**如果我使用 Adobe Identity 來存取其他 Adobe 應用程式，是否可將其用於存取 Marketo？**

即使您擁有其他 Adobe 產品，除非將訂閱遷移至 IMS，否則您無法使用 Adobe Identity 來存取 Marketo。

**Marketo 使用者角色 (在工作區內) 是否在 Adobe Admin Console 中進行管理？**

否。使用者角色管理 (在工作區內) 會在 Marketo Engage 中完成。

**我是 IMS 整合式訂閱的 Marketo 管理員，無法存取 Admin Console。我要如何取得存取權？**

擁有對貴組織之 Admin Console 的存取權的任何 Adobe 系統或產品管理員都可授予您存取權。如果不確定組織內誰擁有主控台的管理員權限，請和 [Adobe 客戶服務](https://helpx.adobe.com/tw/contact.html){target="_blank"}聯絡。

**管理員如何將使用者新增至 Marketo[!DNL Sales Connect]？**

雖然在 Admin Console 中有[!DNL Sales Connect]的產品卡，但 Admin Console 不應用於新增/管理使用者。下列連結可讓管理員透過 Marketo [!DNL Sales Connect]管理使用者：[https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}。

**我可以在何處了解更多 Adobe Admin Console 的資訊？**

[https://helpx.adobe.com/tw/enterprise/admin-guide.html](https://helpx.adobe.com/tw/enterprise/admin-guide.html){target="_blank"}。

**我是否仍需前往 Marketo 中的「管理員」區段，為我的帳戶變更使用者帳戶？**

否，您需瀏覽至 [account.adobe.com](https://account.adobe.com){target="_blank"}。

**這如何與 Marketo 的通用 ID 搭配運作？**

已加入 Adobe Identity 的使用者可透過產品中的訂閱切換器無縫存取所有 IMS 啟用訂閱。

**這是否適用於 SSO？**

是的。與 Adobe IMS 的 Marketo 整合可支援通用 ID 使用者和 SSO。SSO 現在由 Adobe IMS 驅動，並會在 Adobe Admin Console 中的組織層級設定。[若要了解更多資訊，請參閱此處](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}。

**我已經加入 Adobe Identity，現在想要實作 SSO。我該如何處理？**

如果您想要實作單一登入，而且您的訂閱已加入 Adobe Identity，但在 Adobe 組織中未實作 SSO，請提交票證至 [Marketo 支援](https://nation.marketo.com/){target="_blank"}，並將主題指定為「Admin Console 上的 Marketo，實作 SSO」。

**裝置授權如何運作？**

Adobe IMS 目前不支援 Marketo 的裝置授權功能之類的功能。

**是否仍可使用「在邀請使用者對話框中登入」功能，讓使用者的登入在其電子郵件中變成唯一？**

否。訂閱為 IMS 啟用時，使用者邀請工作流程即不再處於使用中狀態，因此功能也不再有效。Adobe Identity 要求以使用者的電子郵件作為使用者的身分識別依據。

**若是 Adobe IMS，我們是否可選擇使用 Adobe ID、Enterprise ID 或 Federated ID？**

是的，您可以決定要獲得組織支援的身分識別類型。如需更多資訊，請參閱這裡：[身分識別概觀](https://helpx.adobe.com/tw/enterprise/using/identity.html)以及這裡：[設定身分識別](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}。

**Adobe Admin Console 支援哪些產品卡？**

支援的產品卡包括：Marketo Engage、Marketo Measure、Marketo Dynamic Chat、Marketo Sales Connect 和 Marketo Sales Insight Actions。

**如果我遷移至 Adobe Identity 時，我的使用者登入與電子郵件不相符，該怎麼辦？**

目前的 Marketo Engage 使用者如果以其電子郵件地址以外的資訊登入，在遷移至 Adobe Identity 後，將不再使用該認證登入。Adobe 身分識別一律使用使用者的電子郵件地址進行驗證。您可以在 [account.adobe.com](https://account.adobe.com){target="_blank"} 更新 Adobe 身分識別電子郵件地址。

**如果我的訂閱使用 IP 限制設定，Adobe Identity 遷移後會發生什麼事？**

您目前的 IP 限制在 2026 年第 1 季度會維持使用中狀態 (這適用於在遷移前已啟用這些 IP 限制的訂閱)。這些限制也會套用至 Adobe ID 使用者，因此您的存取控制可繼續如預期般運作。

自 2026 年第 1 季度起，舊版 IP 限制將遭淘汰。從此以後，IP 型存取將完全在 Adobe Admin Console (AAC) 中進行管理。為了維護安全存取，您需要在 AAC 中設定 IP 限制。如需詳細資訊，請參閱這篇 [Marketing Nation 部落格文章](https://nation.marketo.com/t5/product-blogs/updated-important-update-ip-restrictions-feature-transition/ba-p/358420){target="_blank"}。

**如果我的使用者可選擇「繞過單一登入」，Adobe Identity 遷移後會發生什麼情況？**

Adobe Admin Console 會隨附預設的 Business ID 目錄。在 Adobe 組織的 Federated ID 目錄中所宣告之網域以外的使用者會被指派至此目錄，並屬於 Adobe ID 身分識別類型。這些使用者無需透過單一登入 (SSO) 即可存取 Marketo Engage，而授權所有權仍屬於公司而非個人。

**我有多個訂閱，但並非所有訂閱都已啟用「單一登入」。Adobe Identity 遷移後會發生什麼情況？**

當訂閱加入 Adobe Identity 時，系統會在 Adobe 組織層級設定單一登入 (SSO)。這表示 SSO 會套用至 Adobe 組織中的所有產品執行個體。SSO 設定完成後，將套用至該 Adobe 組織中的所有 Marketo 執行個體。過去，Marketo 僅在執行個體層級支援此設定。Adobe Identity Management 系統不支援此功能。

**Adobe Identity 遷移後，我們是否需要對目前用於 Marketo Engage 的 CNAME、SPF 或 DKIM 進行任何變更？**

否，這些設定不受影響。

**如何才能防止工作階段逾時？**

在[進階設定](https://helpx.adobe.com/tw/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}中，您可以自訂想要的工作階段時限最大值 (需要系統管理員權限)。建議您在產品遷移後、使用者遷移前建立此設定。

**我現在必須瀏覽至 Experience Cloud 才能存取 Marketo Engage。是否能簡化此流程？**

可以。您可以在瀏覽器中建立書籤，將在 Marketo Engage 執行個體入口頁面上按一下&#x200B;**「啟動」**&#x200B;按鈕後所開啟的連結加入書籤，以後即可繞過該頁面。

![](assets/faq-1.png)
