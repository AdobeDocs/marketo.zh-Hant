---
unique-page-id: 10096583
description: 新一代Munchkin跟蹤常見問題 — Marketo文檔 — 產品文檔
title: 新一代Munchkin跟蹤常見問題
exl-id: 283189ac-c817-479a-b896-91233980608c
source-git-commit: 6ad418c8f4056b9a2fb31b0ac995692f0c618795
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# 新一代Munchkin跟蹤常見問題 {#next-generation-munchkin-tracking-faq}

我們很高興地宣佈，我們將很快開始分階段推出下一代網路跟蹤技術。

以下是最重要的資訊：

* 我們正在刪除第1季度發佈時的「匿名」智慧清單篩選器（已完成）
* 我們正在增加可以接收的Web事件數（訪問網頁、按一下網頁連結）
* 您的Munchkin代碼不會更改，因此不需要在您的網站上更新

## 我的Marketo訂購何時在Munchkin V2上？ {#when-will-my-marketo-subscription-be-on-munchkin-v}

我們還沒有確切的日期，但請在此處查看更新。

## 是否需要對網站上的Munchkin跟蹤進行任何更改？ {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

不。 蒙奇金跟蹤代碼保持不變。 無需對您的網站進行任何更改。

>[!NOTE]
>
>此更改不影響WebPersonalization(即時Personalization)。 它繼續識別匿名和已知的網路訪問者，並對這些訪問者即時個性化內容。

## 為什麼Marketo從智慧清單中刪除「匿名」篩選器？ {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

我們改變了匿名者與智慧營銷互動的方式。 以前，他們像知名人一樣，通過一場聰明的競選。 「Is Anonymous」過濾器用於指定只有已知或只有匿名人員才能通過市場活動。

通過Munchkin V2，我們將繼續跟蹤所有匿名活動；但是，您不再能對匿名用戶應用篩選器。 在轉換點(當該人在Marketo已知時)，在該人匿名時發生的所有活動都附加在人員活動日誌中，此時，這些活動會通過他們有資格參加的活動。

如果您已在智慧清單中使用此篩選器（例如，在智慧市場活動或報表中），則不會自動從智慧清單中刪除該篩選器。 有關詳細資訊，請參閱下面。

>[!NOTE]
>
>**觸發器**:訪問網頁，網頁是定價頁\
>**流**:更改分數+10和有趣時刻
>**Web**:已查看定價頁
>
>使用Munchkin V2 ，如果匿名人員訪問定價頁，她不會立即進入市場活動。 當匿名者被認識時，我們會針對她開展這項活動。 她會：
>
>* 得10分
>
>* 將網頁活動設定為正確日期（她實際訪問時）
>
>* 為她記錄一個有趣的時刻（她實際訪問該頁面的日期，而不是她知道的日期）
>
>* 記錄「新人」活動（如今）


## 已具有「匿名」篩選器的智慧清單會如何？ {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

在我們的16年冬季發佈後，如果您有舊的智慧活動清單，其中包含「匿名」過濾器，則將發生以下兩種情況之一：

1. 如果智慧清單具有篩選器「Is Anonymous = False」，則不會發生任何情況。 我們就別管了。
1. 如果智慧清單具有篩選器「匿名=真」，則此市場活動將失敗，您將收到通知。

## 我用Marketo有段時間了。 我如何知道我的哪些活動使用「匿名」過濾器？ {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

在進行此更改之前，我們每週會向您的通知收件箱發送幾次通知，其中包含使用「匿名」過濾器的智慧清單、智慧市場活動和報告清單。 這些功能可幫助您確定當前使用此篩選器的位置。

請查看它們，並確定「匿名」設定為True的位置，因為這些是受影響的市場活動。 大多數情況下，客戶使用此設定進行某種評分。 請參見上面的示例，瞭解這些活動現在將如何運行。

## 我想要更詳細的文檔。 我在哪裡能找到它？ {#id-like-more-detailed-documentation-where-can-i-find-it}

查看以下連結：

[匿名銷售線索升級概述](https://nation.marketo.com/docs/DOC-2937)

[匿名線索升級 — MarketoUI內的更改](https://nation.marketo.com/docs/DOC-2938)

[匿名線索升級 — 需要客戶行動](https://nation.marketo.com/docs/DOC-2939)

[匿名線索升級 — 分析報告](https://nation.marketo.com/docs/DOC-2940)

[匿名銷售線索升級 — 發佈計畫](https://nation.marketo.com/docs/DOC-2961)

[匿名線索升級 — 引擎蓋下](https://nation.marketo.com/docs/DOC-2962)

[匿名Lead升級到已知Lead - Munchkin V2行為](https://nation.marketo.com/docs/DOC-2963)

## 我還有問題要問！ 我怎樣才能得到答案？ {#i-have-more-questions-how-do-i-get-them-answered}

請伸手 [社區](https://nation.marketo.com/)。 您也可以聯繫 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support)。 他們會很樂意回答你的問題。
