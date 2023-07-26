---
unique-page-id: 2359798
description: 新增其他登陸頁面CNAME - Marketo檔案 — 產品檔案
title: 新增其他登陸頁面CNAME
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# 新增其他登陸頁面CNAME {#add-additional-landing-page-cnames}

您可能想要新增登陸頁面CNAME，以允許不同的URL指向您的Marketo登陸頁面。 依照下列步驟操作將協助您管理多個網域。

>[!CAUTION]
>
>Cookie無法跨網域共用。

>[!TIP]
>
>**相同的最上層網域 — 良好！ Cookie已共用**.<br/> **執行**.mycompany.com > **資訊**.mycompany.com
>
>**不同的頂級網域 — 錯誤！ Cookie是 _非_ 已共用**.<br/> 前往。**我的公司**.com >執行。**mynewcompany**.com

>[!NOTE]
>
>**需要管理員許可權**

1. 前往 **管理員** 區域。

   ![](assets/add-additional-landing-page-cnames-1.png)

1. 按一下 **我的帳戶**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. 向下捲動至「支援資訊」並複製您的Munchkin ID。

   ![](assets/add-additional-landing-page-cnames-3.png)

## 傳送要求給IT {#send-request-to-it}

1. 要求您的IT部門設定下列CNAME： (取代 [CNAME] 以及您選擇的CNAME [Munchkin ID] （包含上一步驟中的文字）。

   [CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## 新增CNAME {#add-a-new-cname}

1. IT部門建立CNAME後，請前往 **管理員** 區域。

   ![](assets/add-additional-landing-page-cnames-4.png)

1. 按一下 **登陸頁面**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. 按一下 **新增** 然後選取 **新網域別名**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. 輸入您的 **網域別名。** 此 **預設頁面** 如果訪客未放入URL，則會顯示。 輸入在這種情況下應該前往的位置。

   >[!NOTE]
   >
   >對於「預設頁面」，您可以選取登入頁面或外部URL，例如您的公用網站。

   ![](assets/add-additional-landing-page-cnames-7.png)

1. 輸入您的 **預設頁面** 並按一下 **建立**.

   ![](assets/add-additional-landing-page-cnames-8.png)

很好！ 現在您知道如果想要新增CNAME該怎麼做。
