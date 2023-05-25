---
unique-page-id: 10096583
description: 「新一代 [!DNL Munchkin] 追蹤常見問題集 — Marketo檔案 — 產品檔案」
title: 「新一代 [!DNL Munchkin] 追蹤常見問題集」
exl-id: 283189ac-c817-479a-b896-91233980608c
source-git-commit: 1a6f029b8c9665ecd7fcc066004d88ee6c915505
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---

# 新一代 [!DNL Munchkin] 追蹤常見問題集 {#next-generation-munchkin-tracking-faq}

我們很高興宣佈，我們即將分階段推出新一代的網路追蹤技術。

以下是最重要的須知事項：

* 我們正在第1季版本中移除「匿名」智慧清單篩選器（已完成）
* 我們正增加可擷取的網頁事件數量（造訪網頁、網頁上的點選連結）
* 您的 [!DNL Munchkin] 程式碼不會變更，因此您不需要更新網站

## 我的Marketo訂閱將於何時開啟 [!DNL Munchkin] V2？ {#when-will-my-marketo-subscription-be-on-munchkin-v}

我們還沒有確切日期，但請回到這裡檢視更新。

## 我是否需要變更我的 [!DNL Munchkin] 在我的網站上進行追蹤？ {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

否. 此 [!DNL Munchkin] 追蹤程式碼保持不變。 您的網站不需要任何變更。

>[!NOTE]
>
>此變更不會影響網頁個人化（即時個人化）。 它會持續識別匿名和已知的網頁訪客，並即時對這些訪客個人化內容。

## Marketo為何從智慧清單移除「為匿名」篩選器？ {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

我們已變更匿名人員與Smart Campaigns的互動方式。 過去，他們就像已知人一樣，經常在智慧型行銷活動中穿梭。 「匿名」篩選器用於指定只有已知或只有匿名人員會流經促銷活動。

替換為 [!DNL Munchkin] V2，我們將繼續追蹤所有匿名活動，但您無法再套用篩選器至匿名人員。 轉換時(在Marketo中認識該人員時)，該人員匿名時發生的所有活動都會附加至該人員活動記錄，且此時會流經他們符合資格的促銷活動。

如果您已在智慧清單中使用此篩選器（例如，在智慧行銷活動或報表中），則不會自動將其從智慧清單中移除。 如需更多詳細資訊，請參閱下文。

>[!NOTE]
>
>**觸發**：瀏覽網頁，網頁為定價頁面\
>**流量**：變更分數+10和有趣的時刻
>**Web**：已檢視的定價頁面
>
>替換為 [!DNL Munchkin] V2，如果匿名人員造訪定價頁面，她不會立即進入促銷活動。 當匿名人士成為已知人時，我們會針對她進行此行銷活動。 她將：
>
>* 獲得10分
>
>* 將網頁活動設定為正確的日期（她實際造訪的日期）
>
>* 為她記錄一個「有趣的時刻」 （記錄她實際瀏覽頁面的日期，而不是她成名的日期）
>
>* 像今天一樣記錄「新人員」活動


## 已具有「匿名」篩選器的智慧清單會有什麼改變？ {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

在2016年Winter版本發行後，如果您有包含智慧清單的舊智慧行銷活動，且其中包含「匿名」篩選器，將會發生以下兩種情況之一：

1. 如果智慧清單具有「匿名= False」篩選器，則不會發生任何事情。 我們將忽略它。
1. 如果智慧清單具有「匿名= True」篩選器，則此行銷活動將失敗，並會向您傳送通知。

## 我已經使用Marketo一段時間了。 我如何知道我的哪些行銷活動使用「匿名」篩選器？ {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

在進行此變更之前，我們已將數個每週通知傳送至您的「通知」收件匣，其中包含使用「匿名」篩選器的智慧清單、智慧行銷活動和報告的清單。 這些功能可協助您識別目前使用此篩選器的位置。

請檢閱這些資訊，並識別在何處將「匿名」設為True，因為這些是受影響的行銷活動。 大多數情況下，客戶會將此設定用於某種評分。 請參閱上述範例，瞭解這些行銷活動現在將如何運作。

## 我想要更詳細的檔案。 我可以在哪裡找到它？ {#id-like-more-detailed-documentation-where-can-i-find-it}

檢視下列連結：

[匿名銷售機會升級概述](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[匿名銷售機會升級 — Marketo UI中的變更](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[匿名銷售機會升級 — 需要客戶動作](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[匿名銷售機會升級 — Analytics報告](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[匿名銷售機會升級 — 發行排程](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[匿名銷售機會升級 — 隱蔽](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[匿名潛在客戶促銷至已知潛在客戶 —  [!DNL Munchkin] V2行為](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## 我有更多問題！ 如何獲得解答？ {#i-have-more-questions-how-do-i-get-them-answered}

請聯絡 [社群](https://nation.marketo.com/){target="_blank"}. You can also contact [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}. 他們很樂意回答您的問題。
