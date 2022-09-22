---
description: 設定reCAPTCHA v3 - Marketo檔案 — 產品檔案
title: 設定reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: 457b4aadac47b0a8614c3e6025d2e1ae287b5ecc
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 設定reCAPTCHA v3 {#setting-up-recaptcha-v3}

ReCAPTCHA v3是無摩擦的體驗，可根據提交內容的可疑程度對其評分，而不會使用文字、影像或按鈕挑戰。 [深入了解](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target=&quot;_blank&quot;}。

## 擷取您的資料中心和Munchkin ID {#retrieve-your-data-center-and-munchkin-id}

若為下方「初始reCAPTCHA v3」設定區段中的步驟6，您需要Marketo Engage訂閱的資料中心和Munchkin ID。 這是如何找到它們。

1. 在Marketo中，按一下 **管理**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. 按一下 **我的帳戶**.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. 向下捲動至支援資訊。

   ![](assets/setting-up-recaptcha-v3-3.png)

## 初始reCAPTCHA v3設定 {#initial-recaptcha-v3-setup}

下列步驟在Marketo外部執行。

1. 前往 [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;}，然後按一下v3Admin Console。

1. 登入/註冊Google帳戶。

1. 按一下「建立」按鈕（+號）以建立新密鑰。

1. 建立標籤以識別要用於Marketo Engage的金鑰。

1. 選擇類型 **reCAPTCHA v3**. Marketo Engage目前不支援reCAPTCHA v2。

1. 新增Marketo Engage訂閱使用的每個網域。 若未在此處設定網域，其中reCAPTCHA已啟用，系統會傳回錯誤。 請記得將&#39;datacenter&#39;和&#39;munchkinID&#39;取代為 [訂閱中的資料](#retrieve-your-data-center-and-munchkin-id).

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * 訂閱中設定的任何登錄頁面網域和別名

   >[!NOTE]
   >
   >例如，如果您帳戶的資料中心是「sjst」，表示您允許列出的網域為 `app-sjst.marketo.com`. 如果您的Munchkin ID是123-ABC-789，您允許的網域會是 `123-ABC-789.mktoweb.com`.

1. 設定應接收有關此服務任何警報的擁有者和其他電子郵件地址。

1. 接受reCAPTCHA服務條款。

1. 按一下 **提交**.

   >[!NOTE]
   >
   >保持Marketo Engage配置中可用的站點密鑰和密鑰。

## 在Marketo Engage中設定驗證碼 {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>執行這些步驟後， [在您的第一個Marketo表單中啟用驗證碼](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target=&quot;_blank&quot;}，請務必立即測試表單，因為reCAPTCHA設定中的任何錯誤設定都可能破壞表單。

1. 在Marketo中，按一下 **管理**.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. 選擇 **驗證碼** 在樹上。

   ![](assets/setting-up-recaptcha-v3-5.png)

1. 按一下 **編輯** 在驗證碼設定上。

   ![](assets/setting-up-recaptcha-v3-6.png)

1. 按一下「驗證碼」下拉式清單，然後選擇reCAPTCHA v3。

   ![](assets/setting-up-recaptcha-v3-7.png)

1. 插入密鑰和站點密鑰。 按一下 **儲存** 時才能使用。

   ![](assets/setting-up-recaptcha-v3-8.png)
