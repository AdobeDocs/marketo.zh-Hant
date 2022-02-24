---
description: Reconfigure Dynamics Authentication方法 — Marketo文檔 — 產品文檔
title: 重新配置Dynamics身份驗證方法
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
source-git-commit: 8d401eeba46dc1b21983ea03c8ecd823046a5479
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# 重新配置Dynamics身份驗證方法 {#reconfigure-dynamics-authentication-method}

按照以下步驟更新Dynamics驗證方法。

>[!PREREQUISITES]
>
>使用以下任一文章中所需的身份驗證方法在MicrosoftDynamics和Active Directory(Azure AD/ADFS)中設定應用程式：
>* [第2步（共3步）:設定Marketo解決方案，使用伺服器到伺服器連接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)
>* [第2步（共4步）:設定具有資源所有者密碼控制連接的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)


1. 在Marketo **管理**。

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. 按一下 **Microsoft動力**，則 **禁用同步**。

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >必須暫時禁用全局同步才能更新身份驗證方法。

1. 按一下 **重新配置新身份驗證方法** 頁籤。

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. 選擇所需的新身份驗證方法（在本示例中，我們選擇Web API）。

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. 輸入新的身份驗證方法所需的憑據，然後按一下 **驗證**。

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* 特定欄位將因所選的身份驗證方法而異，表單將根據以前的身份驗證方法自動更新。
   >* 如果以前已同步，則可以預先填充上面表單中的資料。 請重新輸入所有憑據以確保正確的值。


1. 如果一切正常，驗證同步將生成所有綠色複選標籤 ![](assets/green-check.png)。 查看消息，然後按一下 **交換機** 更新驗證方法。

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >如果你看到 ![](assets/red-x.png)這一步有問題。 請參閱 [修復Dynamics驗證同步問題](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) 確定並解決問題。 然後重新運行同步驗證步驟，直到結果看起來與上面的影像類似。

1. 按一下 **確認** 繼續。

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. 按一下 **確認** 的雙曲餘切值。

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. 按一下 **確定**。

   >[!IMPORTANT]
   >
   >系統需要15分鐘才能接受新的身份驗證模式。 請等待15分鐘，從交換機開始，然後重新啟用同步。
