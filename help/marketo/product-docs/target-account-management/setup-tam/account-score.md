---
unique-page-id: 11380774
description: 帳戶分數 — Marketo檔案 — 產品檔案
title: 帳戶分數
exl-id: 68fb5f41-f715-4a4d-b4da-9db4dc38d67d
feature: Target Account Management
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# [!UICONTROL Account Score] {#account-score}

帳戶評分是[!UICONTROL Target Account Management]的重要部分。 它可協助您判斷帳戶的參與層級。

## 什麼是帳戶評分？ {#what-is-account-scoring}

這是一種系統性的方法，旨在協助銷售與行銷團隊識別最有可能購買的公司（包括潛在客戶），並排定其優先順序。

在B2B購買程式的複雜世界中，很少會有一個人做出購買決定。 通常有各種角色參與，每個角色都有其自己的需求。 帳戶型評分會透過彙總來自多個潛在客戶的潛在客戶評分並在帳戶層級提供評分來將此考慮在內。

## 常見範例 {#common-examples}

<table>
 <tbody>
  <tr>
   <td><strong>帳戶參與分數</strong></td>
   <td>參與深度是根據特定目標帳戶中人員的各種管道（例如電子郵件、網頁和廣告）所追蹤的行為活動而定。</td>
  </tr>
  <tr>
   <td><strong>帳戶產品興趣分數</strong></td>
   <td>目標帳戶中的人員對特定產品的內容（例如下載白皮書）表現出興趣。</td>
  </tr>
  <tr>
   <td><strong>帳戶網頁參與分數</strong></td>
   <td>目標帳戶中造訪Web Channel的人員。 可以建立相同的分數來測量電子郵件、廣告或其他頻道的頻道參與度。</td>
  </tr>
 </tbody>
</table>

## 如何設定帳戶分數 {#how-to-configure-account-score}

>[!NOTE]
>
>若要計算帳戶分數，您必須先建立潛在客戶分數。 Marketo TAM會自動將潛在客戶分數彙總至帳戶分數。 舉例來說，我們舉兩個上述範例（_帳戶產品興趣分數_&#x200B;和&#x200B;_帳戶網頁參與分數_）。
>
>首先，建立銷售機會分數欄位，從目標帳戶的每個銷售機會擷取相關詳細資訊。
>&#x200B;>然後，將這些潛在客戶分數指派給其個別帳戶分數：
>&#x200B;>帳戶產品利息分數= SUM （潛在客戶產品利息分數）
>&#x200B;>帳戶網站參與分數= SUM （潛在客戶網站參與分數）

>[!NOTE]
>
>使用者可以建立多個帳戶參與分數，並將不同的人員分數指派給不同的帳戶分數。

設定好銷售機會分數後，請依照下列步驟繼續進行。

1. 按一下「**[!UICONTROL Admin]**」。

   ![](assets/account-score-1.png)

1. 按一下「**[!UICONTROL Target Account Management]**」。

   ![](assets/account-score-2.png)

1. 在[!UICONTROL Scoring Fields]中，按一下&#x200B;**[!UICONTROL Edit]**。

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >您最多可以選擇&#x200B;**5個**&#x200B;欄位來計算[!UICONTROL Account Score]。

1. 輸入[!UICONTROL Account Score]名稱，按一下&#x200B;**[!UICONTROL Select Person Score]**&#x200B;下拉式清單並選取對應的分數。

   ![](assets/account-score-4.png)

1. 按一下&#x200B;**[!UICONTROL +Add]**&#x200B;以新增更多分數。

   ![](assets/account-score-5.png)

1. 新增所有想要的分數。 完成時，按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/account-score-6.png)
