---
unique-page-id: 6848705
description: 最佳實務 — 如何組織您的程式 — Marketo檔案 — 產品檔案
title: 最佳實務 — 如何組織您的計畫
exl-id: 018a3fbd-b741-4005-9695-56958063d71a
feature: Programs
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# 最佳做法：如何組織您的計畫 {#best-practice-how-to-organize-your-programs}

有許多方式可在行銷活動中組織樹狀結構以及單一方案的內容。 不過，有些方式會更好，而且可協助行銷部門的人員。

>[!TIP]
>
>總有一天（晉升後！），其他人會嘗試幫您瞭解計畫。 良好的組織能協助他們迅速提高生產力。

## 資料夾 {#folders}

在行銷活動中，您應該使用資料夾來組織您的方案。 我們建議的結構如以下範例所示：

>[!NOTE]
>
>**範例**
>
>* 有效的行銷方案
>   * 電子郵件
>   * 事件
>      * 直播活動/路演
>      * 商展
>      * 網路研討會
>   * 電子報
>   * 培養
>   * 網頁內容
>   * 網路表單
>* 學習
>* 營運
>   * 生命週期
>   * 評分
>   * 資料管理
>* 銷售分析
>   * 有趣的時刻
>   * 銷售電子郵件
>   * 銷售請求的行銷活動
>* **封存**
>   * 封存事件
>      * 2012年封存
>      * 2013年封存

範例中提到的每個檔案夾都是資料夾。 請注意它們是如何全都唯一命名的。 您可以有重複（較簡單的）資料夾名稱INSIDE程式，但不能在樹狀結構的根目錄。

>[!TIP]
>
>「封存」資料夾是一種特殊型別的資料夾，旨在從選取的清單以及報告中移除專案。 這有助於您的系統更快速地執行。 深入瞭解[資料夾](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md){target="_blank"}。

您當然可以視需要新增更多資料夾。 請記住，公司中未來幾代行銷人員將會接受您命名或組織事情的決定。

## 命名配置 {#naming-schemes}

命名非常重要，因為Marketo的功能都使用共同語言來溝通。 對於計畫，您應該為它們命名一些不重複的名稱。 **沒有兩個程式可以有相同的名稱**。 最佳實務建議使用以下格式：

[程式型別]的縮寫[YYYY]-[MM]-[選擇性DD] [簡短描述]

>[!NOTE]
>
>**範例**
>
>範常式式名稱：
>
>1. ES 2015-09-21 Widget簡介
>1. NL 2015-06電子報
>1. WBN 2015-12-01網路研討會主題，請前往

程式名稱在您的訂閱中必須是唯一的，即使是在不同的[工作區](/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md){target="_blank"}中。  對於程式內的本機資產，規則是&#x200B;**保持名稱簡單**。 只需將邀請命名為「邀請」，而非「2015年6月網路研討會邀請」。 因為這些是在程式中，當從其他位置選擇父程式時，父程式會自動成為名稱的一部分。 換言之，本機資產在程式內只需是唯一的。 您可以有數百個名為「邀請」的資產，每個資產位於不同的程式中，這樣就不會麻煩你了。

## Token {#tokens}

Token會將資料夾和程式當作工具，用來設定供登陸頁面、電子郵件和其他資產使用的變數。

上述組織可讓您將代號放入「事件」資料夾，使其向下套用至所有事件。

>[!NOTE]
>
>**範例**
>
>**您的公司地址**。 使用Token，而非每次都寫入。 如此一來，您就可以在一個位置更新它，而無需建立許多草稿。 然後視需要在較低層級的資料夾中覆寫權杖。

## 事件 {#events}

事件通常有很多移動部分，包括：邀請、登陸頁面、表單、社交Widget和智慧型行銷活動。 組織這些區段以方便使用的最佳實務是依事件的階段進行。 以下是資料夾樹狀結構尋找事件的方式範例。

![](assets/capture.png)

## 參與計畫 {#engagement-programs}

瞭解[參與計畫的所有資訊](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/understanding-engagement-programs.md){target="_blank"}。 組織參與計畫的最佳方式是使用資料夾。 為每個資料流建立一個資料夾，然後將電子郵件或程式放入該資料夾中。 內容過時且您想要移除時，請在每個資料流中加入封存資料夾。

## 操作程式 {#operational-programs}

這些用於資料清理目的。 擁有程式執行日期的資料夾，然後封存資料夾。 讓程式可運作，您就會在報表中省略它，而這對這類活動有利。

## 巢狀電子郵件程式 {#nesting-email-programs}

「電子郵件程式」的設計目的是要成為您用來爆送郵件的工具。 您可以將它們放在活動或其他促銷活動、邀請和提醒的方案中。 附有酷炫的控制面板和其他A/B測試功能。 此外，它們可在方案排程檢視中輕鬆操控。

您也可以製作電子郵件程式，作為獨立程式。 電子郵件程式不允許在其他電子郵件程式中使用。 那太瘋狂了！

## 正在原地複製 {#cloning}

Marketo最酷的功能之一是復製程式。 這表示您可以設定方案「範本」，其中包含所有您想要的智慧行銷活動和電子郵件。 預先設定，然後為您下一個行銷方案複製。

>[!TIP]
>
>請注意頂端範例中的事件範本。 您可以將不同型別的事件放在那裡，以方便複製。

有些人甚至會將電子郵件和登入頁面中的大部分文字抽象為權杖。 這可讓您原地複製並編輯權杖。 最後，前往方案排程檢視並調整日期，您即已完成。 瞧！

## 摘要 {#summary}

如您所見，Marketo可提供強大的功能。 我們在此介紹基本知識，但請考慮來自[Marketo Engage專家](https://business.adobe.com/products/marketo/services-support.html){target="_blank"}的其他服務，以微調並設定您自己的成功計畫。
