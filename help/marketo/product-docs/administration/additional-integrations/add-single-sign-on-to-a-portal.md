---
unique-page-id: 2360356
description: 將單一登入新增至入口網站 — Marketo檔案 — 產品檔案
title: 新增單一登入至入口網站
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
source-git-commit: 1a6f029b8c9665ecd7fcc066004d88ee6c915505
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# 新增單一登入至入口網站 {#add-single-sign-on-to-a-portal}

如果您有驗證使用者的目錄服務，可以允許單一登入(SSO)進入Marketo。 我們使用以下專案支援此功能 [!DNL Security Assertion Markup Language] (SAML) 2.0版和更新版本。

Marketo的作用就像是SAML服務提供者(SP)，並依賴外部身分提供者(IdP)來驗證使用者。

啟用SSO後，IdP可以驗證使用者的認證。 當使用者希望使用Marketo軟體時，IdP會傳送已簽署的SAML訊息給Marketo，並充當SP。 此訊息會向Marketo證明使用者已獲得使用Marketo軟體的授權。

>[!NOTE]
>
>**需要管理員許可權**

>[!NOTE]
>
>您是否為 [!DNL Microsoft Azure] 使用者？ 檢視他們的 [整合教學課程](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/){target="_blank"}.

## 如何傳送請求 {#how-to-send-the-request}

* 將SSO請求（亦即SAML回應）傳送至 `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* 作為SP的對象URL。 使用 `http://saml.marketo.com/sp`
* 如果您使用SPNameQualifier屬性，請將Subject的NameID元素設定為 `http://saml.marketo.com/sp`
* 如果您要將多個Marketo訂閱聯合至相同的SSO提供者，您可以對每個Marketo子檔案使用唯一的SP URL，格式為 `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo僅支援「身分提供者」起始的（也稱為IdP起始的），使用者首先啟動Idp登入頁面、進行驗證，然後導覽至「我的Marketo」。

## 其他附註 {#additional-notes}

* **同步時間**  — 若是新使用者，處理初始SSO請求前會有大約10分鐘的延遲。
* **使用者布建** - Marketo會手動布建使用者。
* **Authorization** - Marketo會維護使用者許可權。
* **OAuth支援** - Marketo目前不支援OAuth。
* **自動使用者傳播**  — 也稱為「即時布建」，這是指使用者的第一個SAML登入能夠在他們存取的任何網頁應用程式(例如Marketo)中建立使用者，且不需要手動管理動作。 Marketo目前不支援此功能。
* **加密** - Marketo目前不支援加密。

>[!NOTE]
>
>開始之前，請以X.509格式和.crt、.der或.cer副檔名取得您的身分提供者憑證。

## 更新SAML設定 {#update-saml-settings}

SSO預設為停用。 請依照下列步驟來啟用SAML並進行設定。

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/add-single-sign-on-to-a-portal-1.png)

1. 按一下 **[!UICONTROL 單一登入]**.

   ![](assets/add-single-sign-on-to-a-portal-2.png)

   >[!NOTE]
   >
   >如果您沒有看見 **[!UICONTROL 單一登入]** 在 **[!UICONTROL 管理員]**，連絡人 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. 在 **[!UICONTROL SAML設定]** 區段，按一下 **[!UICONTROL 編輯]**.

   ![](assets/add-single-sign-on-to-a-portal-3.png)

1. 變更 **[!UICONTROL saml單一登入]** 至 **[!UICONTROL 已啟用]**.

   ![](assets/add-single-sign-on-to-a-portal-4.png)

1. 輸入您的 **[!UICONTROL 簽發者ID]**， **[!UICONTROL 實體ID]**，選取 **[!UICONTROL 使用者ID位置]**，然後按一下 **[!UICONTROL 瀏覽]**.

   ![](assets/add-single-sign-on-to-a-portal-5.png)

1. 選取您的 **[!UICONTROL 身分提供者憑證]** 檔案。

   ![](assets/add-single-sign-on-to-a-portal-6.png)

1. 按一下 **[!UICONTROL 儲存]**.

   ![](assets/add-single-sign-on-to-a-portal-7.png)

## 更新重新導向頁面設定 {#update-redirect-page-settings}

1. 在 **[!UICONTROL 重新導向頁面]** 區段，按一下 **[!UICONTROL 編輯]**.

   ![](assets/add-single-sign-on-to-a-portal-8.png)

   >[!NOTE]
   >
   >使用通用ID和SSO的客戶必須在以下位置輸入身分提供者的登入URL： **[!UICONTROL 登入URL]** 欄位。

1. 輸入 **[!UICONTROL 登出URL]**. 這是您希望使用者登出Marketo時導向至的URL。

   ![](assets/add-single-sign-on-to-a-portal-9.png)

1. 輸入 **[!UICONTROL 錯誤URL]**. 這是您希望在登入Marketo失敗時將使用者導向到的URL。 按一下 **[!UICONTROL 儲存]**.

   ![](assets/add-single-sign-on-to-a-portal-10.png)

   >[!NOTE]
   >
   >這兩個頁面都必須可公開使用。

>[!MORELIKETHIS]
>
>* [使用通用ID進行訂閱登入](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md){target="_blank"}
>* [僅限使用者登入至SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [使用通用ID邀請Marketo使用者使用兩個執行個體](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}

