---
unique-page-id: 2951877
description: 瞭解計畫機會分析區域 — Marketo檔案 — 產品檔案
title: 瞭解計畫機會分析領域
exl-id: 6105df93-b3de-4929-85e3-fd328372bd24
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# 瞭解計畫機會分析領域 {#understanding-the-program-opportunity-analysis-area}

## 概觀 {#overview}

計畫機會分析區域可讓您分析個別計畫的成效，或檢視計畫管道的摘要結果。

**您可以使用此分析區域回答的業務問題範例包括**：

一個特定計畫關聯了多少個機會，以及我們贏得了多少機會？

![](assets/one-1.png)

特定計畫或管道已協助產生多少收入？

![](assets/two-1.png)

對於指定的計畫或頻道，我的投資收入是多少？

![](assets/three-1.png)

特定計畫影響了哪些機會？

![](assets/four-1.png)

## 計畫機會分析歸因措施（藍點） {#program-opportunity-analysis-attribution-measures-blue-dots}

可用於分析的測量通常是數字，並以藍點表示。 Dimension是提供測量不同檢視的屬性，並以黃色點表示。

所有測量（藍點）都與歸因相關 — 潛在客戶贏取或與潛在客戶關聯的銷售成功的「評分」。

![](assets/six.five.png) ![](assets/seven-1.png)

有三種測量方式：

* 取得首次接觸歸因(FT)的贏取相關測量。
* 成功相關測量，可接收多重接觸歸因(MT)。
* 其他與方案相關的測量，包括建立或關閉「商機」之前的平均行銷接觸次數。

## 贏取和成功相關措施 {#acquisition-and-success-related-measures}

贏取相關措施會將評分給予方案，透過該方案首次取得潛在客戶的聯絡資訊。 潛在客戶不必在計畫中取得成功即可獲得贏取評分。

取得指定銷售機會的值會隨著時間而改變。 在潛在客戶進行購買之前，該值為零。 然後，它會隨著額外的購買而增加。

成功相關措施將功勞歸於所有有助於潛在客戶達成購買的計畫。

和收購一樣，對銷售線索的貢獻值會隨著時間而改變，並且在潛在客戶進行某些購買之前為零。

<table> 
 <tbody> 
  <tr> 
   <th>歸因測量 — 機會相關（FT或MT）*</th> 
   <th>說明</th> 
  </tr> 
  <tr> 
   <td>機會成本</td> 
   <td>影響機會的計畫成本部分。 如果涉及多個銷售機會，則成本可能會分割。</td> 
  </tr> 
  <tr> 
   <td>機會已建立</td> 
   <td>計畫因影響機會建立而收到的信用部分。 如果涉及多個銷售機會，則可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>成功的機會</td> 
   <td>計畫因影響贏得的機會而收到的信用部份。 如果涉及多個銷售機會，則可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>管道已建立</td> 
   <td>程式因影響機會建立而收到的信用部份（以貨幣價值表示）。 如果涉及多個銷售機會，則可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>管道已建立 — 仍開啟</td> 
   <td>程式收到影響目前開啟機會建立的信用部份（以貨幣價值表示）。 如果涉及多個銷售機會，則可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>預期收入</td> 
   <td>程式因影響機會建立而收到的信用部份（以貨幣價值表示）。 預期收入是機會機率乘以機會值。 如果涉及多個銷售機會，則可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>投資收入</td> 
   <td>這是程式收到的信用部份（以貨幣價值表示）的比率，用來影響贏得的機會與程式的成本。</td> 
  </tr> 
  <tr> 
   <td>已贏取收入</td> 
   <td>程式因影響贏得的機會而收到的信用部份（以貨幣價值表示）。 如果涉及多個銷售機會，則可能只是一小部分。</td> 
  </tr> 
 </tbody> 
</table>

_&#42;(FT) =首次接觸歸因，用於評估銷售機會贏取；(MT) =多重接觸歸因，用於評估銷售機會的成功_

以下案例說明當有兩個產生潛在客戶的計畫時，如何計算商機單位，但這些潛在客戶會從相同帳戶產生一個商機。

**方案1**

* 產生一個銷售機會：銷售機會1
* 潛在客戶1來自帳戶1

**方案2**

* 產生另一個銷售機會：銷售機會2
* 潛在客戶2也來自帳戶1

**帳戶1**

* 產生一個商機：商機1

Marketo會適當地提供學分，而不會跨計畫重複電腦會。 因此，在此情況下，每個計畫都會收到0.5個機會單位。 也就是說，每個計畫都會獲得所產生Opportunity一半的評分。 此外，與Opportunity相關聯的一半收入會指派給每個Program。

## 其他程式相關測量 {#miscellaneous-program-related-measures}

其他可用的衡量標准則反映方案的整體效能。

<table> 
 <tbody> 
  <tr> 
   <th>歸因測量 — 方案相關</th> 
   <th>說明</th> 
  </tr> 
  <tr> 
   <td>與計畫相關的商機數量</td> 
   <td><p>已將任何種類的歸因評分給予方案的機會總數。 機會可能受到一個或多個潛在客戶以及一個或多個計畫的影響。</p></td> 
  </tr> 
  <tr> 
   <td>每個已結束機會的平均成功數</td> 
   <td>商機關閉前平均方案成功次數。 <br></td> 
  </tr> 
  <tr> 
   <td>每個建立的機會平均成功數</td> 
   <td>建立Opportunity之前平均程式成功數量。</td> 
  </tr> 
  <tr> 
   <td>新名稱</td> 
   <td>計畫獲得的新名稱（即新銷售機會）總數。</td> 
  </tr> 
  <tr> 
   <td>計畫成本</td> 
   <td>計畫的總成本。</td> 
  </tr> 
  <tr> 
   <td>成功（總計）</td> 
   <td>取得成功的計畫成員總數。</td> 
  </tr> 
 </tbody> 
</table>

## 計畫機會分析Dimension（黃色圓點） {#program-opportunity-analysis-dimensions-yellow-dots}

雖然量值（藍點）會經過計算，且需要一些思考和說明才能使用，但維度（黃點）則是描述性的。 以下是可用的維度。

<table> 
 <tbody> 
  <tr> 
   <th>類別</th> 
   <th>顯示標籤</th> 
  </tr> 
  <tr> 
   <td>機會屬性</td> 
   <td>商機已關閉<br>機會名稱*<br>機會擁有者名稱<br>機會階段<br>機會型別</td> 
  </tr> 
  <tr> 
   <td>機會時間範圍</td> 
   <td>商機關閉年份/季度/月<br>建立的商機年/季/月</td> 
  </tr> 
  <tr> 
   <td>計畫屬性</td> 
   <td>計畫頻道<br>計畫名稱</td> 
  </tr> 
  <tr> 
   <td>計畫成本時間範圍</td> 
   <td>成本年/季/月</td> 
  </tr> 
 </tbody> 
</table>

*&#42;將任何型別的歸因評分給予方案的所有機會。 機會可能受到一個或多個潛在客戶以及一個或多個計畫的影響。*

>[!MORELIKETHIS]
>
>[建立Revenue Explorer報表](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
