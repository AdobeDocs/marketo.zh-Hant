---
unique-page-id: 18317340
description: Marketo取消訂閱檢查- Marketo Docs —— 產品檔案
title: Marketo取消訂閱檢查
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Marketo Unsubscribe Check {#marketo-unsubscribe-check}

Marketo Unsubscribe Check會使用您團隊與Market的連線，防止電子郵件寄送給在Marketto銷售機會管理系統中未訂閱的人。 當銷售使用者透過Sales Connect傳送電子郵件時，會向Marketo發出API呼叫，以檢查電子郵件ID是否未訂閱。 如果是，我們將封鎖電子郵件。

>[!NOTE]
>
>**需要管理員權限**

## 開啟{#turning-it-on}

1. 在Web應用程式中，按一下齒輪表徵圖並選擇&#x200B;**設定**。

   ![](assets/one-2.png)

1. 在「管理設定」下，按一下「取消訂閱&#x200B;**」。**

   ![](assets/two-3.png)

1. 按一下「**整合**」。

   ![](assets/three-3.png)

1. 在「Marketo取消訂閱檢查」區段中，按一下滑桿以啟用檢查。

   ![](assets/four-2.png)

## 要知道的{#things-to-know}

「行銷人員取消訂閱」檢查……

* 不計入您的API限制
* 需要建立Market才能建立連線
* 是全域設定
* 封鎖從Web應用程式、電子郵件客戶端和Salesforce傳送的電子郵件
