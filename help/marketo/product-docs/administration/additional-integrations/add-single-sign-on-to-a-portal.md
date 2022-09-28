---
unique-page-id: 2360356
description: 將單一登入新增至入口網站 — Marketo檔案 — 產品檔案
title: 將單一登入新增至入口網站
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
source-git-commit: 813bab6169a121e90919f9a02505ccde5167cda4
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# 將單一登入新增至入口網站 {#add-single-sign-on-to-a-portal}

如果您有驗證使用者的目錄服務，則可允許將單一登入(SSO)登入Marketo。 我們使用安全斷言標籤語言(SAML)2.0版及更新版本來支援此功能。

Marketo以SAML服務提供者(SP)的身分運作，且須仰賴外部身分提供者(IdP)來驗證使用者。

啟用SSO後，IdP就可以驗證使用者的憑證。 當使用者想要使用Marketo軟體時，IdP會傳送已簽署的SAML訊息給Marketo，充當SP。 此訊息為Marketo提供保險箱，讓使用者有權使用Marketo軟體。

>[!NOTE]
>
>**需要管理權限**

>[!NOTE]
>
>您是Microsoft Azure使用者嗎？ 看看他們的 [整合教學課程](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/){target=&quot;_blank&quot;}。

## 如何傳送請求 {#how-to-send-the-request}

* 將SSO要求（即SAML回應）傳送至 `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* 作為SP的對象URL。 使用 `http://saml.marketo.com/sp`
* 如果使用SPNameQualifier屬性，請將「主題」的NameID元素設定為 `http://saml.marketo.com/sp`
* 如果您將多個Marketo訂閱聯合到相同的SSO提供者，則可以使用格式為每個Marketo子訂閱使用唯一的SP URL `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo僅支援由身分提供者啟動（也稱為IdP啟動），使用者在此啟動中會先啟動Idp登入頁面、驗證，然後導覽至我的Marketo。

## 其他附註 {#additional-notes}

* **同步時間**  — 若為新使用者，處理初始SSO請求前大約會延遲10分鐘。
* **用戶布建**  — 使用者由Marketo手動布建。
* **授權**  — 使用者權限會在Marketo中維護。
* **OAuth支援** - Marketo目前不支援OAuth。
* **自動用戶傳播**  — 也稱為「準時布建」，是指使用者的首次SAML登入可在其存取的任何Web應用程式(例如Marketo)中建立使用者，且不需要手動管理動作時。 Marketo目前不支援此功能。
* **加密** - Marketo目前不支援加密。

>[!NOTE]
>
>開始之前，請以X.509格式和.crt、.der或.cer副檔名取得身分提供者憑證。

## 更新SAML設定 {#update-saml-settings}

預設會停用SSO。 請依照下列步驟來啟用SAML並加以設定。

1. 前往 **管理** 的上界。

   ![](assets/add-single-sign-on-to-a-portal-1.png)

1. 按一下 **單一登入**.

   ![](assets/add-single-sign-on-to-a-portal-2.png)

   >[!NOTE]
   >
   >如果你沒看到 **單一登入** 在 **管理**，聯絡 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support){target=&quot;_blank&quot;}。

1. 在 **SAML設定** ，按一下 **編輯**.

   ![](assets/add-single-sign-on-to-a-portal-3.png)

1. 變更 **SAML單一登入** to **已啟用**.

   ![](assets/add-single-sign-on-to-a-portal-4.png)

1. 輸入 **頒發者ID**, **實體ID**，請選取 **使用者ID位置**，然後按一下 **瀏覽**.

   ![](assets/add-single-sign-on-to-a-portal-5.png)

1. 選取 **Identity Provider證書** 檔案。

   ![](assets/add-single-sign-on-to-a-portal-6.png)

1. 按一下 **儲存**.

   ![](assets/add-single-sign-on-to-a-portal-7.png)

## 更新重新導向頁面設定 {#update-redirect-page-settings}

1. 在 **重新導向頁面** ，按一下 **編輯**.

   ![](assets/add-single-sign-on-to-a-portal-8.png)

   >[!NOTE]
   >
   >使用通用ID及SSO的客戶，必須在 **登入URL** 欄位。

1. 輸入 **註銷URL**. 這是您希望在使用者登出Marketo時，將使用者導向的URL。

   ![](assets/add-single-sign-on-to-a-portal-9.png)

1. 輸入 **錯誤URL**. 這是您要將使用者導向的URL，以防登入Marketo失敗。 按一下 **儲存**.

   ![](assets/add-single-sign-on-to-a-portal-10.png)

   >[!NOTE]
   >
   >這兩個頁面必須可供公開使用。

>[!MORELIKETHIS]
>
>* [使用通用ID登入訂閱](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md){target=&quot;_blank&quot;}
>* [僅限用戶登錄到SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target=&quot;_blank&quot;}
>* [邀請Marketo使用者加入兩個具有通用ID的例項](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target=&quot;_blank&quot;}

