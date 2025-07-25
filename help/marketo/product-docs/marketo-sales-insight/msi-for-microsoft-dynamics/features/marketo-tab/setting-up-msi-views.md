---
description: 設定MSI檢視 — Marketo檔案 — 產品檔案
title: 設定MSI檢視
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# 設定MSI檢視 {#setting-up-msi-views}

在Dynamics中安裝[!DNL Sales Insight]外掛程式會自動在網站地圖上新增[!DNL Best Bets]和相關儀表板。 如果由於某種原因沒有新增儀表板，以下說明如何手動新增儀表板。

1. 在Dynamics中，按一下齒輪圖示，然後從下拉式清單中選取&#x200B;**[!UICONTROL Advanced Settings]**。

1. 在熒幕左上方，按一下&#x200B;**[!UICONTROL Settings]**。 在[自訂]下，選擇&#x200B;**[!UICONTROL Customizations]**。

1. 按一下「**[!UICONTROL Customize the System]**」。

1. 在左側的樹狀結構中，按一下&#x200B;**[!UICONTROL Client Extensions]**&#x200B;並連按兩下&#x200B;**[!UICONTROL Site Map]**。

1. 按一下向右箭號移至下一頁。 在銷售底下，您應該會看到Marketo。 如果沒有該套件，請確定您正確匯入該套件。

   >[!NOTE]
   >
   >在Marketo底下，您應該有：Best Bets、我的電子郵件、網頁活動和匿名網頁活動。 如果有任何控制面板遺失，請按一下Sales上方的+符號，並將它們新增為子區域。

1. 按一下控制面板以選取它。 在右側的欄中，為每個欄輸入下方的個別資訊。 您可以忽略任何未列出的類別。

   **首選**</br>
URL： MainviewBestbets.html</br>
圖示： /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
識別碼： marketo_bestbets</br>
標題：首選

   **我的電子郵件**</br>
URL： mkt_/MainViewMyEmail.html</br>
圖示： /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
識別碼： marketo_myemail</br>
標題：我的電子郵件

   **網頁活動**</br>
URL： mkt_/MainViewWebActivity.html</br>
圖示： /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
識別碼： marketo_webactivity</br>
標題：網頁活動

   **匿名網路活動**</br>
URL： mkt_/MainViewWebActivity.html</br>
圖示： /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
識別碼： marketo_anonymous_webactivity</br>
標題：匿名網路活動

1. 完成時，按一下&#x200B;**[!UICONTROL Save]**。
