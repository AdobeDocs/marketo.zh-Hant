---
unique-page-id: 2360297
description: 根據IP限制行銷人員登入——行銷人員檔案——產品檔案
title: 基於IP限制行銷人員登入
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# 基於IP限制行銷人員登入 {#restrict-marketo-logins-based-on-ip}

您可以限制或啟用使用者根據其IP位址存取Marketo。 這是方法。

>[!NOTE]
>
>**需要管理員權限**

>[!NOTE]
>
>本文中的資訊僅適用於login.marketo.com的直接登入。 目前無法對單一登入(SSO)登入強制執行IP限制。

1. 在「管 **理員**」下，按一 **下「登入設定」**。

   ![](assets/image2014-9-16-12-3a57-3a56.png)

1. 按一 **下編輯IP限制**。

   ![](assets/image2014-9-16-12-3a58-3a13.png)

1. 選擇要**允許**還是阻止特 **定地址** ，輸入地址，然後按一下 **保存**。

   >[!NOTE]
   >
   >**定義**
   >
   >    
   >    
   >    * **允許的IP位址**:新增允許的IP位址是包含性的。 它將包含所有指定的IP位址，並排除其他所有IP位址。
   >    * **塊IP地址**:防止特定IP存取Marketo。
   >    * **停用IP限制**:勾選此項將會停止任何／所有限制規則運作。 請將它用於測試用途。


   >[!NOTE]
   >
   >
   >您可以新增多項限制，但只能使用「全部允許」或「全部封鎖」。 您不能混搭、比對並允許和封鎖。

   ![](assets/image2014-9-16-13-3a9-3a40.png)

   您的行銷資料做得好，現在比以往更安全！

