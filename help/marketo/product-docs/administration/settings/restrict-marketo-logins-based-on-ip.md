---
unique-page-id: 2360297
description: 根據IP限制Marketo登入 — Marketo檔案 — 產品檔案
title: 根據 IP 限制 Marketo 登入
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 3595cdc76a0f92da10dc5ddaac64c4cf83056e88
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 9%

---

# 根據 IP 限制 Marketo 登入 {#restrict-marketo-logins-based-on-ip}

您可以根據使用者的IP位址來限制或允許使用者存取Marketo。 方法如下。

>[!NOTE]
>
>**需要管理員許可權**

>[!IMPORTANT]
>
>Adobe Admin Console (AAC)支援[IP型存取控制](https://helpx.adobe.com/tw/enterprise/using/ip-based-access.html){target="_blank"}。 為確保順暢轉換，在啟用此功能的訂閱中，現有Marketo Engage IP限制將啟用，包括到2026年第1季的Adobe ID使用者。
>
>* 您可以隨時設定AAC IP型存取。
>* AAC和Marketo Engage限制可以同時執行。 使用相同的IP允許清單以瞭解相容性。
>
>2026年第1季度後，Marketo Engage IP限制將會淘汰。 IP型存取將透過AAC獨家管理，且必須設定為強制執行登入限制。 最終轉換日期將於稍後宣佈。

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
