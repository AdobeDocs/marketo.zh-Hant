---
description: 步驟4之1 — 安裝具有資源所有者密碼控制連線的Marketo解決方案 — Marketo檔案 — 產品檔案
title: 步驟4之1 — 安裝具有資源擁有者密碼控制連線的Marketo解決方案
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 3%

---

# 步驟4之1：安裝具有資源擁有者密碼控制連線的Marketo解決方案 {#step-1-of-4-install-the-marketo-solution-ropc}

在同步處理[!DNL Microsoft Dynamics] 365與Marketo之前，您必須先在[!DNL Dynamics]中安裝Marketo解決方案。 需要&#x200B;**[!DNL Dynamics]管理員許可權。**

>[!CAUTION]
>
>* 初始同步處理完成之前，請勿啟用自訂實體同步處理。 初始同步完成後，您將會收到電子郵件通知。
>* 如果您為[!DNL Dynamics]同步處理啟用多重驗證(MFA)，您必須停用它才能讓[!DNL Dynamics]與Marketo正確同步。 如需其他資訊，請連絡[Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support)。

>[!NOTE]
>
>將Marketo同步至CRM後，如果不取代執行個體，就無法執行新的同步。

>[!PREREQUISITES]
>
>[下載Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. 登入&#x200B;**[[!DNL Microsoft Office 365]](https://login.microsoftonline.com/)**。

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. 按一下![](assets/image2015-3-16-16-3a1-3a13.png)功能表並選取&#x200B;**[!UICONTROL CRM]**。

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. 按一下![](assets/image2015-5-13-10-3a5-3a8.png)功能表。 在下拉式功能表中選取&#x200B;**[!UICONTROL Settings]**，然後選取&#x200B;**[!UICONTROL Solutions]**。

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. 按一下「**[!UICONTROL Import]**」。

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. 按一下&#x200B;**[!UICONTROL Choose File]**。 選取您[下載的Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 按一下「**[!UICONTROL Next]**」。

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. 檢視方案資訊並按一下&#x200B;**[!UICONTROL View solution package details]**。

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. 檢查完所有詳細資料後，按一下&#x200B;**[!UICONTROL Close]**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 現在，返回[方案資訊]頁面，按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. 確認已選取SDK選項核取方塊。 按一下「**[!UICONTROL Import]**」。

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

1. 現在請等待匯入完成。 站起來做一些伸展。

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. 按一下「**[!UICONTROL Close]**」。

   >[!NOTE]
   >
   >您可能會看到顯示「Marketo銷售機會管理已完成，但有警告」的訊息。 這是完全正常的情況。

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. 「Marketo銷售機會管理」現在會出現在解決方案清單中。

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. 選取「**[!UICONTROL Marketo Lead Management]**」然後按一下「**[!UICONTROL Publish All Customizations]**」。

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   做得很好！安裝完成。

   >[!MORELIKETHIS]
   >
   >[步驟2之4：使用資源擁有者密碼控制連線設定Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}
