---
unique-page-id: 2951103
description: 發行說明 — 2013年2月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2013年2月
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# 發行說明： 2013年2月 {#release-notes-february}

2月版本包含強烈要求的功能、[!DNL Apple Safari]支援和其他小型增強功能。

## [!DNL Apple Safari]的官方支援 {#official-support-for-apple-safari}

Mac和[!DNL Windows]的最新版本[!DNL Apple Safari]完全支援搭配Marketo銷售機會管理使用。 注意： iOS上的[!DNL Safari]不完全相容。

## Webhooks增強功能 {#webhooks-enhancements}

Webhook已增強，以逸出URL/承載中的權杖，也可剖析來自協力廠商系統的XML/JSON回應（無法在[!DNL Spark SMB Edition]中使用）來更新Marketo潛在客戶欄位。

## 已更新SOAP API端點 {#updated-soap-api-endpoint}

更新偏好的SOAP API端點，顯示在[!UICONTROL Admin] -> SOAP API中。 請更新您的呼叫以使用此新端點。 對舊端點的API呼叫已過時，但將繼續運作。 ([!DNL Spark SMB Edition]中不提供SOAP API)

## [!DNL Facebook]索引標籤的行動支援 {#mobile-support-for-facebook-tabs}

從Marketo發佈的[!DNL Facebook]個索引標籤會偵測行動裝置，並將其路由至登陸頁面。 這將確保使用者在不支援[!DNL Facebook]索引標籤的行動裝置上取得正確內容（可在[!DNL Spark]、[!DNL Standard]、[!DNL Select SMB Editions]和[!DNL Marketo Social Marketing]中使用）。

## 即將推出：支援多種模型 {#coming-soon-support-for-multiple-models}

我們正在做基礎工作，以支援多個收入週期模型，並在未來版本中#1社群中投票贊成以RCA的構想。 在此版本中，您會注意到某些變更，包括[智慧清單篩選器，以及在流程步驟](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md)中新增選擇，以支援選取模型和階段。 我們也會將「銷售機會收入階段」和「銷售機會收入週期模型」欄位移出「智慧清單銷售機會網格」標籤。
