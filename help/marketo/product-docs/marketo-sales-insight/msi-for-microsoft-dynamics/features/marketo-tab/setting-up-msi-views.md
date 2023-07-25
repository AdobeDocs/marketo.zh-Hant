---
description: 設定MSI檢視 — Marketo檔案 — 產品檔案
title: 設定MSI檢視
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 設定MSI檢視 {#setting-up-msi-views}

在Dynamics中安裝Sales Insight外掛程式，會自動在「網站地圖」上新增「首選」和相關儀表板。 如果由於某種原因沒有新增儀表板，以下說明如何手動新增儀表板。

1. 在Dynamics中，按一下齒輪圖示並選取 **進階設定** 下拉式清單。

1. 在熒幕左上方，按一下 **設定**. 在「自訂」底下，選擇 **自訂**.

1. 按一下 **自訂系統**.

1. 在左側的樹狀結構中，按一下 **使用者端擴充功能** 並連按兩下 **網站地圖**.

1. 按一下向右箭號以前往下一頁。 在「銷售」底下，您應該會看到Marketo。 如果沒有匯入，請確定已正確匯入套件。

   >[!NOTE]
   >
   >在Marketo底下，您應該有：Best Betts、我的電子郵件、網路活動和匿名網路活動。 如果有任何控制面板遺失，請按一下Sales上方的+號，然後將它們新增為子區域。

1. 按一下控制面板以選取它。 在右側的欄中，為每個欄輸入下列個別資訊。 您可以忽略任何未列出的類別。

   **最佳比對**</br>
URL： MainviewBestbets.html</br>
圖示： /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID： marketo_bestbets</br>
標題：最佳比對

   **我的電子郵件**</br>
URL： mkt_/MainViewMyEmail.html</br>
圖示： /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID： marketo_myemail</br>
標題：我的電子郵件

   **網頁活動**</br>
URL： mkt_/MainViewWebActivity.html</br>
圖示： /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID： marketo_webactivity</br>
標題：網頁活動

   **匿名網路活動**</br>
URL： mkt_/MainViewWebActivity.html</br>
圖示： /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID： marketo_anonymous_webactivity</br>
標題：匿名Web活動

1. 按一下 **儲存** 完成時。
