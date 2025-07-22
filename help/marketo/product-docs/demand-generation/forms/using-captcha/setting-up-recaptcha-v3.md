---
description: 設定reCAPTCHA v3 - Marketo檔案 — 產品檔案
title: 設定reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 1%

---

# 設定[!UICONTROL reCAPTCHA v3] {#setting-up-recaptcha-v3}

ReCAPTCHA v3是一款順暢的體驗，可依據提交表單的可疑程度為其評分，而不使用文字、影像或按鈕挑戰。 [了解更多](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target="_blank"}。

## 擷取您的[!UICONTROL Data Center]和[!UICONTROL Munchkin ID] {#retrieve-your-data-center-and-munchkin-id}

對於下方的初始[!UICONTROL reCAPTCHA v3]設定區段中的步驟6，您將需要Marketo Engage訂閱的[!UICONTROL Data Center]和[!UICONTROL Munchkin ID]。 以下說明如何尋找這些區段。

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/setting-up-recaptcha-v3-1.png)

1. 按一下「**[!UICONTROL My Account]**」。

   ![](assets/setting-up-recaptcha-v3-2.png)

1. 向下捲動至[!UICONTROL Support Information]。

   ![](assets/setting-up-recaptcha-v3-3.png)

## 初始[!UICONTROL reCAPTCHA v3]設定 {#initial-recaptcha-v3-setup}

下列步驟會在Marketo外部執行。

1. 前往[https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target="_blank"}，然後按一下v3 Admin Console。

1. 使用Google帳戶登入/註冊。

1. 按一下[!UICONTROL Create]按鈕（+符號）以建立新金鑰。

1. 建立標籤以識別要用於Marketo Engage的金鑰。

1. 選擇型別&#x200B;**[!UICONTROL reCAPTCHA v3]**。 Marketo Engage目前不支援reCAPTCHA v2。

1. 新增Marketo Engage訂閱使用的每個網域。 若未在此處設定網域，則會在啟用reCAPTCHA的表單上傳回錯誤。 請記得將&#39;datacenter&#39;和&#39;munchkinID&#39;取代為您訂閱[中的](#retrieve-your-data-center-and-munchkin-id)資料。

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * 訂閱中設定的任何登陸頁面網域和別名

   >[!NOTE]
   >
   >例如，如果帳戶的[!UICONTROL Data Center]為「sjst」，您允許清單的網域將是`app-sjst.marketo.com`。 如果您的[!UICONTROL Munchkin ID]是123-ABC-789，則您允許清單的網域將是`123-ABC-789.mktoweb.com`。

1. 設定應接收有關此服務之任何警示的所有者和其他電子郵件地址。

1. 接受reCAPTCHA服務條款。

1. 按一下「**[!UICONTROL Submit]**」。

   >[!NOTE]
   >
   >讓網站金鑰和秘密金鑰方便用於Marketo Engage設定。

## 在Marketo Engage中設定驗證碼 {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>按照這些步驟操作，並在第一個Marketo表單[中](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}啟用驗證碼後，請務必立即測試表單，因為reCAPTCHA設定中的任何錯誤設定都會破壞表單。

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/setting-up-recaptcha-v3-4.png)

1. 在樹狀結構中選取&#x200B;**[!UICONTROL CAPTCHA]**。

   ![](assets/setting-up-recaptcha-v3-5.png)

1. 在&#x200B;**[!UICONTROL Edit]**&#x200B;設定上按一下[!UICONTROL CAPTCHA]。

   ![](assets/setting-up-recaptcha-v3-6.png)

1. 按一下[!UICONTROL CAPTCHA]下拉式清單，然後選擇[!UICONTROL reCAPTCHA v3]。

   ![](assets/setting-up-recaptcha-v3-7.png)

1. 插入&#x200B;**[!UICONTROL Secret Key]**&#x200B;和&#x200B;**[!UICONTROL Site Key]**。 完成時，按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[在Marketo Forms中啟用驗證碼](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
