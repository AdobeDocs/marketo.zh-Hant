---
description: 設定reCAPTCHA v3 - Marketo檔案 — 產品檔案
title: 設定reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# 設定reCAPTCHA v3 {#setting-up-recaptcha-v3}

ReCAPTCHA v3是一種順暢的體驗，可根據表單提交中的可疑程度為其評分，而不使用文字、影像或按鈕挑戰。 [深入了解](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target="_blank"}.

## 擷取您的資料中心和Munchkin ID {#retrieve-your-data-center-and-munchkin-id}

針對下方的初始reCAPTCHA v3設定區段中的步驟6，您將需要Marketo Engage訂閱的資料中心和Munchkin ID。 以下說明如何尋找這些區段。

1. 在Marketo中，按一下 **管理員**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. 按一下 **我的帳戶**.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. 向下捲動至支援資訊。

   ![](assets/setting-up-recaptcha-v3-3.png)

## 初始reCAPTCHA v3設定 {#initial-recaptcha-v3-setup}

下列步驟是在Marketo外部執行。

1. 前往 [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target="_blank"} 並按一下v3Admin Console。

1. 使用Google帳戶登入/註冊。

1. 按一下「建立」按鈕（+號）以建立新金鑰。

1. 建立標籤以識別要用於Marketo Engage的金鑰。

1. 選擇型別 **reCAPTCHA v3**. Marketo Engage目前不支援reCAPTCHA v2。

1. 新增Marketo Engage訂閱使用的每個網域。 此處未設定的網域會在啟用reCAPTCHA的表單上傳回錯誤。 請記得將「data center」和「munchkinID」取代為 [您的訂閱中的資料](#retrieve-your-data-center-and-munchkin-id).

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * 訂閱中設定的任何登陸頁面網域和別名

   >[!NOTE]
   >
   >舉例來說，如果您的帳戶資料中心是「sjst」，您允許清單中的網域將是 `app-sjst.marketo.com`. 如果您的Munchkin ID是123-ABC-789，則您允許清單的網域將是 `123-ABC-789.mktoweb.com`.

1. 設定應接收有關此服務之任何警示的所有者和其他電子郵件地址。

1. 接受reCAPTCHA服務條款。

1. 按一下 **提交**.

   >[!NOTE]
   >
   >讓網站金鑰和秘密金鑰方便用於Marketo Engage設定。

## 在Marketo Engage中設定驗證碼 {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>依照下列步驟操作後，然後 [在第一個Marketo表單中啟用驗證碼](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}，請務必立即測試表單，因為reCAPTCHA設定中的任何錯誤設定都可能破壞表單。

1. 在Marketo中，按一下 **管理員**.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. 選取 **驗證碼** 在樹狀結構中。

   ![](assets/setting-up-recaptcha-v3-5.png)

1. 按一下 **編輯** 驗證碼設定上的。

   ![](assets/setting-up-recaptcha-v3-6.png)

1. 按一下「驗證碼」下拉式清單，然後選擇reCAPTCHA v3。

   ![](assets/setting-up-recaptcha-v3-7.png)

1. 插入秘密金鑰和網站金鑰。 按一下 **儲存** 完成時。

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[在Marketo Forms中啟用驗證碼](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
