---
description: 步驟4之1 — 安裝具有資源所有者密碼控制連線的Marketo解決方案 — Marketo檔案 — 產品檔案
title: 步驟4之1 — 安裝具有資源擁有者密碼控制連線的Marketo解決方案
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
feature: Microsoft Dynamics
source-git-commit: 2eb61d43f2f470d42e1b50ab8edc99e4e25c23cf
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 1%

---

# 步驟4之1：安裝具有資源擁有者密碼控制連線的Marketo解決方案 {#step-1-of-4-install-the-marketo-solution-ropc}

在同步Microsoft Dynamics 365和Marketo Engage之前，您必須先在Dynamics中安裝Marketo解決方案。 **需要Dynamics管理員許可權**。

>[!CAUTION]
>
>* 初始同步處理完成之前，請勿啟用自訂實體同步處理。 初始同步完成後，您將會收到電子郵件通知。
>* 如果您的Dynamics Sync已啟用多重驗證(MFA)，您必須將其停用，Dynamics才能正確地與Marketo同步。 如需其他資訊，請連絡[Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}。

>[!NOTE]
>
>將Marketo同步至CRM後，如果不取代執行個體，就無法執行新的同步。

>[!PREREQUISITES]
>
>[下載Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. 登入&#x200B;**[Microsoft Office 365](https://login.microsoftonline.com/)**。

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. 按一下![](assets/image2015-3-16-16-3a1-3a13.png)功能表並選取&#x200B;**[!UICONTROL CRM]**。

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. 按一下![](assets/image2015-5-13-10-3a5-3a8.png)功能表。 在下拉式功能表中選取&#x200B;**[!UICONTROL 設定]**，然後選取&#x200B;**[!UICONTROL 解決方案]**。

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. 按一下&#x200B;**[!UICONTROL 匯入]**。

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. 按一下&#x200B;**[!UICONTROL 選擇檔案]**。 選取您[下載的Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}。 按一下&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. 檢視方案資訊，然後按一下&#x200B;**[!UICONTROL 檢視方案封裝詳細資料]**。

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. 檢查完所有詳細資料後，按一下[關閉]。**&#x200B;**

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 現在，返回[方案資訊]頁面，按一下[下一步]。**&#x200B;**

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. 確認已選取SDK選項核取方塊。 按一下&#x200B;**[!UICONTROL 匯入]**。

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

1. 現在請等待匯入完成。 站起來做一些伸展。

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. 按一下 **[!UICONTROL 關閉]**。

   >[!NOTE]
   >
   >您可能會看到顯示「Marketo銷售機會管理已完成，但有警告」的訊息。 這是完全正常的情況。

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. 「Marketo銷售機會管理」現在會出現在解決方案清單中。

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. 選取&#x200B;**[!UICONTROL Marketo銷售機會管理]**，然後按一下&#x200B;**[!UICONTROL Publish所有自訂]**。

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   做得很好！安裝完成。

   >[!MORELIKETHIS]
   >
   >[步驟2之4：使用資源擁有者密碼控制連線設定Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}
