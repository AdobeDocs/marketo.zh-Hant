---
unique-page-id: 10096583
description: 新一代Munchkin追蹤常見問答集-Marketo文檔——產品文檔
title: 新一代Munchkin追蹤常見問答集
exl-id: 283189ac-c817-479a-b896-91233980608c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---

# 新一代Munchkin追蹤常見問答集{#next-generation-munchkin-tracking-faq}

我們很高興宣佈，我們即將開始分階段推出新一代Web追蹤技術。

以下是最重要的事項：

* 我們將在第1季度發行（已完成）時移除「匿名」智慧清單篩選器
* 我們正在增加可收錄的網頁事件（瀏覽網頁、網頁上的點按連結）
* 您的Munchkin程式碼不會變更，因此您的網站不需要更新

## 我的Marketo訂閱將於何時推出Munchkin V2?{#when-will-my-marketo-subscription-be-on-munchkin-v}

我們尚未確定確切的日期，但請在這裡查看更新。

## 我是否需要對網站上的Munchkin追蹤進行任何變更？{#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

不。 Munchkin追蹤代碼保持不變。 您的網站不需要進行任何變更。

>[!NOTE]
>
>此變更不會影響網頁個人化（即時個人化）。 它會持續識別匿名和已知的網頁訪客，並即時為這些訪客個人化內容。

## 為什麼Marketo會從智慧型清單中移除「匿名」篩選器？{#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

我們改變了匿名人士與智慧型宣傳互動的方式。 以前，他們像知名人士一樣，通過聰明的宣傳。 「匿名」篩選器可用來指定只有已知或只有匿名人士會在促銷活動中流動。

有了Munchkin V2，我們將繼續追蹤所有匿名活動；但是，您無法再將篩選套用至匿名人員。 在轉換時(當該人在Marketo得知時)，當該人匿名時發生的所有活動都會附加至人員活動記錄，而此時，這些活動會流入他們符合的促銷活動。

如果您已在智慧型清單中使用此篩選器（例如，在智慧型促銷活動或報表中），則不會自動從智慧型清單中移除。 請參閱下方以取得詳細資訊。

>[!NOTE]
>
>**觸發器**:瀏覽網頁，網頁是定價頁面\
>**流量**:變更分數+10和有趣時刻
>**Web**:已查看定價頁
>
>有了Munchkin V2，如果匿名人士造訪定價頁面，她不會立即進入促銷活動。 當匿名人士被知道時，我們會對她進行這項活動。 她會：
>
>* 獲得10分
   >
   >
* 將「網頁」活動設定在正確的日期（她實際造訪時）
   >
   >
* 為她記錄「有趣的時刻」（她實際瀏覽頁面的日期，而不是她知道的日期）
   >
   >
* 記錄「新人員」活動，如今


## 已具有「匿名」篩選器的「智慧型清單」會如何？{#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

在我們的16年冬季發行後，如果您有舊版智慧型促銷活動，其中包含「匿名」篩選器的智慧型清單，將會發生下列兩種情況：

1. 如果智慧型清單的篩選條件為「匿名=假」，則不會發生任何事。 我們只管忽略它。
1. 如果智慧型清單的篩選條件為「匿名=真」，則此促銷活動將失敗，您會收到通知。

## 我用Marketo有段時間了。 我要如何得知哪些促銷活動使用「匿名」篩選？{#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

在進行此項變更之前，我們會以「匿名」篩選條件，將數個每週通知傳送至您的「通知」收件匣，並列出智慧型清單、智慧型促銷活動和報表。 這些功能可協助您識別目前使用此篩選器的位置。

請檢閱並識別您將「匿名」設為「真」的位置，因為這些是受影響的促銷活動。 大多數情況下，客戶都會使用此設定進行某種評分。 請參閱上述範例，瞭解這些促銷活動現在的運作方式。

## 我想要更詳細的檔案。 哪裡可以找到它？{#id-like-more-detailed-documentation-where-can-i-find-it}

查看下列連結：

[匿名銷售機會升級概觀](https://nation.marketo.com/docs/DOC-2937)

[匿名銷售機會升級-MarketoUI內的更改](https://nation.marketo.com/docs/DOC-2938)

[匿名銷售線索升級——需要客戶行動](https://nation.marketo.com/docs/DOC-2939)

[匿名銷售機會升級——分析報表](https://nation.marketo.com/docs/DOC-2940)

[匿名銷售機會升級——發行計畫](https://nation.marketo.com/docs/DOC-2961)

[匿名銷售機會升級- Under The Hood](https://nation.marketo.com/docs/DOC-2962)

[向已知銷售線索的匿名銷售線索促銷- Munchkin V2行為](https://nation.marketo.com/docs/DOC-2963)

## 我還有更多問題！ 我要如何讓他們回答？{#i-have-more-questions-how-do-i-get-them-answered}

請到[社群](https://nation.marketo.com/welcome)。 您也可以聯繫[Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support)。 他們會很樂意回答你的問題。
