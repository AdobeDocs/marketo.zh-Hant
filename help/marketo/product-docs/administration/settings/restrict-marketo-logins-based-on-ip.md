---
unique-page-id: 2360297
description: 根據IP限制Marketo登入-Marketo文檔——產品文檔
title: 基於IP限制Marketo登錄
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# 根據IP {#restrict-marketo-logins-based-on-ip}限制Marketo登錄

您可以限制或讓使用者根據其IP位址存取Marketo。 這是方法。

>[!NOTE]
>
>**需要管理員權限**

>[!NOTE]
>
>本文中的資訊僅適用於login.marketo.com的直接登入。 目前無法對單一登入(SSO)登入強制執行IP限制。

1. 在&#x200B;**Admin**&#x200B;下，按一下&#x200B;**登錄設定**。

   ![](assets/image2014-9-16-12-3a57-3a56.png)

1. 按一下「編輯IP限制」。****

   ![](assets/image2014-9-16-12-3a58-3a13.png)

1. 選擇要&#x200B;**允許**&#x200B;還是&#x200B;**阻止**&#x200B;特定地址，輸入地址，然後按一下&#x200B;**保存**。

   >[!NOTE]
   >
   >**定義**
   >
   >* **允許的IP位址**:新增允許的IP位址是包含性的。它將包含所有指定的IP位址，並排除其他所有IP位址。
   >* **塊IP地址**:阻止特定IP訪問Marketo。
   >* **停用IP限制**:勾選此項將會停止任何／所有限制規則運作。請將它用於測試用途。


   >[!NOTE]
   >
   >您可以新增多項限制，但只能使用「全部允許」或「全部封鎖」。 您不能混搭、比對並允許和封鎖。

   ![](assets/image2014-9-16-13-3a9-3a40.png)

   您的行銷資料做得好，現在比以往更安全！
