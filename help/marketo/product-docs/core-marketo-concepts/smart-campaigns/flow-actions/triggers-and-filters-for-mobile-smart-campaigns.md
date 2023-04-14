---
unique-page-id: 9437991
description: 行動智慧行銷活動的觸發器和篩選器 — Marketo檔案 — 產品檔案
title: 行動智慧型行銷活動的觸發器和篩選器
exl-id: 76fc7a74-b27d-4898-a8ca-85c9c2828a28
source-git-commit: 98eac847e62df1e17a6abefde0f9097b12cbbf9c
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# 行動智慧型行銷活動的觸發器和篩選器 {#triggers-and-filters-for-mobile-smart-campaigns}

您可以為行動應用程式智慧型行銷活動設定觸發器和篩選器。

對於大部分活動，會有觸發器、篩選器和閒置篩選器。 使用不活動篩選器來追蹤動作，例如點選推播通知 *didn&#39;t* 發生。

* 已安裝/已安裝行動應用程式
* 已開啟行動應用程式
* 有/有行動應用程式活動
* 有/有行動應用程式工作階段
* 點選/點選行動推播通知

只有此活動的篩選器：

* 已傳送推播通知 — 篩選和閒置篩選

搜尋 **行動應用程式** 列出所有行動應用程式觸發器和篩選器。

![](assets/triggers-and-filters-for-mobile-smart-campaigns-1.png)

## 限制 {#constraints}

使用觸發器和篩選器的限制來進一步排序資料。

![](assets/triggers-and-filters-for-mobile-smart-campaigns-2.png)

除「已傳送推播通知」外，所有觸發器和篩選器都包含以下兩個標準限制：

* 裝置類型 — iPod、iPhone、iPhone 6 Plus、iPad mini、iPad、Android智慧型手機、Android平板電腦、未知（此為預設清單）

* 平台 — iPhone或Android

有些觸發器和篩選器提供其他限制，例如：

* 應用程式版本 — 鎖定非最新版本使用者的方式。 例如，如果最新應用程式版本為2.0，您便可使用它來尋找未使用應用程式版本2.0的使用者

* 安裝來源 — 目前，唯一的選項是API

* 地區設定 — 裝置上的設定

* 行動應用程式 — 特定應用程式的名稱。 指定是否有多個

* 平台版本 — 作業系統版本

* 工作階段長度（秒） — 應用程式於前景時的工作階段時間

* 是否啟用推送 —  **True** 表示可傳送推播通知。 **False** 意味著他們不能。例如，該人員可能已選擇退出接收推播通知

## 觸發器和篩選器 {#triggers-and-filters}

**有行動應用程式**

使用此篩選器來找出所有已安裝您應用程式的使用者。 這只能當作篩選器使用。

>[!NOTE]
>
>篩選器會找出目前和之前的安裝，因為Marketo不會追蹤應用程式的卸載。

**限制**:裝置類型、平台、行動應用程式、行動應用程式版本、裝置類型、安裝來源、已啟用推送，且地區設定

![](assets/triggers-and-filters-for-mobile-smart-campaigns-3.png)

>[!TIP]
>
>在定義應接收推播通知的智慧清單時，最佳作法是指定「行動應用程式= true」和「已啟用推播」= true，以及行動應用程式的名稱。

已安裝/已安裝行動應用程式

* 已安裝行動應用程式 — 觸發器

* 已安裝行動應用程式 — 篩選器

* 未安裝行動應用程式 — 閒置篩選器

**限制**:裝置類型、平台、應用程式版本、地區設定和安裝來源

![](assets/triggers-and-filters-for-mobile-smart-campaigns-4.png)

已開啟行動應用程式

* 行動應用程式已開啟 — 觸發器

* 行動應用程式已開啟 — 篩選器

* 未開啟行動應用程式 — 閒置篩選器

**限制**:裝置類型與平台

![](assets/triggers-and-filters-for-mobile-smart-campaigns-5.png)

有/有行動應用程式活動

這些提供強大的方式來追蹤自訂行動活動。 您需要與開發人員合作以設定追蹤 [Android適用](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android) 和 [針對iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios).

* 有行動應用程式活動 — 觸發器

* 有行動應用程式活動 — 篩選

* 沒有行動應用程式活動 — 閒置篩選器

**限制**:裝置類型和平台，再加上5個額外類型：

* 動作 — 自訂行動活動

* 動作類型 — （選用）用來分類多個動作的文字欄位

* 動作詳細資料 — （選用）文字欄位，提供動作的其他資訊

* 動作量度 — （選用）數值欄位，提供動作（例如價格）的其他資訊

* 動作長度（秒） — （選用）數值欄位，可用來擷取使用者完成動作所花的時間

動作限制可讓您使用觸發器和篩選器來非常密切地追蹤行動活動。

>[!NOTE]
>
>**範例**
>
>在 *購物*，此為非常特定的動作，其他限制會定義它：
>
>* 買了件襯衫
   >   * 是紅色的
   >   * 它花了30美元
   >   * 花了20秒才買的


以下是Marketo中篩選器的外觀：

![](assets/triggers-and-filters-for-mobile-smart-campaigns-6.png)

>[!NOTE]
>
>**範例**
>
>在相同的動作類型下可以有多個動作。 事實上，您一般的購物體驗可能會包含「購物」下的數個欄！ 要不要穿襪子？
>
>| 動作類型 | 購物 | 購物 |
>|---|---|---|
>| 動作 | 購買的襯衫 | 買褲子 |
>| 動作詳細資料 | 顏色 | 顏色 |
>| 動作量度 | 價格 | 價格 |


**有/有行動應用程式工作階段**

* 有行動應用程式工作階段 — 觸發器

* 有行動應用程式工作階段 — 篩選器

* 沒有行動應用程式工作階段 — 閒置篩選

**限制**:裝置類型、平台和工作階段長度（秒）

![](assets/triggers-and-filters-for-mobile-smart-campaigns-7.png)

點選/點選推播通知

* 點選推播通知 — 觸發器

* 點選推播通知 — 篩選

* 未點選推播通知 — 閒置篩選

**限制**:裝置類型、平台、行動應用程式版本、推播通知和平台版本

![](assets/triggers-and-filters-for-mobile-smart-campaigns-8.png)

>[!TIP]
>
>使用「未點選推播通知」閒置篩選器，尋找最近未點選傳送給他們的推播通知的使用者，以便您透過電子郵件追蹤。

**已傳送推播通知** 此活動僅作為篩選器可用。

* 已傳送推播通知 — 篩選

* 未傳送推播通知 — 閒置篩選器

**限制**:推播通知和行動應用程式

![](assets/triggers-and-filters-for-mobile-smart-campaigns-9.png)

>[!MORELIKETHIS]
>
>* [向智慧清單篩選器添加約束](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)
>* [在智慧清單中使用不活動篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

