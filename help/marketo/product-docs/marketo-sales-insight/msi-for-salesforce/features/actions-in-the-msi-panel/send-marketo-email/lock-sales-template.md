---
unique-page-id: 12981050
description: 鎖定銷售範本 — Marketo檔案 — 產品檔案
title: 鎖定銷售模板
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# 鎖定銷售模板 {#lock-sales-template}

為防止CRM使用者編輯銷售範本，管理員可啟用鎖定範本的功能，如此便可讓使用者從電子郵件編輯器中個別鎖定範本。

>[!CAUTION]
>
>此功能僅適用於Salesforce，且與Microsoft Dynamics或其他CRM不相容。 從Outlook或Gmail外掛程式存取的範本將不會鎖定，因為編輯器不受Marketo控制。

## 啟用鎖定模板 {#enable-lock-template}

>[!NOTE]
>
>**需要管理權限**

1. 前往 **管理**，然後按一下 **Sales Insight**.

   ![](assets/1.png)

1. 在 **設定**，按一下 **編輯**.

   ![](assets/2.png)

1. 檢查 **啟用鎖定範本的功能**. 按一下 **儲存**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>預設會勾選此方塊，並啟用鎖定範本的功能。 取消勾選此選項會停用電子郵件編輯器中的鎖定範本功能。

>[!NOTE]
>
>將此設定變更為管理員後 **not** 可回溯地影響現有模板；即不會自動鎖定。

## 在電子郵件編輯器中鎖定範本 {#lock-template-in-the-email-editor}

1. 選取您要鎖定的電子郵件，然後按一下 **編輯草稿**.

   ![](assets/5.png)

1. 在電子郵件編輯器中，按一下 **電子郵件設定**.

   ![](assets/6.png)

1. 檢查 **發佈至Marketo Sales Insight** 如果尚未檢查。 您現在可以取消勾選 **允許CRM使用者編輯電子郵件** 以鎖定範本。 按一下 **儲存**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >依預設，此方塊會勾選，CRM使用者可編輯電子郵件。
