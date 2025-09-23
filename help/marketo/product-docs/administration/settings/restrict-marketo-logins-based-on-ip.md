---
unique-page-id: 2360297
description: 根據IP限制Marketo登入 — Marketo檔案 — 產品檔案
title: 根據 IP 限制 Marketo 登入
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 11%

---

# 根據 IP 限制 Marketo 登入 {#restrict-marketo-logins-based-on-ip}

您可以根據使用者的IP位址來限制或允許使用者存取Marketo。 方法如下。

>[!NOTE]
>
>**需要管理員許可權**

>[!IMPORTANT]
>
>本文資訊適用於直接登入login.marketo.com的使用者，不適用於使用Adobe ID進行驗證的使用者。 目前無法對單一登入(SSO)登入強制執行IP限制。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. 按一下「**[!UICONTROL Login Settings]**」。

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. 按一下「**[!UICONTROL Edit IP Restrictions]**」。

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. 選擇您要&#x200B;**允許**&#x200B;或&#x200B;**封鎖**&#x200B;特定地址，輸入地址，然後按一下&#x200B;**[!UICONTROL Save]**。

   >[!NOTE]
   >
   >**定義**
   >
   >* **[!UICONTROL Allowed IP addresses]**：新增允許的IP位址具有包含性。 它會包含指定的所有IP位址，並排除其他所有位址。
   >* **[!UICONTROL Block IP addresses]**：防止特定IP存取Marketo。
   >* **[!UICONTROL Disable IP Restrictions]**：核取此項將停止任何/所有限制規則運作。 將此用於測試目的。

   >[!NOTE]
   >
   >您可以新增多個限制，但是這些限制只能是「全部允許」或「全部封鎖」。 您無法混搭允許和封鎖。

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   做得很好，您的行銷資料現在比以往更安全！
