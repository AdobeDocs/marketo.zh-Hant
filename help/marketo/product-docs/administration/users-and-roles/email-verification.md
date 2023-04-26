---
description: 電子郵件驗證 — Marketo檔案 — 產品檔案
title: 電子郵件驗證
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: f60c40441be4bcfcc277b620f6d4e19b2047caef
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# 電子郵件驗證 {#email-verification}

Adobe Marketo Engage訂閱需要所有非API使用者(包括Marketo Engage管理員)來驗證其電子郵件地址。 未指派管理員角色的單一登入(SSO)使用者，會在透過電子郵件驗證功能啟用訂閱時，自動進行電子郵件驗證。

**使用者邀請**

當管理員邀請使用者時，當該使用者按一下邀請連結後，就會自動驗證該使用者。 系統會自動驗證未指派管理員角色的SSO使用者。

**變更電子郵件地址**

使用者的電子郵件地址變更後，即會無法驗證。 系統會傳送電子郵件給他們，讓他們重新驗證。 使用者可以按一下「 」，手動重新傳送該電子郵件 **重發驗證**.

![](assets/email-verification-1.png)

![](assets/email-verification-2.png)

**使用者和角色**

在「管理員>使用者和角色」中，「電子郵件狀態」欄會顯示每位使用者的驗證狀態。

![](assets/email-verification-3.png)

要向未驗證的用戶重新發送驗證電子郵件，只需選擇其記錄並按一下 **驗證電子郵件** 按鈕。
