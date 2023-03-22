---
unique-page-id: 2359746
description: 使用CNAME自訂您的登錄頁面URL - Marketo檔案 — 產品檔案
title: 使用CNAME自訂您的登錄頁面URL
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# 使用CNAME自訂您的登錄頁面URL {#customize-your-landing-page-urls-with-a-cname}

即使Marketo托管您的登錄頁面，URL仍可完全自訂。 沒有CNAME時的外觀：

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

它應該看起來的樣子：

`https://go.YourCompany.com/UnsubscribePage.html`

## 選擇CNAME {#choose-a-cname}

選取要進入登錄頁面之URL開頭的字詞。 它只是一個詞，應該相對短。 範例:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

一個詞（加上YourCompany.com）稱為CNAME。 你以後需要這個，記一下。

## 找到您的Munchkin ID {#find-your-munchkin-id}

1. 前往 **管理** 的上界。

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. 按一下 **我的帳戶**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**需要管理權限**

1. 向下捲動至「支援資訊」，並複製您的Munchkin ID。

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## 向IT人員發送請求 {#send-request-to-it}

請您的IT人員設定下列CNAME:(取代 [CNAME] 和 [蒙奇金ID] 和上一步的文字。)

[CNAME].YourCompany.com > [蒙奇金ID].mktoweb.com

## 完成CNAME設定 {#complete-cname-setup}

1. IT建立CNAME後，請前往 **管理** 的上界。

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. 按一下 **登錄頁面**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. 在 **設定** ，按一下 **編輯**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. 在 **登錄頁面的網域名稱**，請輸入 **後援頁面**，請輸入 **首頁** 按一下 **儲存**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>如果您的Marketo登陸頁面無法使用，系統會將您的後援頁面做為頁面銷售機會，重新導向至。

幹得好！ 您的登錄頁面現在已與您的公司網域加上品牌。
