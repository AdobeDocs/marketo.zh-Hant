---
unique-page-id: 10096583
description: 有關新一代 [!DNL Munchkin] 追蹤轉出和Is Anonymous篩選器變更的常見問題集。
title: 新一代 [!DNL Munchkin] 追蹤常見問題集
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
hidefromtoc: true
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# 新一代[!DNL Munchkin]追蹤常見問題集 {#next-generation-munchkin-tracking-faq}

Marketo正分階段推出新一代網路追蹤技術。

以下是最重要的須知事項：

* 已移除「為匿名」智慧清單篩選器
* Marketo可擷取的網頁事件數量（瀏覽網頁、點選網頁上的連結）正在增加
* 您的[!DNL Munchkin]程式碼不會變更，因此不需要更新您的網站

## 我的Marketo訂閱何時會在[!DNL Munchkin] V2上進行？ {#when-will-my-marketo-subscription-be-on-munchkin-v}

尚未提供確切日期。 檢查此頁面是否有更新。

## 我是否需要變更網站上的[!DNL Munchkin]追蹤？ {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

否。 [!DNL Munchkin]追蹤程式碼維持不變。 您的網站不需要任何變更。

>[!NOTE]
>
>此變更不會影響網頁Personalization （即時Personalization）。 它會持續識別匿名與已知網路訪客，並即時為這些訪客個人化內容。

## Marketo為何從智慧清單移除「為匿名」篩選器？ {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Marketo已變更匿名人員與Smart Campaigns互動的方式。 過去，他們過著智慧的行銷活動，就像已知人一樣。 「為匿名」篩選器用於指定只有已知或僅匿名人員會通過行銷活動。

透過[!DNL Munchkin] V2，Marketo將繼續追蹤所有匿名活動；不過，您無法再對匿名人員套用篩選器。 在轉換點（在Marketo中知道人員時），當人員匿名時發生的所有活動都會附加至人員活動記錄，並且在這個時候會流經他們符合資格的促銷活動。

如果您已在智慧清單中使用此篩選器（例如，在智慧行銷活動或報表中），則不會自動從智慧清單中移除此篩選器。 如需更多詳細資訊，請參閱下文。

>[!NOTE]
>
>**觸發器**：瀏覽網頁，網頁為定價頁面&#x200B;>**流量**：變更分數+10和有趣的時刻&#x200B;>**Web**：已檢視的定價頁面
>
>使用[!DNL Munchkin] V2時，如果匿名人員造訪定價頁面，他們不會立即進入行銷活動。 在匿名人士成為已知人時，Marketo會對其執行此促銷活動。 他們會：
>
>* 取得10分
>
>* 將網頁活動設定為正確的日期（實際造訪的日期）
>
>* 為他們記錄了一個有趣的時刻（包含他們實際造訪頁面的日期，而不是他們得知的時間）
>
>* 如今天般記錄「新人員」活動

## 如果我的智慧清單已有「匿名」篩選器，會發生什麼事？ {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

在2016年冬季發行版本之後，如果您有包含智慧清單的舊智慧行銷活動，且其中包含「為匿名」篩選器，將會發生以下兩種情況之一：

1. 如果「智慧列示」具有篩選器「Is Anonymous = False」，則不會發生任何動作。 會予以忽略。
1. 如果「智慧清單」具有「為匿名= True」篩選條件，此行銷活動將會失敗並傳送通知。

## 我使用Marketo已經有一段時間了。 我如何知道我的哪些行銷活動使用「匿名」篩選器？ {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

在此變更前，Marketo會傳送數個每週通知至您的「通知」收件匣，其中包含使用「匿名」篩選器的智慧清單、智慧行銷活動和報告的清單。 這些功能可協助您識別目前使用此篩選器的位置。

請檢閱這些資訊，並識別將「匿名」設為「True」的位置，因為這些是受影響的行銷活動。 大多數情況下，此設定會用於某種型別的評分。 請參閱上述範例，瞭解這些行銷活動現在將如何運作。

## 我想要更詳細的檔案。 我可以在哪裡找到它？ {#id-like-more-detailed-documentation-where-can-i-find-it}

檢視下列連結：

[匿名潛在客戶升級概觀](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[匿名銷售機會升級 — Marketo UI中的變更](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[匿名銷售機會升級 — 需要客戶動作](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[匿名銷售機會升級 — Analytics報表](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[匿名銷售機會升級 — 發行排程](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[匿名銷售機會升級 — 隱秘的](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[匿名銷售機會促銷給已知銷售機會 —  [!DNL Munchkin] V2行為](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## 我有更多問題！ 如何獲得解答？ {#i-have-more-questions-how-do-i-get-them-answered}

造訪[Marketo社群](https://experienceleaguecommunities.adobe.com/){target="_blank"}。 您也可以聯絡Marketo支援。 他們很高興回答您的問題。
