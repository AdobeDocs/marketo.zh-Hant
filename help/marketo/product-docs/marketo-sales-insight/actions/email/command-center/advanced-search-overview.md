---
description: 進階搜尋概觀 — Marketo檔案 — 產品檔案
title: 進階搜尋概觀
exl-id: a7cf5078-1d24-4fc0-a82d-02f46f93893d
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 2%

---

# 進階搜尋概觀 {#advanced-search-overview}

透過使用進階搜尋來鎖定已檢視、按一下或回覆電子郵件的潛在客戶，您可以建立最常參與潛在客戶的目標清單。

## 如何存取進階搜尋 {#how-to-access-advanced-search}

1. 在網頁應用程式中，按一下&#x200B;**[!UICONTROL Command Center]**。

   ![](assets/advanced-search-overview-1.png)

1. 按一下「**[!UICONTROL Emails]**」。

   ![](assets/advanced-search-overview-2.png)

1. 選擇適用的標籤。

   ![](assets/advanced-search-overview-3.png)

1. 按一下「[!UICONTROL Advanced Search]」。

   ![](assets/advanced-search-overview-4.png)

## 篩選器 {#filters}

**日期**

選擇搜尋的日期範圍。 預設日期會根據您選擇的電子郵件狀態([!UICONTROL Sent]、[!UICONTROL Undelivered]、[!UICONTROL Pending])而更新。

![](assets/advanced-search-overview-5.png)

**誰**

在[!UICONTROL Who]區段中依電子郵件收件者/寄件者篩選。

![](assets/advanced-search-overview-6.png)

<table>
 <tr>
  <td><strong>下拉式清單</strong></td>
  <td><strong>說明</strong></td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL View As]</strong></td>
  <td>在您的Sales Connect執行個體中依特定寄件者篩選（此選項僅供管理員使用）。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL By Group]</strong></td>
  <td>依特定收件者群組篩選電子郵件。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL By Person]</strong></td>
  <td>依特定收件者篩選。</td>
 </tr>
</table>

**時間**

依建立日期、傳送日期、失敗日期或排程日期選擇。 可用選項會根據您選擇的電子郵件狀態而變更([!UICONTROL Sent]、[!UICONTROL Undelivered]、[!UICONTROL Pending])。

![](assets/advanced-search-overview-7.png)

**行銷活動**

依行銷活動參與率篩選電子郵件。

![](assets/advanced-search-overview-8.png)

**狀態**

有三個電子郵件狀態可供選擇。 型別/活動選項會根據選取的狀態而變更。

![](assets/advanced-search-overview-9.png)

_&#x200B;**狀態：已傳送**&#x200B;_

![](assets/advanced-search-overview-10.png)

依您傳送的電子郵件活動篩選。 您可以選擇[!UICONTROL views]/[!UICONTROL no views]、[!UICONTROL clicks]/[!UICONTROL no clicks]和/或[!UICONTROL replies]/[!UICONTROL no replies]。

_&#x200B;**狀態：擱置中**&#x200B;_

![](assets/advanced-search-overview-11.png)

依所有待處理電子郵件篩選。

<table>
 <tr>
  <td><strong>狀態</strong></td>
  <td><strong>說明</strong></td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL Scheduled]</strong></td>
  <td>已從撰寫視窗(Salesforce或Web應用程式)、電子郵件外掛程式或促銷活動排程的電子郵件。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL Drafts]</strong></td>
  <td>目前處於草稿狀態的電子郵件。 電子郵件需要主旨行和收件者才能儲存為草稿。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL In Progress]</strong></td>
  <td>正在傳送的電子郵件。 電子郵件不應維持此狀態超過數秒鐘。</td>
 </tr>
</table>

_&#x200B;**狀態：未傳遞**&#x200B;_

![](assets/advanced-search-overview-12.png)

根據從未傳遞的電子郵件進行篩選。

<table>
 <tr>
  <td><strong>狀態</strong></td>
  <td><strong>說明</strong></td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL Failed]</strong></td>
  <td>當電子郵件無法從Sales Connect傳送時（常見原因包括：電子郵件會傳送給已取消訂閱/遭到封鎖的連絡人，或是在填入動態欄位時發生問題）。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL Bounced]</strong></td>
  <td>收件者的伺服器拒絕電子郵件時，該電子郵件會標示為已退回。 此處只會顯示透過Sales Connect伺服器傳送的電子郵件。</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL Spam]</strong></td>
  <td>收件者將電子郵件標示為垃圾訊息時（未經請求的電子郵件的常見詞語）。 此處只會顯示透過Sales Connect伺服器傳送的電子郵件。</td>
 </tr>
</table>

## 已儲存的搜尋 {#saved-searches}

以下說明如何建立已儲存的搜尋。

1. 所有篩選器都就緒後，按一下&#x200B;**[!UICONTROL Save Filters As]**。

   ![](assets/advanced-search-overview-13.png)

1. 提供搜尋名稱，然後按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/advanced-search-overview-14.png)

您已儲存的搜尋會顯示在左側的側邊欄中。

![](assets/advanced-search-overview-15.png)
