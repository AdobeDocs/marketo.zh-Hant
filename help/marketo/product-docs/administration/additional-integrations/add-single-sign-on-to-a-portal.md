---
unique-page-id: 2360356
description: 將單一登入新增至入口網站 — Marketo檔案 — 產品檔案
title: 將單一登入新增至入口網站
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 3%

---

# 將單一登入新增至入口網站 {#add-single-sign-on-to-a-portal}

如果您有驗證使用者的目錄服務，可以允許單一登入(SSO)進入Marketo。 我們使用[!DNL Security Assertion Markup Language] (SAML) 2.0版和更新版本支援此功能。

Marketo的作用就像是SAML服務提供者(SP)，並且仰賴外部身分提供者(IdP)來驗證使用者。

啟用SSO後，IdP可以驗證使用者的認證。 當使用者希望使用Marketo軟體時，IdP會傳送已簽署的SAML訊息給Marketo（充當SP）。 此訊息會向Marketo證明使用者已獲得使用Marketo軟體的授權。

>[!NOTE]
>
>**需要管理員許可權**

>[!IMPORTANT]
>
>這不適用於已上線至Adobe Identity的訂閱。 對於已上線至Adobe Identity的訂閱，單一登入是在Adobe Admin Console中的Adobe組織層級設定。 Adobe Admin Console目前僅支援SP起始。 [在這裡瞭解更多](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}。

>[!NOTE]
>
>您是[!DNL Microsoft Azure]使用者嗎？ 檢視他們的[整合教學課程](https://learn.microsoft.com/en-us/entra/identity/saas-apps/marketo-tutorial){target="_blank"}。 僅供參考，其教學課程的步驟5c中有一個錯字。 請將轉送狀態設定為`https://<munchkinid>.mktoweb.com`，**_不是_** `https://<munchkinid>.marketo.com`。

## 如何傳送請求 {#how-to-send-the-request}

* 將SSO要求（亦即SAML回應）傳送至`https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* 做為SP的對象URL。 使用`http://saml.marketo.com/sp`
* 如果您使用SPNameQualifier屬性，請將Subject的NameID元素設定為`http://saml.marketo.com/sp`
* 如果您要將多個Marketo訂閱聯合到同一個SSO提供者，則可以針對每個Marketo子檔案使用格式為`http://saml.marketo.com/sp/<munchkin_id>`的唯一SP URL

>[!NOTE]
>
>Marketo僅支援身分提供者起始（也稱為IdP起始），使用者在啟動時會先啟動IdP登入頁面、進行驗證，然後導覽至「我的Marketo」。 如果您的Marketo訂閱已移至Admin Console，Adobe Admin Console目前僅支援服務提供者起始的（也稱為SP起始的）。 您的SSO體驗可能會有所變更。

## 其他附註 {#additional-notes}

* **同步處理時間** — 對於新使用者而言，在處理初始SSO要求之前，大約會延遲10分鐘。
* **使用者布建** - Marketo會手動布建使用者。
* **授權** — 在Marketo中維護使用者許可權。
* **OAuth支援** - Marketo目前不支援OAuth。
* **自動使用者傳播** — 也稱為「準時布建」，這是當使用者的首次SAML登入能夠在他們存取的任何網頁應用程式(例如Marketo)中建立使用者，且不需要手動管理動作時。 Marketo目前不支援此功能。
* **加密** - Marketo目前不支援加密。

>[!NOTE]
>
>開始之前，請以X.509格式取得身分提供者憑證，副檔名為.crt、.der或.cer。

## 更新SAML設定 {#update-saml-settings}

SSO預設為停用。 請依照以下步驟啟用SAML並進行設定。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/add-single-sign-on-to-a-portal-1.png)

1. 按一下「**[!UICONTROL Single Sign-On]**」。

   ![](assets/add-single-sign-on-to-a-portal-2.png)

   >[!NOTE]
   >
   >如果您在&#x200B;**[!UICONTROL Single Sign-On]**&#x200B;下沒有看到&#x200B;**[!UICONTROL Admin]**，請連絡[Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}。

1. 在&#x200B;**[!UICONTROL SAML Settings]**&#x200B;區段下，按一下&#x200B;**[!UICONTROL Edit]**。

   ![](assets/add-single-sign-on-to-a-portal-3.png)

1. 將&#x200B;**[!UICONTROL SAML Single Sign-On]**&#x200B;變更為&#x200B;**[!UICONTROL Enabled]**。

   ![](assets/add-single-sign-on-to-a-portal-4.png)

1. 輸入您的&#x200B;**[!UICONTROL Issuer ID]**、**[!UICONTROL Entity ID]**、選取&#x200B;**[!UICONTROL User ID Location]**，然後按一下&#x200B;**[!UICONTROL Browse]**。

   ![](assets/add-single-sign-on-to-a-portal-5.png)

1. 選取您的&#x200B;**[!UICONTROL Identity Provider Certificate]**&#x200B;檔案。

   ![](assets/add-single-sign-on-to-a-portal-6.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/add-single-sign-on-to-a-portal-7.png)

## 更新重新導向頁面設定 {#update-redirect-page-settings}

1. 在&#x200B;**[!UICONTROL Redirect Pages]**&#x200B;區段下，按一下&#x200B;**[!UICONTROL Edit]**。

   ![](assets/add-single-sign-on-to-a-portal-8.png)

   >[!NOTE]
   >
   >使用通用ID及SSO的客戶必須在&#x200B;**[!UICONTROL Login URL]**&#x200B;欄位中輸入身分提供者的登入URL。

1. 輸入&#x200B;**[!UICONTROL Logout URL]**。 這是您希望在使用者登出Marketo時導向他們的URL。

   ![](assets/add-single-sign-on-to-a-portal-9.png)

1. 輸入&#x200B;**[!UICONTROL Error URL]**。 這是您希望在登入Marketo失敗時導向使用者的URL。 按一下「**[!UICONTROL Save]**」。

   ![](assets/add-single-sign-on-to-a-portal-10.png)

   >[!NOTE]
   >
   >這兩個頁面都必須可公開使用。

>[!MORELIKETHIS]
>
>* [使用通用識別碼進行訂閱登入](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md){target="_blank"}
>* [僅將使用者登入限製為SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [邀請Marketo使用者使用兩個具有通用ID的執行個體](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}
