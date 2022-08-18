---
description: 設定reCAPTCHA v3 -Marketo文檔 — 產品文檔
title: 設定reCAPTCHA v3
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: 24942664d613fa2851bad7a0dd3862027deacf37
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 設定reCAPTCHA v3 {#setting-up-recaptcha-v3}

簡介文本

## 初始reCAPTCHA v3設定 {#initial-recaptcha-v3-setup}

文本：描述v3 — 在Marketo Engage之外執行以下步驟。

1. 轉到 [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;}，然後按一下v3Admin Console。

1. 登錄/註冊Google帳戶。

1. 按一下「建立」按鈕（+號）以建立新鍵。

1. 建立標籤以標識要用於Marketo Engage的密鑰。

1. 選擇類型 **reCAPTCHA v3**。 Marketo Engage當前不支援reCAPTCHA v2。

1. 添加Marketo Engage訂閱使用的每個域。 未在此處設定的域將在啟用reCAPTCHA的表單上返回錯誤。

   * 123-ABC-456.mktoweb.com
   * app-pod.marketo.com
   * 訂閱中配置的任何登錄頁域和別名

1. 設定應接收有關此服務的任何警報的所有者和其他電子郵件地址。

1. 接受reCAPTCHA服務條款。

1. 按一下 **提交**。

>[!NOTE]
>
>使站點密鑰和密鑰在Marketo Engage配置中保持方便。

## 在Marketo Engage中設定驗證碼 {#setting-up-captcha-in-marketo-engage}

1. 在Marketo，按一下 **管理**。

   ![](assets/setting-up-recaptcha-v3-1.png)

1. 選擇 **驗證碼** 在樹上。

   ![](assets/setting-up-recaptcha-v3-2.png)

1. 按一下 **編輯** 驗證碼設定。

   ![](assets/setting-up-recaptcha-v3-3.png)

1. 按一下「驗證碼」下拉清單，然後選擇reCAPTCHA v3。

   ![](assets/setting-up-recaptcha-v3-4.png)

1. 插入密鑰和站點密鑰。 按一下 **保存** 完成。

   ![](assets/setting-up-recaptcha-v3-5.png)
