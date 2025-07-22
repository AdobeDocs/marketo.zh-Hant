---
description: Marketo取消訂閱檢查 — Marketo檔案 — 產品檔案
title: Marketo取消訂閱檢查
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---

# [!UICONTROL Marketo Unsubscribe Check] {#marketo-unsubscribe-check}

[!UICONTROL Marketo Unsubscribe Check]會使用您團隊與Marketo的連線，防止電子郵件傳送給已在Marketo的潛在客戶管理系統中取消訂閱的使用者。 當銷售使用者傳送包含[!DNL Marketo Sales]的電子郵件時，將會對Marketo進行API呼叫，以檢查電子郵件ID是否已取消訂閱。 如果是，我們將封鎖電子郵件的傳送。

>[!NOTE]
>
>**需要管理員許可權**

## 開啟 {#turning-it-on}

1. 按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/marketo-unsubscribe-check-1.png)

1. 在[!UICONTROL Admin Settings]底下，按一下&#x200B;**[!UICONTROL Unsubscribes]**。

   ![](assets/marketo-unsubscribe-check-2.png)

1. 按一下「**[!UICONTROL Integrations]**」標籤。 在[!UICONTROL Marketo Unsubscribe Check]區段中，按一下滑桿以啟動檢查。

   ![](assets/marketo-unsubscribe-check-3.png)

## 須知 {#things-to-know}

Marketo取消訂閱檢查……

* 不會計入API限制中
* 需要建立Marketo連線
* 是全域設定
* 封鎖從Web應用程式、電子郵件使用者端和[!DNL Salesforce]傳送的電子郵件
