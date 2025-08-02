---
description: Salesforce同步處理待處理量度 — Marketo檔案 — 產品檔案
title: Salesforce同步處理待處理專案量度
feature: Reporting
exl-id: 6b58eb50-ff0d-4774-a232-3ae929948e2a
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# Salesforce同步處理待處理專案量度  {#salesforce-sync-backlog-metrics}

同步處理待處理專案是用於擱置同步處理之記錄的名稱。 它會將擱置從Salesforce同步至Marketo Engage的記錄計算在內，反之亦然。 確保待處理專案維持在可控範圍內，可順利進行時間同步。 待處理專案涵蓋兩側擱置同步發佈更新的數量，而非同步流程步驟(例如Sync Lead to SFDC流程步驟)所執行的數量。

## 如何存取 {#how-to-access}

1. 在Marketo Engage中，移至&#x200B;**管理員**&#x200B;區域。

   ![](assets/salesforce-sync-backlog-metrics-1.png)

1. 選取&#x200B;**Salesforce**。

   ![](assets/salesforce-sync-backlog-metrics-2.png)

## 同步處理待處理專案趨勢 {#sync-backlog-trend}

待處理專案趨勢反映過去5天所記錄的待處理專案變更。 待處理專案會以4小時間隔顯示，分佈在5天內。 因此，圖表每天將顯示6個間隔乘以5天，這等於30個間隔。

在x軸上的特定4小時間隔觀察待處理專案。 此值適用於同步下的所有物件。 這是Salesforce和Marketo Engage中等待同步處理的待處理專案總數。

![](assets/salesforce-sync-backlog-metrics-3.png)

## 同步處理輸送量和待處理專案 {#sync-throughput-and-backlog}

統計資料反映過去24小時內同步處理下每種物件型別的輸送量和待處理狀態。 物件型別包含同步處理下的所有物件，包括：銷售機會、連絡人、帳戶、商機、促銷活動、使用者和自訂物件。 輸送量統計資料每15分鐘會自動重新整理一次，但您可以使用重新整理圖示手動重新整理。 每小時會擷取待處理專案。

>[!NOTE]
>
>統計資料會以滾動方式更新，而非以行事曆日期更新。

![](assets/salesforce-sync-backlog-metrics-4.png)

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
    <td>物件型別的擱置同步處理記錄待處理專案。 這是兩個方向(從Salesforce到Marketo Engage，反之亦然)的待處理同步總數。 Salesforce的待處理專案是透過Salesforce的API呼叫取得，而Marketo Engage的待處理專案是透過從變更資料記錄檔取得的統計資料進行計算。 每小時計算一次。 此表格中的下兩個欄位會分別通知上次計算待處理專案的時間以及下一個計算的排程。</td>
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

無論更新是在Marketo Engage端或CRM端進行，都會觸發要重新同步的記錄，以透過一般Marketo Engage到CRM同步週期更新另一端上的資訊。 每當在Salesforce上更新記錄時，它都會產生系統修改時間戳記，稱為「SysModStamp」。 此會將變更排入佇列以進行同步。

進行大量更新（例如變更欄位值）時，許多記錄會變更，導致新的SysModStamps。 之後，需要在Marketo Engage與您的CRM之間重新同步大量人員記錄更新，有時會產生暫時性的待處理專案。

## 管理同步積壓的最佳作法 {#best-practices}

**同步處理使用者可見的欄位**：請確定同步處理使用者可見的欄位只是需要同步處理的欄位，且對行銷工作有價值。 如果更新Salesforce中的記錄以更新上次修改的時間戳記，會將記錄排入同步待處理專案的佇列，且不必要的欄位同步可能會減慢同步下更重要的欄位的速度。 如果同步使用者看不到不必要的欄位，則更新這些欄位將會導致略過，其速度會比更新快得多。 與您的Salesforce管理員合作檢閱[這裡](https://nation.marketo.com/t5/marketo-whisperer-blogs/best-practices-for-determining-which-fields-to-sync-with-marketo/ba-p/247449){target="_blank"}的最佳實務，並更新Marketo同步使用者可看到的欄位。

**隱藏或篩選不必要的記錄**：如果記錄無法銷售，則可能是浪費同步資源。 如果同步使用者看不到，則不會浪費資源嘗試同步處理。 [Marketo Engage支援](https://nation.marketo.com/t5/support/ct-p/Support#_blank){target="_blank"}可協助設定同步篩選器，以根據其他條件禁止記錄同步。 如需設定自訂同步篩選器[的詳細資訊，請參閱此處](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"}。 強烈建議在Salesforce中使用索引欄位（如需進一步資訊，請聯絡Salesforce）。

**在非關鍵期間排程大量更新**：檢閱您的資料同步模式，以識別非關鍵期間。 如果可能的話，請檢閱是否可以在這些非關鍵期間排程大量更新。

**經常更新的欄位**：有些欄位很容易經常更新。 例如，貨幣欄位可能會發生貨幣變更。 檢閱這些欄位是否需要同步，或欄位是否應以不同方式設計。 如果您有其他經常更新且不需要的欄位，請向同步使用者隱藏它們。 請務必與您的SFDC管理員整合討論可能會更新欄位的問題。

**自訂物件**：定期檢閱[啟用同步的自訂物件](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync){target="_blank"}，並停用不再需要同步的自訂物件。

**活動**： [檢閱是否有任何活動](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync){target="_blank"}已啟用從同步中移除的同步。  每個潛在客戶每天只能同步處理一次這些活動。

**檢閱同步處理錯誤**：例外狀況處理可能會減慢同步處理的速度。 檢閱使用者通知並解決錯誤可以改善同步處理健康情況。

**連絡支援人員**：如果您遵循上述所有最佳實務，但仍有大量積壓，請連絡[Marketo Engage支援人員](https://nation.marketo.com/t5/support/ct-p/Support#_blank){target="_blank"}。
