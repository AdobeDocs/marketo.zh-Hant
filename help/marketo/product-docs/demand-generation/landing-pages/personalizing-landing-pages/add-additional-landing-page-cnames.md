---
unique-page-id: 2359798
description: 新增其他登錄頁面CNAME - Marketo檔案 — 產品檔案
title: 新增其他登錄頁面CNAME
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# 新增其他登錄頁面CNAME {#add-additional-landing-page-cnames}

您可能想要新增登錄頁面CNAME，以允許不同的URL指向您的Marketo登錄頁面。 依照下列步驟，將可協助您管理多個網域。

>[!CAUTION]
>
>Cookie無法跨網域共用。

>[!TIP]
>
>**相同的頂級域 — 好！ Cookie已共用**.<br/> **go**.mycompany.com > **資訊**.mycompany.com
>
>**不同的頂級域 — 錯誤！ Cookie為 _not_ 共用**.<br/> 走。**mycompany**.com > go。**mynewcompany**.com

>[!NOTE]
>
>**需要管理權限**

1. 前往 **管理** 的上界。

   ![](assets/add-additional-landing-page-cnames-1.png)

1. 按一下 **我的帳戶**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. 向下捲動至「支援資訊」，並複製您的Munchkin ID。

   ![](assets/add-additional-landing-page-cnames-3.png)

## 向IT人員發送請求 {#send-request-to-it}

1. 請您的IT部門設定下列CNAME:(取代 [CNAME] 以及您選擇的CNAME [蒙奇金ID] 和上一步的文字)。

   [CNAME].YourCompany.com > [蒙奇金ID].mktoweb.com

## 新增CNAME {#add-a-new-cname}

1. IT部門建立CNAME後，請前往 **管理** 的上界。

   ![](assets/add-additional-landing-page-cnames-4.png)

1. 按一下 **登錄頁面**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. 按一下 **新增** 然後選取 **新域別名**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. 輸入 **域別名。** 此 **預設頁面** 若訪客未放入URL，則會顯示。 在這種情況下，輸入他們應該去的地方。

   >[!NOTE]
   >
   >對於「預設頁面」，您可以選取登錄頁面或外部URL，例如您的公開網站。

   ![](assets/add-additional-landing-page-cnames-7.png)

1. 輸入 **預設頁面** 按一下 **建立**.

   ![](assets/add-additional-landing-page-cnames-8.png)

不錯！ 現在，如果您想要新增CNAME，您知道該做什麼。
