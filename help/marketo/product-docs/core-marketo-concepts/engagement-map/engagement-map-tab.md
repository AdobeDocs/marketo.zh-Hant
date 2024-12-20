---
description: 參與地圖示籤 — Marketo檔案 — 產品檔案
title: 參與地圖示籤
exl-id: 8c4d076a-d8aa-44ff-b538-ca6a6778697a
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# 參與地圖示籤 {#engagement-map-tab}

參與地圖會透過一系列觸發器、篩選器和流量卡來表示。 按一下每個卡片就會顯示其他資訊。

觸發器概覽：此卡片顯示促銷活動中的觸發器數量。 按一下卡片就會顯示每個觸發器的卡片，以及提供下列資訊的滑出面板：

* 觸發器所屬的行銷活動
* 觸發器名稱清單
* 編輯觸發器

  ![](assets/engagement-map-tab-1.png)

觸發程式詳細資料：此卡片會顯示觸發程式名稱。 按一下滑出畫面會顯示包含下列資訊的滑出面板：

* 觸發器所屬的行銷活動
* 與觸發程式關聯的限制清單
* 編輯觸發器

篩選：按一下此卡片將顯示一個包含下列資訊的滑出面板：

* 篩選器所屬的行銷活動
* 符合篩選條件的預估人數
* 篩選器清單及其個別限制
* 編輯篩選器

  ![](assets/engagement-map-tab-3.png)

流程步驟：如果「流程步驟」包含選項，此卡片會顯示「流程步驟」的名稱。 按一下滑出畫面會顯示包含下列資訊的滑出面板：

* 流程步驟所屬的行銷活動
* 與流程步驟相關的選擇條件清單
* 編輯流程步驟

流程步驟：如果流程步驟&#x200B;_不_&#x200B;包含任何選擇，此卡片將顯示與流程步驟相關的屬性。 按一下滑出畫面會顯示包含下列資訊的滑出面板：

* 流程步驟所屬的行銷活動
* 與「流程步驟」相關聯的屬性清單
* 編輯流程步驟

  ![](assets/engagement-map-tab-5.png)

## 執行和請求行銷活動的流程步驟 {#flow-step-for-execute-and-request-campaigns}

* 如果「執行」或「請求促銷活動流程步驟」不含任何選項，資訊卡會顯示促銷活動名稱。 按一下卡片會顯示一個包含下列資訊的滑出面板：

   * 流程步驟所屬的行銷活動
   * 編輯流程步驟
   * 與「流程步驟」相關聯的屬性清單
   * 「檢視清單」按鈕可開啟使用特定請求/執行行銷活動的行銷活動清單

>[!NOTE]
>
>您可以從主要行銷活動中編輯流量步驟。 若要編輯巢狀行銷活動，您必須透過滑出面板中的連結導覽至行銷活動。

* 如果執行或請求促銷活動流程步驟包含選項，按一下卡片即會顯示提供下列資訊的滑出面板：

   * 流程步驟所屬的行銷活動
   * 與流程步驟相關的選擇條件清單
   * 編輯流程步驟

* 如果「執行」或「請求促銷活動」包含選項，則按一下流量卡片即會展開，以顯示個別卡片中的所有選項。 按一下&#x200B;_選擇_&#x200B;卡片會展開與特定選擇相關聯的促銷活動，並顯示包含下列資訊的滑出面板：

   * 選擇所屬的行銷活動
   * 編輯選擇
   * 與流程步驟相關的選擇條件清單
   * 檢視清單，這會開啟使用特定請求/執行行銷活動的行銷活動清單

  ![](assets/engagement-map-tab-10.png)

## 將巢狀執行行銷活動視覺化 {#visualizing-a-nested-execute-campaign}

執行與父行銷活動連續執行的行銷活動。 符合可執行行銷活動資格的人會完成行銷活動的所有流程步驟，然後返回主要行銷活動，以繼續完成此行銷活動的流程步驟。

以下是智慧行銷活動「行銷活動A」的範例，其中包括執行行銷活動流程步驟。 請將「促銷活動A」視為您的主要促銷活動。

![](assets/engagement-map-tab-11.png)

1. 按一下執行行銷活動流量卡片將會展開，以顯示「行銷活動B」的詳細資訊。
1. 「促銷活動B」包含篩選器，可將受眾分割成兩個群組：合格和未合格。
1. 合格對象會完成與「促銷活動B」相關的流程步驟。
1. 所有對象（合格且非合格）會回到「行銷活動A」並繼續進行下一個流程步驟。

   ![](assets/engagement-map-tab-12.png)

您可以按一下「行銷活動B」中的執行行銷活動流程步驟，其將展開以顯示與每個選擇相關聯的選擇卡和行銷活動。

![](assets/engagement-map-tab-13.png)

## 將請求行銷活動視覺化 {#visualizing-request-campaign}

請求行銷活動與父行銷活動平行執行。 符合請求行銷活動資格的人完成行銷活動的所有流程步驟，然後退出行銷活動。 同時，同一組人員會通過主要促銷活動的「流量步驟」。

以下是智慧行銷活動「行銷活動A」的範例，其中包括請求行銷活動流程步驟。 請將「促銷活動A」視為您的主要促銷活動。

![](assets/engagement-map-tab-14.png)

1. 按一下請求行銷活動流量卡片將會展開，以顯示「行銷活動B」的詳細資料
1. 「促銷活動B」包含篩選器，可將受眾分割成兩個群組：合格和未合格。
1. 合格對象會完成與「促銷活動B」相關的流程步驟。
1. 同時，所有對象會移至「促銷活動A」中的下一個流量步驟。

   ![](assets/engagement-map-tab-15.png)

如果任何流量步驟包含其他請求行銷活動，您可以按一下流量卡片來檢視行銷活動的詳細資訊，以深入瞭解巢狀行銷活動。

![](assets/engagement-map-tab-16.png)

以下是包含選擇的請求行銷活動的範例。

![](assets/engagement-map-tab-17.png)

## 錯誤處理 {#error-handling}

智慧列示和流量步驟中的錯誤會透過卡片中的紅色圖示醒目提示。 此外，對應的錯誤訊息將會反映在滑出面板中。

智慧清單和流量步驟中的警告會透過卡片中的橘色圖示強調顯示。 此外，對應的警告訊息也會反映在滑出面板中。

以下是「選擇」卡片中的警告範例，該卡片會顯示在「執行Campaign」流程步驟卡片、滑出面板和「預設」選擇卡片中。

![](assets/engagement-map-tab-18.png)

>[!NOTE]
>
>警告是可檢閱的建議，但並不表示Smart Campaign發生錯誤。

**篩選器卡片中的錯誤可能包括：**

* 智慧清單中發生錯誤，導致未顯示合格對象

* 篩選器邏輯發生錯誤

* 一或多個篩選器中的限制（或缺少限制）發生錯誤

  ![](assets/engagement-map-tab-20.png)

>[!NOTE]
>
>在您按一下以展開巢狀行銷活動之前，巢狀行銷活動中的錯誤不會顯示。
