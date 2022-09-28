---
unique-page-id: 10096583
description: 新一代Munchkin追蹤常見問題集 — Marketo檔案 — 產品檔案
title: 新一代Munchkin追蹤常見問題集
exl-id: 283189ac-c817-479a-b896-91233980608c
source-git-commit: 813bab6169a121e90919f9a02505ccde5167cda4
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# 新一代Munchkin追蹤常見問題集 {#next-generation-munchkin-tracking-faq}

我們很高興能宣佈，我們即將開始分階段推出新一代網頁追蹤技術。

以下是最重要的事項：

* 我們正在第1季版本中移除「匿名」智慧清單篩選器（已完成）
* 我們正在增加可擷取的網頁事件（瀏覽網頁、網頁上的點按連結）數量
* 您的Munchkin程式碼不會變更，因此不需要更新您的網站

## 我的Marketo訂閱將於何時上線Munchkin V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

我們尚未確定確切的日期，但請返回這裡查看更新。

## 我是否需要對網站上的Munchkin追蹤進行任何變更？ {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

否. Munchkin追蹤程式碼維持不變。 您的網站無需進行任何變更。

>[!NOTE]
>
>此變更不會影響網站個人化（即時個人化）。 它會持續識別匿名和已知的網站訪客，並對這些訪客即時個人化內容。

## Marketo為何從智慧清單中移除「匿名」篩選器？ {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

我們已變更匿名人員與智慧行銷活動互動的方式。 以前，他們像已知人一樣，通過了一場聰明的運動。 「是匿名的」篩選條件可用來指定只有已知或只有匿名的訪客會透過促銷活動。

有了Munchkin V2，我們將繼續追蹤所有匿名活動；但是，您無法再將篩選器套用至匿名人員。 轉換時(當人員在Marketo中已知)，當該人員匿名時發生的所有活動都會附加至人員活動記錄，而此時這些活動會流經他們符合資格的促銷活動。

如果您已在智慧清單中使用此篩選器（例如，在智慧促銷活動或報表中），則不會從智慧清單中自動移除它。 如需詳細資訊，請參閱下方。

>[!NOTE]
>
>**觸發**:瀏覽網頁、網頁為定價頁面\
>**流量**:更改分數+10和有趣時刻
>**Web**:已查看定價頁
>
>若使用Munchkin V2，如果匿名人員造訪定價頁面，她不會立即進入促銷活動。 當匿名者被知道時，我們會對她進行這場運動。 她會：
>
>* 得10分
>
>* 將網頁活動設為正確的日期（她實際造訪的時間）
>
>* 為她記錄「有趣的時刻」（她實際瀏覽頁面的日期，而不是她成為知名的日期）
>
>* 記錄「新人員」活動，如今


## 已有「匿名」篩選器的智慧清單有什麼改變？ {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

在』16年冬季發行後，如果您有舊版智慧型行銷活動，其中包含「匿名」篩選條件的智慧清單，將會發生下列兩種情況之一：

1. 如果智慧清單的篩選器為「Is Anonymous = False」，則不會發生任何情況。 我們就忽略它。
1. 如果智慧清單的篩選器為「Is Anonymous = True」，則此促銷活動會失敗，您會收到通知。

## 我用了Marketo一段時間了。 如何知道哪些促銷活動使用「匿名」篩選器？ {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

在進行此變更前，我們會先將數個每週通知傳送至您的通知收件匣，內含使用「匿名」篩選條件的智慧清單、智慧促銷活動和報表清單。 這些功能可協助您識別目前使用此篩選器的位置。

請檢閱這些行銷活動，並識別您將「匿名」設為True的位置，因為這些是受影響的行銷活動。 大多數情況下，客戶會使用此設定進行某種計分。 請參閱上述範例，了解這些促銷活動現在的運作方式。

## 我想要更詳細的檔案。 在哪裡可以找到它？ {#id-like-more-detailed-documentation-where-can-i-find-it}

查看下列連結：

[匿名銷售機會升級概述](https://nation.marketo.com/docs/DOC-2937){target=&quot;_blank&quot;}

[匿名銷售機會升級 — Marketo UI內的變更](https://nation.marketo.com/docs/DOC-2938){target=&quot;_blank&quot;}

[匿名銷售機會升級 — 需要客戶操作](https://nation.marketo.com/docs/DOC-2939){target=&quot;_blank&quot;}

[匿名銷售機會升級 — Analytics報表](https://nation.marketo.com/docs/DOC-2940){target=&quot;_blank&quot;}

[匿名銷售機會升級 — 發行計畫](https://nation.marketo.com/docs/DOC-2961){target=&quot;_blank&quot;}

[匿名銷售機會升級 — 在Hood下](https://nation.marketo.com/docs/DOC-2962){target=&quot;_blank&quot;}

[匿名銷售機會促銷至已知銷售機會 — Munchkin V2行為](https://nation.marketo.com/docs/DOC-2963){target=&quot;_blank&quot;}

## 我還有更多問題！ 我該如何得到他們的回答？ {#i-have-more-questions-how-do-i-get-them-answered}

請到 [社群](https://nation.marketo.com/){target=&quot;_blank&quot;}。 您也可以聯絡 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support){target=&quot;_blank&quot;}。 他們會很樂意回答你的問題。
