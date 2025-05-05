---
description: 設定reCAPTCHA v3 - Marketo檔案 — 產品檔案
title: 設定reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# 設定reCAPTCHA v3 {#setting-up-recaptcha-v3}

ReCAPTCHA v3是一款順暢的體驗，可依據提交表單的可疑程度為其評分，而不使用文字、影像或按鈕挑戰。 [深入瞭解](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target="_blank"}。

## 擷取您的資料中心和Munchkin ID {#retrieve-your-data-center-and-munchkin-id}

針對下方「初始reCAPTCHA v3設定」區段中的步驟6，您將需要Marketo Engage訂閱的資料中心和Munchkin ID。 以下說明如何尋找這些區段。

1. 在Marketo中，按一下&#x200B;**管理員**。

   ![](assets/setting-up-recaptcha-v3-1.png)

1. 按一下&#x200B;**我的帳戶**。

   ![](assets/setting-up-recaptcha-v3-2.png)

1. 向下捲動至「支援資訊」。

   ![](assets/setting-up-recaptcha-v3-3.png)

## 初始reCAPTCHA v3設定 {#initial-recaptcha-v3-setup}

下列步驟會在Marketo外部執行。

1. 移至[https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target="_blank"}，然後按一下v3Admin Console。

1. 使用Google帳戶登入/註冊。

1. 按一下「建立」按鈕（+號）以建立新金鑰。

1. 建立標籤以識別要用於Marketo Engage的金鑰。

1. 選擇型別&#x200B;**reCAPTCHA v3**。 Marketo Engage目前不支援reCAPTCHA v2。

1. 新增Marketo Engage訂閱使用的每個網域。 若未在此處設定網域，則會在啟用reCAPTCHA的表單上傳回錯誤。 請記得將&#39;datacenter&#39;和&#39;munchkinID&#39;取代為您訂閱[&#128279;](#retrieve-your-data-center-and-munchkin-id)中的資料。

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * 訂閱中設定的任何登陸頁面網域和別名

   >[!NOTE]
   >
   >舉例來說，如果帳戶的資料中心是&quot;sjst&quot;，您允許清單的網域將是`app-sjst.marketo.com`。 如果您的Munchkin ID是123-ABC-789，您允許清單的網域將是`123-ABC-789.mktoweb.com`。

1. 設定應接收有關此服務之任何警示的所有者和其他電子郵件地址。

1. 接受reCAPTCHA服務條款。

1. 按一下&#x200B;**提交**。

   >[!NOTE]
   >
   >讓網站金鑰和秘密金鑰方便用於Marketo Engage設定。

## 在Marketo Engage中設定驗證碼 {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>按照這些步驟操作，並在第一個Marketo表單[&#128279;](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}中啟用驗證碼後，請務必立即測試表單，因為reCAPTCHA設定中的任何錯誤設定都會破壞表單。

1. 在Marketo中，按一下&#x200B;**管理員**。

   ![](assets/setting-up-recaptcha-v3-4.png)

1. 在樹狀結構中選取&#x200B;**驗證碼**。

   ![](assets/setting-up-recaptcha-v3-5.png)

1. 在驗證碼設定上按一下&#x200B;**編輯**。

   ![](assets/setting-up-recaptcha-v3-6.png)

1. 按一下CAPTCHA下拉式清單，然後選擇reCAPTCHA v3。

   ![](assets/setting-up-recaptcha-v3-7.png)

1. 插入秘密金鑰和網站金鑰。 完成時，按一下&#x200B;**儲存**。

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[在Marketo Forms中啟用驗證碼](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
