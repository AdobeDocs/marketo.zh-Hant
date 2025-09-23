---
description: 重新設定 [!DNL Dynamics] 驗證方法 — Marketo檔案 — 產品檔案
title: 重新設定 [!DNL Dynamics] 驗證方法
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 1%

---

# 重新設定 Dynamics 驗證方法 {#reconfigure-dynamics-authentication-method}

請依照下列步驟更新您的[!DNL Dynamics]驗證方法。

>[!PREREQUISITES]
>
>使用以下任一文章中的所需驗證方法，在[!DNL Microsoft Dynamics]和Active Directory (Azure AD/ADFS)中設定應用程式：
>
>* [步驟2之3：設定具有伺服器對伺服器連線的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}
>* [步驟2之4：使用資源擁有者密碼控制連線設定Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. 按一下&#x200B;**Microsoft Dynamics**，然後按&#x200B;**[!UICONTROL Disable Sync]**。

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >您必須暫時停用全域同步才能更新驗證方法。

1. 按一下「**[!UICONTROL Reconfigure New Auth Method]**」標籤。

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. 選取想要的新驗證方法（在此範例中，我們選擇Web API）。

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. 輸入新驗證方法所需的認證，然後按一下&#x200B;**[!UICONTROL Validate]**。

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* 特定欄位將因選擇的驗證方法而異，表單將根據之前的驗證方法自動更新。
   >* 如果您之前已同步，上述表單中的資料可能會預先填入。 請重新輸入所有認證，以確保值正確無誤。

1. 如果一切正常，驗證同步將會產生所有綠色核取標籤![](assets/green-check.png)。 檢閱訊息並按一下&#x200B;**[!UICONTROL Switch]**&#x200B;以更新驗證方法。

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >如果您看見![](assets/red-x.png)，則該步驟有問題。 請參閱[修正 [!DNL Dynamics] 驗證同步問題](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)以識別並修正問題。 然後重新執行同步驗證步驟，直到結果如上圖所示。

1. 按一下&#x200B;**[!UICONTROL Confirm]**&#x200B;以繼續。

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. 再按一下&#x200B;**[!UICONTROL Confirm]**。

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. 按一下「**[!UICONTROL OK]**」。

   >[!IMPORTANT]
   >
   >系統需要15分鐘的時間來接受新的驗證模式。 請於切換後等待15分鐘，再重新啟用同步處理。
