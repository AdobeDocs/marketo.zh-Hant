---
unique-page-id: 10092925
description: 預覽和測試網站行銷活動 — Marketo檔案 — 產品檔案
title: 預覽和測試網站行銷活動
exl-id: 6cc4ebd8-0d39-4a7d-bc3d-e8cd18157470
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 預覽和測試網站行銷活動 {#preview-and-test-a-web-campaign}

本文說明預覽網站行銷活動的不同方式，以及如何使用沙箱區段即時測試您的網站。

>[!NOTE]
>
>預覽只會顯示促銷活動在選定網站上的外觀。 連結和Widget將無法使用，因為會避免Analytics中的錯誤點選/檢視。

## 在建立頁面上預覽網站行銷活動 {#preview-a-web-campaign-on-the-creation-page}

1. 前往 **網站行銷活動**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. 按一下 **建立新的網站行銷活動** 或圖示以編輯現有的行銷活動。

   ![](assets/create-new-or-edit-web-campaign.png)

1. 在網站預覽中，新增頁面URL並按一下 **預覽**. 隨即開啟新視窗/標籤，顯示行銷活動預覽。

   ![](assets/three-1.png)

   >[!TIP]
   >
   >按一下 **共用** 以開啟具有促銷活動預覽之固定URL的電子郵件。

   >[!NOTE]
   >
   >您也可以選擇安裝瀏覽器外掛程式(可 [鉻黃](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) 或 [Firefox](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi))，以獲得預覽行銷活動的最佳體驗。 請參閱以下小節。

## 使用瀏覽器外掛程式，在建立頁面上預覽網站行銷活動 {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. 請依照上節中的步驟1和2操作。

1. 按一下瀏覽器外掛程式的連結（在此案例中我們使用的是Chrome）。

   ![](assets/4-1.png)

1. 新視窗/標籤隨即開啟。 按一下 **新增至Chrome**.

   ![](assets/five.png)

1. 按一下 **新增擴充功能**.

   ![](assets/six.png)

1. 返回Marketo。 新增頁面URL並按一下 **預覽**.

   ![](assets/seven.png)

1. 隨即開啟新視窗/標籤，讓您預覽行銷活動在桌上型電腦、手機或平板電腦上的外觀。

   ![](assets/campaign-preview.png)

## 在網站行銷活動頁面上預覽網站行銷活動 {#preview-a-web-campaign-on-the-web-campaigns-page}

1. 檢視您的網路行銷活動清單時，只要選擇行銷活動並按一下 **預覽** 圖示。

   ![](assets/web-campaigns-1-preview-hand.png)

   輕鬆！

## 在您的網站上預覽網站行銷活動 {#preview-a-web-campaign-on-your-website}

建立沙箱區段和行銷活動。

1. 前往 **區段**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. 按一下 **新建**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. 為區段命名。

1. 在「行為」底下，將「包含頁面」拖曳至畫布上。 新增值 &#42;sandbox=1&#42;. 按一下 **儲存並定義行銷活動**.

   ![](assets/segment.png)

1. 在「設定網頁行銷活動」頁面上，從清單中選取目標區段，將其變更為沙箱區段。

   ![](assets/set-web-campaign-target-segment.jpg)

1. 完成行銷活動創意並按一下 **Launch**.

   ![](assets/click-launch.jpg)

1. 前往您的網站，在URL結尾新增URL引數&quot;？sandbox=1&quot;。 範例： `www.marketo.com?sandbox=1`.

1. 請參閱您網站上的行銷活動反應。

>[!NOTE]
>
>行銷活動在訪客工作階段期間只會回應一次。 若要再次檢視行銷活動，請清除您的瀏覽器Cookie。

>[!NOTE]
>
>無法預覽重新導向行銷活動。 測試它們的唯一方式是使用沙箱區段(依特定頁面鎖定目標 —  &#42;sandbox=redirect&#42;)
