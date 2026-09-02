---
description: 瞭解如何使用封鎖或允許的網域來設定Dynamic Chat安全性。 限制代理程式可以檢視哪些電子郵件網域，以及哪些網站可以使用您的聊天指令碼。
title: 安全性設定
feature: Dynamic Chat
exl-id: 68a53986-6f42-4aa2-86f6-0b2097f94963
TQID: https://experienceleague.adobe.com/7ans6J5WCXbTalK7ubMCrWBLWaJm3prPCoxsrCWEKtg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 88949407423d12a95bf39470e3c29835d934e2f6
workflow-type: tm+mt
source-wordcount: 238
ht-degree: 3%

---

# 安全性設定 {#security-settings}

在「安全性」設定中，您可以將網域新增至封鎖或允許的清單。

![](assets/security-settings-1.png)

>[!IMPORTANT]
>
>封鎖和允許電子郵件網域篩選僅適用於訪客直接在Dynamic Chat中（在聊天機器人或對話流程中）輸入其電子郵件地址時。 它不適用於Dynamic Chat從整合產品（例如Marketo Engage）收到的電子郵件地址。 如需詳細資訊，請參閱下表。

| 狀況 | 篩選是否適用？ |
|---|---|
| 訪客直接在Dynamic Chat聊天機器人中輸入電子郵件 | 是 |
| 訪客直接在Dynamic Chat對話流程中輸入電子郵件 | 是 |
| 電子郵件是從Marketo表單提交預先填入（對話流程會在表單填寫後顯示） | 無 |
| 電子郵件會從任何其他整合系統傳遞至Dynamic Chat | 無 |

## 封鎖的電子郵件網域 {#blocked-email-domains}

如果有任何訪客具有您不希望您的代理程式與之互動（例如競爭者）的電子郵件網域，請將其電子郵件網域新增至封鎖清單。

1. 選取&#x200B;**啟用驗證**&#x200B;滑桿以啟用封鎖清單。 最多可輸入50個網域，然後按一下&#x200B;**儲存**。

   ![](assets/security-settings-2.png)

## 允許的網域 {#allowed-domains}

新增允許的網域可確保第三方無法從您的網站刮取JavaScript並將其新增到他們自己的網站。

1. 選取&#x200B;**啟用驗證**&#x200B;滑桿以啟用您的允許清單。 輸入允許的網域，然後按一下&#x200B;**儲存**。

   ![](assets/security-settings-3.png)
