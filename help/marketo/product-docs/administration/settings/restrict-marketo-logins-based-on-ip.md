---
unique-page-id: 2360297
description: 根據IP限制Marketo登入 — Marketo檔案 — 產品檔案
title: 根據IP限制Marketo登入
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
source-git-commit: bd6f049d5959356a99314e81bb6cfe517c2efdfa
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 根據IP限制Marketo登入 {#restrict-marketo-logins-based-on-ip}

您可以根據使用者的IP位址，限制或允許使用者存取Marketo。 這是方法。

>[!NOTE]
>
>**需要管理權限**

>[!NOTE]
>
>本文中的資訊僅適用於login.marketo.com的直接登入。 目前無法對單一登入(SSO)登入強制實施IP限制。

1. 前往 **管理** 的上界。

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. 按一下 **登入設定**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. 按一下 **編輯IP限制**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. 選擇是否 **允許** 或 **區塊** 特定地址，輸入地址，然後按一下 **儲存**.

   >[!NOTE]
   >
   >**定義**
   >
   >* **允許的IP位址**:新增允許的IP位址是包容性的。 其中會包含所有指定的IP位址，並排除其他項目。
   >* **封鎖IP位址**:防止特定IP存取Marketo。
   >* **禁用IP限制**:勾選此項，會使任何/所有限制規則無法運作。 請將其用於測試用途。


   >[!NOTE]
   >
   >您可以新增多個限制，但只能是「全部允許」或「全部封鎖」。 您不能混合匹配允許和阻止的。

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   做得好，您的行銷資料比以往更安全了！
