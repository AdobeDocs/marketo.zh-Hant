---
description: 第1步（共4步） — 使用資源擁有者密碼控制連線安裝Marketo解決方案 — Marketo檔案 — 產品檔案
title: 第1步（共4步） — 使用資源擁有者密碼控制連線安裝Marketo解決方案
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
source-git-commit: 7e6fab646ec03394cb406fc41442d585c162bb25
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 第1步，共4步：安裝具有資源擁有者密碼控制連線的Marketo解決方案 {#step-1-of-4-install-the-marketo-solution-ropc}

您必須先在Dynamics中安裝Microsoft解決方案，才能同步Marketo Dynamics 365和Marketo。 **需要Dynamics管理員權限。**

>[!CAUTION]
>
>* 在完成初始同步之前，請勿啟用自訂實體同步。 完成初始同步後，系統會透過電子郵件通知您。
>* 如果已為Dynamics同步啟用了多重身份驗證(MFA)，則必須禁用它，以便Dynamics與Marketo正確同步。 欲知更多資訊，請聯繫 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support).


>[!NOTE]
>
>將Marketo同步至CRM後，若不取代執行個體，就無法執行新同步。

>[!PREREQUISITES]
>
>[下載Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. 登入 **[Microsoft Office 365](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. 按一下 ![](assets/image2015-3-16-16-3a1-3a13.png) 選取 **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. 按一下 ![](assets/image2015-5-13-10-3a5-3a8.png) 功能表。 在下拉式功能表中選取 **設定** 然後選取 **解決方案**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. 按一下 **匯入。**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. 按一下 **選擇「檔案」。** 選擇您的Marketo銷售機會管理解決方案 [已下載](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). 按一下 **下一個**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. 檢視解決方案資訊，然後按一下 **查看解決方案包詳細資訊**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. 檢查完所有詳細資訊後，按一下 **關閉**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 現在，返回「解決方案資訊」頁面，按一下 **下一個**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. 確認已選取SDK選項核取方塊。 按一下 **匯入**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

1. 現在等待匯入完成。 起來，做些伸展。

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. 按一下 **關閉。**

   >[!NOTE]
   >
   >您可能會看到一則訊息，指出「Marketo銷售機會管理已完成並出現警告」。 這是完全預期的。

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. Marketo銷售機會管理現在會顯示在解決方案清單中。

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. 選擇 **Marketo銷售機會管理** 按一下 **發佈所有自訂。**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   五！ 安裝已完成。

   >[!MORELIKETHIS]
   >
   >[第2步，共4步：使用資源擁有者密碼控制連線設定Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
