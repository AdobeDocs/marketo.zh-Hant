---
unique-page-id: 2951877
description: 瞭解計畫機會分析領域——行銷文檔——產品文檔
title: 瞭解計畫機會分析領域
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---


# 瞭解計畫機會分析領域{#understanding-the-program-opportunity-analysis-area}

## 概述{#overview}

Program Opportunity Analysis區域允許您分析單個Programs的有效性，或查看按Program Channel列出的總結結果。

**使用此分析區域可回答的業務問題示例包括**:

有多少機會與特定計畫相關，以及我們贏得了多少機會？

![](assets/one-1.png)

特定方案或渠道可帶來多少收入？

![](assets/two-1.png)

特定方案或渠道的「投資收益」是多少？

![](assets/three-1.png)

特定方案對哪些機會有影響？

![](assets/four-1.png)

## 計畫機會分析歸因度量（藍點）{#program-opportunity-analysis-attribution-measures-blue-dots}

可用於分析的度量通常是數字，用藍點表示。 尺寸是提供測量不同視圖的屬性，由黃點表示。

所有度量（藍點）都與歸因有關——銷售機會獲取或銷售成功與銷售機會相關的「評分」。

![](assets/six.five.png) ![](assets/seven-1.png)

有三種措施：

* 與贏取相關的測量，獲得首次接觸歸因(FT)。
* 成功相關措施，可接收多點觸控歸因(MT)。
* 其他與Program相關的度量，包括在建立或關閉Opportunity之前的平均行銷接觸數。

## 贏取與成功相關度量{#acquisition-and-success-related-measures}

與收購相關的措施可讓潛在客戶的聯絡資訊首次獲得的方案獲得肯定。 銷售機會不必在要授予的贏取評價方案中取得成功。

獲取給定銷售線索的值隨時間而改變。 直到銷售機會完成購買，這個數字才會為零。 隨後，隨著額外購買量增加。

成功相關措施可表揚促成潛在客戶購買進度的所有方案。

與贏取一樣，銷售機會的貢獻值會隨著時間而改變，直到銷售機會進行某些購買為止為零。

<table> 
 <tbody> 
  <tr> 
   <th>歸因度量——機會相關（FT或MT）*</th> 
   <th>說明</th> 
  </tr> 
  <tr> 
   <td>機會成本</td> 
   <td>影響機會的計畫成本部分。 如果涉及多個銷售線索，成本可能會被分攤。</td> 
  </tr> 
  <tr> 
   <td>建立的機會</td> 
   <td>方案為影響創造機會而獲得的信用部分。 如果涉及多個線索，這可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>贏得機會</td> 
   <td>計畫因影響贏得的機會而獲得的積分部分。 如果涉及多個線索，這可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>已建立管線</td> 
   <td>該方案為影響機會創造而收到的信用部分（以貨幣價值計）。 如果涉及多個線索，這可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>已建立管線——仍然開啟</td> 
   <td>該方案為影響創造當前開放機會而收到的信用部分（以貨幣價值計）。 如果涉及多個線索，這可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>預期收入</td> 
   <td>該方案為影響機會創造而收到的信用部分（以貨幣價值計）。 預期收入是機會概率乘以機會值。 如果涉及多個線索，這可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>收入對投資</td> 
   <td>這是程式為影響成功機會而收到的信用部分（以貨幣價值計）與程式成本之比。</td> 
  </tr> 
  <tr> 
   <td>贏取收入</td> 
   <td>該計畫為影響贏得的機會而收到的信用部分（以貨幣價值計）。 如果涉及多個線索，這可能只是一小部分。</td> 
  </tr> 
 </tbody> 
</table>

_*(FT)=首次接觸歸因，用於鉛獲取量度；(MT)=多點觸控歸因，用於銷售機會成功的度量_

以下是一種方案，說明當有兩個程式產生銷售機會，但這些銷售機會導致同一帳戶中出現一個銷售機會時，如何計算Opportunity Units。

**方案1**

* 生成一個銷售線索：Lead 1
* 銷售線索1來自帳戶1

**方案2**

* 生成另一個銷售線索：Lead 2
* 銷售線索2也來自帳戶1

**帳戶1**

* 生成一個Opportunity :機會1

Marketo在不重複計算各方案的機會的情況下，適當地提供信用。 因此，在此例中，每個方案收到0.5個機會單位。 也就是說，每個Program都會獲得生成的Opportunity的一半評價。 此外，與Opportunity相關的一半收入分配給每個Program。

## 與其他方案有關的措施{#miscellaneous-program-related-measures}

其他可用措施反映了方案的總體業績。

<table> 
 <tbody> 
  <tr> 
   <th>歸因度量——方案相關</th> 
   <th>說明</th> 
  </tr> 
  <tr> 
   <td>與計畫相關的機會數</td> 
   <td><p>給予方案任何歸因評價的總Opportunities數。 機會可能受到一個或多個銷售機會以及一個或多個計畫的影響。</p></td> 
  </tr> 
  <tr> 
   <td>每個已關閉機會的平均成功數</td> 
   <td>在Opportunity關閉之前， Program成功的平均數。 <br></td> 
  </tr> 
  <tr> 
   <td>每次建立的機會平均成功數</td> 
   <td>在建立Opportunity之前， Programs成功的平均數。</td> 
  </tr> 
  <tr> 
   <td>新名稱</td> 
   <td>由方案獲得的新名稱，即新銷售線索的總數。</td> 
  </tr> 
  <tr> 
   <td>方案成本</td> 
   <td>方案總費用。</td> 
  </tr> 
  <tr> 
   <td>成功（總計）</td> 
   <td>獲得成功的方案成員總數。</td> 
  </tr> 
 </tbody> 
</table>

## 計畫機會分析維（黃點）{#program-opportunity-analysis-dimensions-yellow-dots}

測量（藍點）是計算的，需要一些思考和說明才能使用，而尺寸（黃點）則是描述性的。 以下是可用維度。

<table> 
 <tbody> 
  <tr> 
   <th>類別</th> 
   <th>顯示標籤</th> 
  </tr> 
  <tr> 
   <td>機會屬性</td> 
   <td>Opportunity Closed<br> Opportunity Name*<br> Opportunity Owner Name<br> Opportunity Stage<br> Opportunity Type</td> 
  </tr> 
  <tr> 
   <td>機會時間範圍</td> 
   <td>業務機會關閉年／季/月<br>業務機會建立年／季/月</td> 
  </tr> 
  <tr> 
   <td>方案屬性</td> 
   <td>節目頻道<br>節目名稱</td> 
  </tr> 
  <tr> 
   <td>計畫成本時間範圍</td> 
   <td>成本年／季/月</td> 
  </tr> 
 </tbody> 
</table>

**提供任何類型歸因給方案的所有Opportunities。機會可能受到一個或多個銷售機會以及一個或多個方案的影響。*

>[!MORELIKETHIS]
>
>[建立收入總管報表](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
