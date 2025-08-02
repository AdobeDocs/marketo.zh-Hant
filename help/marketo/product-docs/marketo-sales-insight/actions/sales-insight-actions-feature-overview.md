---
description: 銷售Insight動作功能概觀 — Marketo檔案 — 產品檔案
title: 銷售Insight動作功能概觀
exl-id: 059de248-d1a2-42cd-a7ec-f10b15d0b526
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1305'
ht-degree: 0%

---

# 銷售Insight動作功能概觀 {#msi-actions-feature-overview}

透過行銷支援的智慧和參與工具，使用Sales Insight Actions在單一工作流程中加速潛在客戶搜尋工作。

>[!NOTE]
>
>Marketo Sales Insight Actions是網頁式應用程式，透過[Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}專門與Salesforce CRM整合。 有時稱為「Marketo銷售」，或簡稱為「動作」。

如需銷售Insight動作的影片概觀，[請按一下這裡](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/sales-insight-actions/overview.html?lang=zh-Hant){target="_blank"}。

![](assets/sales-insight-actions-feature-overview-1.png)

## 潛在客戶配置和聯絡人配置 {#lead-layout-and-contact-layout}

頂端導覽列的「選擇動作」下拉式清單中有下列動作：

* 傳送銷售電子郵件
   * 銷售電子郵件具有檢視、點選和回覆追蹤（當設定傳遞管道時）
   * 包括電子郵件Personalization、自訂簽名和附件
   * 範本共用與報告
   * 團隊共用、群組電子郵件和副本/密件副本功能
   * 銷售電子郵件活動將記錄在Marketo個人記錄中
   * Marketo Smart Campaigns中的對應篩選器和觸發器（詳細資訊如下）

* 新增至銷售行銷活動
   * 將潛在客戶新增至銷售教戰手冊，這是一系列電子郵件和任務
   * 包括團隊存取和共用、產生任務、略過週末、忽略回覆的OOO電子郵件以及自動結束
   * 行銷活動將記錄在Marketo人員記錄中
   * Marketo Smart Campaigns中的對應篩選器和觸發器（詳細資訊如下）

* 銷售電話
   * 在CRM內使用撥號器進行銷售通話
   * 包括本機狀態，預先錄製
   * 記錄通話結果、面板中的通話記錄和活動歷史記錄
   * 通話活動將記錄在Marketo人員記錄中
   * Marketo Smart Campaigns中的篩選器和觸發器

* 新增任務
   * 為您的潛在客戶建立電子郵件、通話、InMail和自訂工作
   * 使用Sales Campaigns自動建立任務
   * 與[!DNL Salesforce]同步處理工作
   * 在[!DNL Salesforce] Activity History區段中記錄任務

您可以按一下頂端導覽的((0))圖示來存取即時摘要。 包括檢視銷售活動即時更新的能力，以及熒幕停駐功能。

![](assets/sales-insight-actions-feature-overview-2.png)

以下資料可在MSI面板內的標籤中使用：

* 見解控制面板
   * 參與Velocity格線將包括來自銷售電子郵件、銷售促銷活動動作和銷售電話的活動
   * 即將推出的銷售行銷活動 — 當潛在客戶屬於正在進行的行銷活動時，此資訊將顯示在即將推出的銷售行銷活動標籤中
   * 近期任務 — 當有與潛在客戶相關的近期任務時，此資訊將在近期任務標籤中提供

* 電子郵件索引標籤
   * 所有傳送的銷售電子郵件都會記錄在這裡。 活動也會記錄在Marketo人員記錄中
   * 欄包括主旨、開啟、按一下、已回覆（僅適用於已設定傳送管道的銷售電子郵件）、寄件者、日期
   * 包含投影片輸出卡片，以及寄件者、範本、促銷活動和預覽電子郵件等其他詳細資訊

* 呼叫標籤
   * 使用銷售撥號器功能撥打的所有電話都會記錄在這裡。 活動也會記錄在Marketo人員記錄中
   * 欄包括「名稱」、「結果」、「附註」、「呼叫時間」、「持續時間」和錄製連結
   * 包含投影卡片，以及其他詳細資料，例如來電者、接聽者、電話號碼和狀態

## 帳戶和機會配置 {#account-and-opportunity-layout}

可從頂端導覽取得下列動作：

* 傳送銷售電子郵件 — 能夠傳送個人化或範本化的群組電子郵件，其中包含針對與帳戶/商機相關聯之所有連絡人的檢視、點按及回覆追蹤
   * 銷售電子郵件具有檢視、點選和回覆追蹤（當設定傳遞管道時）
   * 包括電子郵件Personalization、自訂簽名和附件
   * 範本共用與報告
   * 團隊共用、群組電子郵件和副本/密件副本功能
   * 銷售電子郵件活動將記錄在Marketo個人記錄中
   * Marketo Smart Campaigns中的對應篩選器和觸發器（詳細資訊如下）

* 新增至銷售行銷活動 — 將所有與帳戶/機會關聯的連絡人新增至銷售教戰手冊，這是一系列電子郵件和工作
   * 將潛在客戶新增至銷售教戰手冊，這是一系列電子郵件和任務
   * 包括團隊存取和共用、產生任務、略過週末、忽略回覆的OOO電子郵件以及自動結束
   * 行銷活動將記錄在Marketo人員記錄中
   * Marketo Smart Campaigns中的對應篩選器和觸發器（詳細資訊如下）

您可以按一下頂端導覽列中的((0))圖示來存取即時摘要。 包括檢視銷售活動即時更新的能力，以及熒幕停駐功能。

以下資料可在標籤中使用：

* 見解控制面板
   * 參與Velocity格線將包括來自銷售電子郵件、銷售促銷活動動作和銷售電話的活動
   * 即將推出的銷售行銷活動 — 當客戶/商機的連絡人加入進行中的行銷活動時，此資訊將顯示在即將推出的銷售行銷活動標籤中
   * 近期任務 — 當存在與來自帳戶/機會的聯絡人相關的近期任務時，此資訊將可在近期任務標籤中獲得

* 電子郵件索引標籤
   * 所有從帳戶/商機傳送給連絡人的銷售電子郵件都會記錄在這裡。 活動也會記錄在Marketo人員記錄中
   * 欄包括主旨、開啟、按一下、已回覆（僅適用於已設定傳送管道的銷售電子郵件）、寄件者和日期
   * 包含投影片輸出卡片，以及寄件者、範本、促銷活動和預覽電子郵件等其他詳細資訊

* 呼叫標籤
   * 所有使用銷售撥號器功能從客戶/商機撥打給連絡人的電話都會記錄在這裡。 活動也會記錄在Marketo人員記錄中
   * 欄包括名稱、結果、附註、呼叫時間、持續時間和錄製連結
   * 包含投影卡片，以及其他詳細資料，例如來電者、接聽者、電話號碼和狀態

## 潛在客戶與聯絡人清單檢視（大量動作） {#lead-and-contact-list-view}

* [!UICONTROL Send Sales Email] — 能夠傳送包含檢視、點按和回覆追蹤的個人化或範本化電子郵件至聯絡人/潛在客戶清單
* [!UICONTROL Add to Sales Campaign] — 新增到銷售教戰手冊，這是一系列電子郵件和任務到連絡人/潛在客戶清單

## Marketo全域標籤 {#marketo-global-tab}

**[!UICONTROL Best Bets]索引標籤**

![](assets/sales-insight-actions-feature-overview-3.png)

下列大量動作可從[!UICONTROL Best Bets]標籤的下拉式清單中取得：

* [!UICONTROL Send Sales Email] — 可傳送包含檢視、點按及回覆追蹤的個人化或範本化電子郵件
* [!UICONTROL Add to Sales Campaign] — 將銷售機會新增至銷售教戰手冊，這是一系列電子郵件和工作

  ![](assets/sales-insight-actions-feature-overview-4.png)

下列內嵌動作適用於[!UICONTROL Best Bets]標籤中的個別銷售機會/聯絡人：

* [!UICONTROL Send Sales Email] — 可傳送包含檢視、點按及回覆追蹤的個人化或範本化電子郵件
* [!UICONTROL Add to Sales Campaign] — 將銷售機會新增至銷售教戰手冊，這是一系列電子郵件和工作
* [!UICONTROL Sales Call] — 在CRM內使用撥號器進行銷售通話
* [!UICONTROL Add Task] — 為潛在潛在潛在客戶建立電子郵件、通話、客戶或Linkedin工作

  ![](assets/sales-insight-actions-feature-overview-5.png)

**電子郵件索引標籤**

* 所有傳送的銷售電子郵件都會記錄在這裡。 活動也會記錄在Marketo人員記錄中
* 欄包括主旨、開啟、按一下、已回覆（僅適用於已設定傳送管道的銷售電子郵件）、寄件者和日期
* 包含投影片輸出卡片，以及寄件者、範本、促銷活動和預覽電子郵件等其他詳細資訊

**呼叫標籤**

* 使用銷售撥號器功能撥打的所有電話都會記錄在這裡。 活動也會記錄在Marketo人員記錄中
* 欄包括名稱、結果、附註、呼叫時間、持續時間和錄製連結
* 包含投影卡片，以及其他詳細資料，例如來電者、接聽者、電話號碼和狀態

**任務標籤**

* 建立並完成的電子郵件、通話、InMail及自訂工作將可在此標籤中用於工作管理。 包含新增任務的功能
* 使用Sales Campaigns自動建立任務
* 與[!DNL Salesforce]同步處理工作
* 在[!DNL Salesforce] Activity History區段中記錄任務

  ![](assets/sales-insight-actions-feature-overview-6.png)

**即時摘要**

* 可檢視銷售活動的即時更新以及熒幕停駐功能
* 內嵌電子郵件、呼叫和步調按鈕讓每個客戶insight都能操作

## Marketo中可用的功能 {#features-available-in-marketo}

在Marketo中擷取的銷售活動：

* 傳送銷售電子郵件 — 使用者傳送銷售電子郵件給潛在客戶
* 開啟銷售電子郵件 — 潛在客戶開啟已傳送的銷售電子郵件
* 按一下銷售電子郵件 — 潛在客戶按一下銷售電子郵件中的連結
* 已回覆的銷售電子郵件 — 潛在客戶已回覆的銷售電子郵件
* 接聽銷售電話 — 潛在客戶使用銷售電話接聽來自銷售人員的電話。
* Add to Sales Campaign — 將潛在客戶新增至已建立的銷售行銷活動
* 從銷售行銷活動中移除 — 潛在客戶已從建立的銷售行銷活動中移除

篩選器和觸發器包括：

* [!UICONTROL Is Sent Sales Email]
* [!UICONTROL Opens Sales Email]
* [!UICONTROL Clicks Sales Email]
* [!UICONTROL Replies to Sales Email]
* [!UICONTROL Receives Sales Call]
* [!UICONTROL Added to Sales Campaign]
* [!UICONTROL Removed from Sales Campaign]

  ![](assets/sales-insight-actions-feature-overview-7.png)
