---
description: 預測性篩選器 — Marketo檔案 — 產品檔案
title: 預測性篩選器
exl-id: 27736b80-cd8b-455d-9d73-c17d492d0906
feature: Predictive Audiences
source-git-commit: 9019cb4b81fb3acd744e644d51059644af454e5e
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# 預測性篩選器 {#predictive-filters}

作為預測對象的一部分，Marketo在智慧行銷活動的智慧清單中提供一組以AI/ML為基礎的篩選器。

![影像1](assets/predictive-filters-1.png)

>[!NOTE]
>
>「可能參加」和「可能註冊」篩選器只能用於事件或電子郵件程式。 「取消訂閱的可能性」、「方案成員的相似程度」和「智慧清單成員的相似程度」可用於所有方案型別。

## 出席的可能性 {#likelihood-to-attend}

此篩選器可有效縮小您的對象範圍。 這有助於您鎖定和邀請具有較高發生頻率的潛在客戶 **出席** 您的網路研討會或活動。 請注意，您的「參加計畫的可能性」將是您目前的活動計畫。

![影像2](assets/predictive-filters-2.png)

## 註冊的可能性 {#likelihood-to-register}

類似於 _出席的可能性_ 篩選，使用此篩選器來縮小對象範圍，並鎖定具有較高發生可能性之潛在客戶 **註冊** 您的網路研討會或活動。

![影像三](assets/predictive-filters-3.png)

## 取消訂閱的可能性 {#likelihood-to-unsubscribe}

依據對象在未來兩週內取消訂閱的可能性高或低，這會篩選對象。 您可以使用此功能，以不同且更有效率的方式鎖定高疲勞銷售機會。 取消訂閱臨界值是動態的，並且由AI模型驅動，該模型會考慮多個屬性，包括資料庫中的前置時間和前置活動。

![影像四](assets/predictive-filters-4.png)

>[!NOTE]
>
>參加/註冊/取消訂閱篩選器的可能性必須與其他標準篩選器結合使用。

## 方案成員的相似對象/智慧清單成員的相似對象 {#lookalike-of-members}

這兩個篩選器可協助您鎖定其他與另一個計畫或智慧清單成員類似的潛在客戶，以擴大目前的對象。 相似篩選器會考慮50多種因素，包括潛在客戶屬性、電子郵件活動、網頁活動和參與。

按一下 **[!UICONTROL 新增限制]** 以選擇所選方案成員的成功標準。

按一下 **+** 圖示可輕鬆將多個程式/智慧列示新增至一個篩選器。

![影像五](assets/predictive-filters-5.png)

## 注意事項 {#things-to-note}

* 即使父方案是在啟用預測篩選器之前建立的，您仍可以將預測篩選器套用至Smart Campaign。
* 預測性篩選器無法用於觸發行銷活動。
* 不支援複製或移動包含預測性篩選器的行銷活動。
* 您可以在「智慧清單」中使用最多5個預測篩選器。
* 如果Marketo Engage在評估預測性篩選器時遇到錯誤，行銷活動執行將自動中止，而您將在Marketo通知中心收到通知。
* 預測篩選器目前的輸入限製為100萬名合格人員。
* 您最多可以有50個使用中的方案包含預測性篩選器。
