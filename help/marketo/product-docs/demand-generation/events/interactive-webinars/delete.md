---
description: 推廣互動式網路研討會 — Marketo檔案 — 產品檔案
title: 推廣互動式網路研討會
feature: Interactive Webinars
exl-id: d26f91ce-3a95-4247-9a52-085260bb15e8
source-git-commit: 75035e6ae7989aaf3ed6cedd7fdab42c79ab8f37
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# 推廣互動式網路研討會 {#promoting-an-interactive-webinar}

宣傳互動式網路研討會與透過Launchpoint宣傳合作夥伴網路研討會類似。 建立互動式網路研討會事件程式時，您可以執行行銷活動或將成員匯入程式來新增成員。 若要檢查已新增至互動式網路研討會活動程式的成員，請按一下&#x200B;**成員**&#x200B;標籤。

![](assets/promoting-an-interactive-webinar-1.png)

新增或匯入成員後，您可以在互動式網路研討會活動方案內建立電子郵件促銷活動，以傳送邀請給所有方案成員，並在傳送電子郵件後將其狀態變更為「已邀請」。

>[!NOTE]
>
>如果您想要將共同主持人或簡報者新增為互動式網路研討會活動計畫的對象成員，您必須為他們使用不同的電子郵件ID，否則他們會收到「此電子郵件已註冊」錯誤。

電子郵件可以包含方案的特定詳細資料，並包含登陸頁面URL，後者會將收件者重新導向至特定頁面，以新增更多關於網路研討會的資訊（例如內容、簡報者資訊等）。 此登陸頁面可在互動式網路研討會活動程式中建立為本機資產。

您可以在登入頁面上啟用表單，並將表單點按連結至互動式網路研討會事件程式中已啟用的註冊，以請求註冊此網路研討會。 接著可以建立行銷活動，使用表單提交作為觸發器，並將方案狀態從「已邀請」變更為「已註冊」。

>[!NOTE]
>
>在互動式網路研討會中，從「已邀請」到「已註冊」的轉變不會是自動的，因為可能有多個觸發器會建立轉變。

一旦成員在互動式網路研討會活動計畫中處於「已註冊」計畫狀態，系統就會自動向Adobe Connect中建立的網路研討會進行註冊。 然後會將名字、姓氏和電子郵件ID等註冊資料傳輸至Adobe Connect。 這表示一旦使用者以參與者身份加入網路研討會，簡報者或主持人在網路研討會期間就可以使用這些資訊。

在註冊後的幾分鐘內，成員的「網路研討會URL」就會填入到「成員」標籤中。 如果您找不到網路研討會URL的欄，請確定該欄已新增至您的檢視。 這是每個註冊會員的個人化URL，可讓您在排程時間參加網路研討會，而不需要任何驗證。 內部交換的權杖會處理成員的驗證。

您可以使用`{{member.webinar url}}` [權杖](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}將網路研討會URL加入電子郵件促銷活動中的個別成員，以傳達他們已在事件中註冊，並使用加入URL在排程時間進入網路研討會。 行事曆權杖可用於相同的電子郵件行銷活動，以確保網路研討會排程可新增到成員的行事曆。

連結可在您的Event Program中的「概觀」標籤右側取得，以建立登入頁面以及電子郵件促銷活動。 與活動相關的其餘促銷活動，與使用Launchpoint整合的合作夥伴網路研討會相同。

![](assets/promoting-an-interactive-webinar-2.png)

互動式網路研討會可讓您在網路研討會之前、期間或之後索取報名。 在所有情況下，您只需要與潛在客戶共用網路研討會URL即可。 在網路研討會開始前按一下連結，即會將連結傳送至網路研討會前登陸頁面。 在網路研討會期間按一下，系統就會將他們導向進行中的網路研討會。 在網路研討會後按一下，系統會將他們導向至網路研討會的錄影。

## 互動式網路研討會Token {#interactive-webinars-tokens}

使用權杖，在電子郵件和登陸頁面中推廣互動式網路研討會，無需手動新增網路研討會詳細資訊。 這麼做可改善整體效率，因為對網路研討會中繼資料所做的任何變更（例如網路研討會標題、開始日期等）都會自動反映在您的資產中。

![](assets/promoting-an-interactive-webinar-3.png)

**權杖清單**

* program.webinarCapacity
* program.webinarDuration
* program.webinarEndDate
* program.webinarEndTime
* program.webinarGenericURL
* program.webinarLanguage
* program.webinarStartDate
* program.webinarStartTime
* program.webinarTimezone
* program.webinarTitle
