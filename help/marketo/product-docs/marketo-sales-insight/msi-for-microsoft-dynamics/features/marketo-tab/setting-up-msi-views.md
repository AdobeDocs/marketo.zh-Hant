---
description: 設定MSI檢視 — Marketo檔案 — 產品檔案
title: 設定MSI視圖
source-git-commit: 8227648ce67bf0f9f8b3b2fea7445850d8e154d5
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 設定MSI視圖 {#setting-up-msi-views}

在Dynamics中安裝Sales Insight外掛程式時，會自動在網站地圖上新增「最佳下注」和相關控制面板。 如果由於某些原因未新增控制面板，以下說明如何手動新增控制面板。

1. 在Dynamics中，按一下齒輪圖示並選取 **進階設定** 從下拉式清單中。

1. 在畫面左上角，按一下 **設定**. 在「自定義」下選擇 **自訂**.

1. 按一下 **自訂系統**.

1. 在左側的樹中，按一下 **用戶端擴充功能** 按兩下 **網站地圖**.

1. 按一下右箭頭前往下一頁。 在「銷售」下，您應該會看到Marketo。 如果沒有，請確定已正確匯入套件。

   >[!NOTE]
   >
   >在Marketo底下，您應該有：最佳選擇、我的電子郵件、Web活動和匿名Web活動。 如果缺少其中任何一個控制面板，請按一下「銷售」上方的+號，並將其新增為「子區域」。

1. 按一下控制面板以選取。 在右側的欄中，為每個欄輸入下方的個別資訊。 您可以忽略未列出的任何類別。

   **最佳下注**</br>
URL:MainviewBestbets.html</br>
圖示：/WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID:marketo_bestbets</br>
標題：最佳下注

   **我的電子郵件**</br>
URL:mkt_/MainViewMyEmail.html</br>
圖示：/WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID:marketo_myemail</br>
標題：我的電子郵件

   **網路活動**</br>
URL:mkt_/MainViewWebActivity.html</br>
圖示：/WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID:marketo_webactivity</br>
標題：網路活動

   **匿名Web活動**</br>
URL:mkt_/MainViewWebActivity.html</br>
圖示：/WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID:marketo_anonymous_webactivity</br>
標題：匿名Web活動

1. 按一下 **儲存** 時才能使用。
