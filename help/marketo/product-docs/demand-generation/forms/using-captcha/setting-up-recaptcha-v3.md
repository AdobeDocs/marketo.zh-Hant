---
description: 設定reCAPTCHA v3 -Marketo文檔 — 產品文檔
title: 設定reCAPTCHA v3
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: 1803d6355747f4b6300509a3d361bf235dd56f44
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 設定reCAPTCHA {#setting-up-recaptcha}

簡介文本

## 設定reCAPTCHA v3 {#setting-up-recaptcha-v3}

文本：描述v3 — 在Marketo Engage之外執行以下步驟。

1. 轉到 [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;}，然後按一下v3Admin Console。

1. 登錄/註冊Google帳戶。

1. 按一下「建立（+號）」按鈕以建立新鍵。

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
>使站點密鑰和密鑰便於Marketo Engage配置。

## 在Marketo Engage中設定驗證碼 {#setting-up-captcha-in-marketo-engage}

1. 在Marketo，按一下 **管理** 選擇 **驗證碼**。

PICC

1. 按一下 **編輯** 驗證碼設定。

PICC

1. 按一下「驗證碼」下拉清單，然後選擇reCAPTCHA v3。

PICC

1. 插入密鑰和站點密鑰。 按一下 **保存** 完成。

PICC
