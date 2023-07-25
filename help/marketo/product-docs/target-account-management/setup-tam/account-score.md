---
unique-page-id: 11380774
description: 帳戶分數 — Marketo檔案 — 產品檔案
title: 帳戶分數
exl-id: 68fb5f41-f715-4a4d-b4da-9db4dc38d67d
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 帳戶分數 {#account-score}

帳戶評分是Target帳戶管理的重要部分。 它可協助您判斷帳戶的參與層級。

## 什麼是帳戶評分？ {#what-is-account-scoring}

這是一種系統化方法，旨在協助銷售及行銷團隊識別最有可能購買的公司（包括潛在客戶）並排定其優先順序。

在B2B購買程式的複雜世界中，很少會有一個人做出購買決定。 其中通常包含各種角色，每個角色都有其專屬的需求。 根據帳戶的評分會透過彙總來自多個潛在客戶的潛在客戶評分並在帳戶層級提供評分來將此考慮在內。

## 常見範例 {#common-examples}

<table> 
 <tbody>
  <tr>
   <td><strong>帳戶參與分數</strong></td> 
   <td>參與度深度是根據特定目標帳戶中，不同管道（例如電子郵件、網頁和廣告）所追蹤的行為活動而定。</td>
  </tr>
  <tr>
   <td><strong>帳戶產品興趣分數</strong></td>
   <td>目標帳戶中的人員對特定產品的內容表現出興趣（例如下載白皮書）。</td> 
  </tr>
  <tr>
   <td><strong>帳戶網站參與度分數</strong></td>
   <td>來自目標帳戶的使用者造訪Web Channel。 可以建立相同的分數來測量電子郵件、廣告或其他管道的管道參與度。</td> 
  </tr>
 </tbody>
</table>

## 如何設定帳戶分數 {#how-to-configure-account-score}

>[!NOTE]
>
>若要計算帳戶分數，您必須先建立潛在客戶分數。 Marketo TAM會自動將潛在客戶分數彙總至帳戶分數。 以上面兩個範例為例(_帳戶產品興趣分數_ 和 _帳戶網站參與度分數_)。
>
>首先，建立銷售機會分數欄位，從目標帳戶的每個銷售機會擷取相關詳細資訊。\
>然後，將這些潛在客戶分數指派給其個別帳戶分數：\
>帳戶產品利息分數= SUM （潛在客戶產品利息分數）\
>帳戶網路參與分數= SUM （潛在客戶網路參與分數）

>[!NOTE]
>
>使用者可以建立多個帳戶參與分數，並將不同的個人分數指派給不同的帳戶分數。

設定好銷售機會分數後，請依照下列步驟繼續。

1. 按一下 **管理員**.

   ![](assets/one-1.png)

1. 按一下 **目標帳戶管理**.

   ![](assets/account-score-2.png)

1. 在評分欄位中，按一下 **編輯**.

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >您最多可以選擇 **五** 用於計算帳戶分數的欄位。

1. 輸入「帳戶分數」名稱，按一下 **選取個人分數** 下拉式清單，並選取對應的分數。

   ![](assets/four.png)

1. 按一下 **+新增** 以新增更多分數。

   ![](assets/five.png)

1. 新增所有想要的分數。 按一下 **儲存** 完成時。

   ![](assets/six.png)
