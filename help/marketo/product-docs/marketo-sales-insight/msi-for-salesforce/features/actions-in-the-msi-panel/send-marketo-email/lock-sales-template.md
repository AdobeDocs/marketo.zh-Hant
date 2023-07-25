---
unique-page-id: 12981050
description: 鎖定銷售範本 — Marketo檔案 — 產品檔案
title: 鎖定銷售範本
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# 鎖定銷售範本 {#lock-sales-template}

為了防止CRM使用者編輯銷售範本，管理員可以啟用鎖定範本的功能，然後讓使用者可以從電子郵件編輯器個別鎖定範本。

>[!CAUTION]
>
>此功能僅適用於Salesforce，與Microsoft Dynamics或其他CRM不相容。 不會鎖定從Outlook或Gmail外掛程式存取的範本，因為編輯器不受Marketo控制。

## 啟用鎖定範本 {#enable-lock-template}

>[!NOTE]
>
>**需要管理員許可權**

1. 前往 **管理員**，然後按一下 **銷售分析**.

   ![](assets/1.png)

1. 下 **設定**，按一下 **編輯**.

   ![](assets/2.png)

1. Check **啟用鎖定範本的功能**. 按一下 **儲存**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>預設會勾選此方塊，並啟用鎖定範本的功能。 取消核取此選項將會停用電子郵件編輯器中的鎖定範本功能。

>[!NOTE]
>
>以管理員身分變更此設定將會 **not** 回溯影響現有的範本；也就是說，它不會自動鎖定它們。

## 在電子郵件編輯器中鎖定範本 {#lock-template-in-the-email-editor}

1. 選取您要鎖定的電子郵件，然後按一下 **編輯草稿**.

   ![](assets/5.png)

1. 在電子郵件編輯器中，按一下 **電子郵件設定**.

   ![](assets/6.png)

1. Check **發佈至Marketo Sales Insight** 如果尚未核取。 您現在可以取消勾選 **允許CRM使用者編輯電子郵件** 以鎖定範本。 按一下 **儲存**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >預設會勾選此方塊，並允許CRM使用者編輯電子郵件。
