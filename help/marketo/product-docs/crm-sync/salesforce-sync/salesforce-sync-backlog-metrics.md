---
description: Salesforce同步處理待處理量度 — Marketo檔案 — 產品檔案
title: Salesforce同步處理待處理專案量度
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: 1cc876285f8d7ac7a21a763dd65da34341341a0e
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Salesforce同步處理待處理專案量度  {#salesforce-sync-backlog-metrics}

同步待處理專案代表擱置從Salesforce同步至Marketo Engage的記錄，反之亦然。 若能確保待處理專案維持在可控範圍內，就能順利且及時地進行同步。

>[!NOTE]
>
>待處理專案涵蓋兩側擱置同步後更新的數字，而非同步流程步驟所執行的數字，例如[將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}或[將人員同步到Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"}流程步驟。

## 如何存取 {#how-to-access}

1. 在Marketo Engage中，移至&#x200B;**管理員**&#x200B;區域。

   熒幕擷圖

1. 選取&#x200B;**Salesforce**。

   熒幕擷圖

## 同步處理待處理專案趨勢 {#sync-backlog-trend}

待處理專案趨勢反映過去5天所記錄的待處理專案變更。 待處理專案會以4小時間隔顯示，分佈在5天內。 因此，圖表每天將顯示6個間隔乘以5天，這等於30個間隔。

在x軸上的特定4小時間隔觀察待處理專案。 此值適用於同步下的所有物件。 這是Salesforce和Marketo Engage等待同步處理的待處理專案總數。

熒幕擷圖

## 同步處理輸送量和待處理專案 {#sync-throughput-and-backlog}

統計資料反映過去24小時內同步處理下每種物件型別的輸送量和待處理狀態。 物件型別包含同步處理下的所有物件，包括：銷售機會、連絡人、帳戶、商機、促銷活動、使用者和自訂物件。 輸送量統計資料每15分鐘會自動重新整理一次，但您可以使用重新整理圖示手動重新整理。 每小時會擷取待處理專案。

>[!NOTE]
>
>統計資料會以滾動方式更新，而非以行事曆日期更新。

熒幕擷圖

<table><thead>
  <tr>
    <th>欄位</th>
    <th>說明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>同步的最大記錄數/小時</td>
    <td>物件型別在過去24小時內觀察到的每小時同步記錄數上限（最大輸送量）。 24小時期間會隨著時間滾動，而不是隨著行事曆日期滾動。</td>
  </tr>
  <tr>
    <td>同步的最小記錄數/小時</td>
    <td>物件型別在過去24小時內觀察到的每小時同步的最小記錄數（最小輸送量）。 24小時期間會隨著時間滾動，而不是隨著行事曆日期滾動。</td>
  </tr>
  <tr>
    <td>平均同步記錄數/小時</td>
    <td>物件型別在過去24小時內觀察到的每小時同步的平均記錄數（最小輸送量）。 24小時期間會隨著時間滾動，而不是隨著行事曆日期滾動。 這是以過去24小時內同步的記錄總數計算。</td>
  </tr>
  <tr>
    <td>同步處理待處理專案</td>
    <td>物件型別的擱置同步處理記錄待處理專案。 這是兩個方向(從Salesforce到Marketo Engage，反之亦然)擱置同步處理的待處理專案總數。 Salesforce的待處理專案是透過Salesforce的API呼叫取得，而Marketo Engage的待處理專案是透過從變更資料記錄檔取得的統計資料進行計算。 每小時計算一次。 此表格中的下兩個欄位會分別通知上次計算待處理專案的時間以及下一個計算的排程。</td>
  </tr>
  <tr>
    <td>預估待處理專案（時間）</td>
    <td>根據物件型別同步處理待處理專案所需的預估時間。 計算為「同步處理待處理專案/每小時同步處理的平均記錄」。</td>
  </tr>
  <tr>
    <td>上次擷取的待處理專案</td>
    <td>上次待處理專案計算的時間。</td>
  </tr>
  <tr>
    <td>待處理專案下一個擷取</td>
    <td>下一個待處理專案計算的時間。</td>
  </tr>
  <tr>
    <td>待處理專案狀態</td>
    <td>這會顯示未處理專案在過去6小時內是否有所增加。 如果目前的待處理專案大於6小時前記錄的待處理專案，則推斷為「成長」。 否則，會顯示為「正常」。 這是為了顯示同步處理輸送量是否趕上待處理專案。</td>
  </tr>
</tbody></table>

## 導致同步積壓的原因 {#what-causes-sync-backlogs}

無論是在Marketo Engage端或CRM端進行更新，都會觸發要重新同步的記錄，以透過對CRM同步循環的一般Marketo Engage更新另一端上的資訊。 每當在Salesforce上更新記錄時，它都會產生系統修改時間戳記，稱為「SysModStamp」。 此會將變更排入佇列以進行同步。

進行大量更新（例如變更欄位值）時，許多記錄會變更，導致新的SysModStamps。 然後，需要在Marketo Engage和您的CRM之間重新同步大量人員記錄更新，有時還會建立暫時性的待處理專案。

## 管理同步積壓的最佳作法 {#best-practices}

**同步處理下的欄位**：請確定同步處理下的欄位只是需要同步的欄位。 變更欄位會增加同步處理待處理專案，而低優先順序欄位可能會停止或減慢同步處理中較重要的欄位。 請聯絡[Marketo Engage支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}以移除同步處理下的欄位。

**敏感欄位**：某些欄位容易頻繁更新（例如，貨幣會變更的貨幣欄位）。 檢閱這些欄位是否需要同步，或欄位是否需要以不同方式設計。

**自訂物件**：定期檢閱同步處理的自訂物件，並移除任何不再需要同步處理的物件。

**活動**：檢查同步處理下是否有任何活動可以從同步處理移除。

**在非關鍵期間排程大量更新**：檢閱您的資料同步模式，以識別非關鍵期間。 檢視是否可以在這些非關鍵期間排程大量更新。

如果您遵循上述所有最佳實務，但仍有大量積壓，請聯絡[Marketo Engage支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。
