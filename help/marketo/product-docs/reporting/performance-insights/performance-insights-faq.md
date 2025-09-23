---
unique-page-id: 12979858
description: 效能深入分析常見問題集 — Marketo檔案 — 產品檔案
title: 績效洞察常見問題
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 0%

---

# [!UICONTROL Performance Insights]常見問題集 {#performance-insights-faq}

## [!UICONTROL Engagement]索引標籤中「success」的定義是什麼？ {#what-is-the-definition-of-success-in-the-engagement-tab}

在Marketo中，成功是衡量有意義的互動。 方案的目的是建立與人員或潛在客戶的有意義的互動。 當個人達到達到達到該目標的狀態時會標籤成功。 可能是參加網路研討會、按一下電子郵件中的連結，或填寫網路表單。 成功與否因方案管道而異。

>[!NOTE]
>
>網路研討會計畫中有多種狀態，例如：已邀請、已註冊和已參加。 「已邀請」或「已註冊」互動沒有意義，因為使用者不會實際觀看網路研討會。 在此情況下，出席被視為成功。

## MPI是否可與任何CRM搭配使用？ {#will-mpi-work-with-any-crm}

可以。就技術方面而言，MPI不會直接與CRM互動以進行資料同步。 MPI會利用儲存在Marketo Analytics Data Warehouse中的資料。 由於CRM同步作業會在銷售機會管理應用程式中進行，因此Marketo支援的與銷售機會管理應用程式整合的任何CRM都會正確顯示資料。 不過，CRM機會欄位確實需要正確對應到Marketo機會欄位。

## 我沒有其他任何Marketing Analytics產品(ARB、RCE、RCA、Program Analysis)。 MPI是否適合我？ {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI是Lead Management應用程式的獨立附加元件。 它不需要使用任何其他分析產品。

## RCA也會顯示程式效能資料。 MPI和RCA中顯示的資料之間是否有差異？ {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

不可以。 MPI會從與RCA相同的資料倉儲取得資料。 因此，您將不會看到兩者之間的任何資料差異。 RCA可讓您即時建立自己的報表。 MPI可讓您存取容易理解的視覺儀表板。

## 我不希望我的某些程式（例如作業）顯示在MPI中。 我該如何控制特定程式的可見度？ {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

您可以將程式的Analytics行為設定為「作業」，藉此控制程式的可見度。 這將導致該程式被排除在分析計算之外。

>[!NOTE]
>
>在[此處](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md)進一步瞭解設定分析行為。

## 我正在為新產品上市執行多頻道行銷活動。 如何在一個位置檢視跨所有不同管道的此行銷活動績效？ {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

我們建議您在行銷活動中的方案使用方案標籤。 方案標籤會自動同步至MPI，您可以在所有MPI儀表板中篩選它們，以檢視您的多頻道行銷活動績效。

## 如果沒有RCA，我是否可存取歸因設定？ {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

如果您有MPI，則無論您是否有RCA，都可以存取歸因設定。

## 當我登入時在MPI中收到警報，告知我歸因設定不正確。 有什麼問題嗎？ {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI會計算您的所有機會是否都包含在Analytics中。 如果沒有，系統會提示您考慮變更歸因設定（明確、隱含、混合）以包含更多機會。

您也可能因為方案中缺少方案成本而缺少機會。 請檢閱程式的Analytics行為。 它們可以是：

1. 預設 — 預設行為是只有在至少一個期間成本（即使指派零美元）時，程式才會包含在MPI中。

1. 包含 — 此選項將確保MPI中可以使用程式，無論您是否包含期間成本。

1. [作業中](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs) — 此選項導致程式無法在MPI中顯示。

>[!NOTE]
>
>期間成本&#x200B;**已設定**&#x200B;以在參與儀表板中報告成功和新名稱。 此儀表板利用期間成本資料來彙總成功和新名稱。 如果未設定「期間成本」，則無論上述Analytics行為設定為何，參與控制面板都不會正確報告。

## 為什麼我在MPI中錯過了一些機會？ {#why-am-i-missing-some-opportunities-in-mpi}

您可能在MPI中錯過商機的兩個主要原因為：

1. 歸因設定設為「明確」，但機會未指派聯絡人角色
1. 期間成本不包含在您的方案中

MPI會計算您的所有機會是否都包含在Analytics中。 如果沒有，系統會提示您考慮變更歸因設定（明確、隱含、混合）以包含更多機會。

您也可能因為方案中缺少方案成本而缺少機會。 警報會出現，但不會指出哪些程式缺少成本。 請檢閱您的方案設定以包含成本，以確保您的所有方案和機會都包含在MPI中。

## 為什麼在參與儀表板上看不到自訂欄位、機會型別和ABM篩選器？ {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

自訂欄位、機會型別和ABM篩選器都是與機會相關的屬性。 「業務開發」儀表板可讓您測量您的業務開發，以及潛在客戶贏取，無論他們是否與商機相關聯。 由於Engagement儀表板未考慮機會，因此自訂欄位、機會型別和ABM篩選器不適用。

## 我想要使用自訂Salesforce機會欄位來報告收入，而不是使用標準Salesforce機會金額欄位。 MPI允許我這麼做嗎？ {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

可以。只要欄位型別為貨幣，[Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support)就能將Marketo的「機會金額」欄位重新對應到自訂Salesforce「機會」欄位。 由於MPI指向Marketo機會數量欄位，因此MPI可以使用重新對應的自訂Salesforce欄位中的資料。

>[!NOTE]
>
>重新對應後，MPI會顯示後續的資料。 不會變更歷史數量。

## 如果不使用機會，還可以使用MPI嗎？ {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI的設計可讓您從漏斗的頂部開始測量計畫效能，直到收入影響。 如果您沒有使用機會，您仍然能夠：

* 檢視您的Nurture方案效能，以吸引受眾參與。
* 檢視潛在客戶贏取計畫的績效。
* 透過方案標籤檢視多管道行銷活動的績效。
* 檢視過去12個月的對象參與趨勢。
* 在PowerPoint中儲存並匯出效能資料。

## 我可以測量MPI中帳戶型策略的成功程度嗎？ {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

可以。MPI與[Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview)整合，可順暢地將ABM帳戶清單提取至MPI。 您可以使用「ABM帳戶清單」篩選器來選擇所需的ABM清單以篩選資料。

## 購買MPI時，是否可以立即使用歸因？ {#is-attribution-instantly-available-when-i-purchase-mpi}

客戶購買MPI時，可使用Marketo歸因功能。 不過，需要[適當的設定](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md)，才能確保機會和程式資料正確流入MPI。

## 我該怎麼做才能設定歸因？ {#what-do-i-have-to-do-to-set-up-attribution}

1. 機會設定

   1. 確保機會與您的CRM同步
   1. 如果您的歸因設定設為「明確」，請確定已填入商機的聯絡角色
   1. 建議將歸因設定變更為混合式
   1. 計畫設定

      1. 將計畫成本納入您的計畫
      1. 檢閱Analytics行為，指出分析中是否應包含方案
      1. 為您擁有的每個管道設定成功標準
      1. 將人員連結至方案

         1. 請確定已為資料庫中的每個人設定贏取方案和贏取日期，以便首次接觸歸因能夠運作。
         1. 確保您的程式正在為資料庫中的人員設定成功狀態

>[!TIP]
>
>[本文章](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md)中詳細說明了所有需要的設定步驟。

## MPI和Program Analyzer之間有何差異？ {#whats-the-difference-between-mpi-and-the-program-analyzer}

Program Analyzer可讓您比較您最多四個測量中的計畫。 MPI可讓您分析您的管道和方案對所選量度（例如成功、建立的新機會等）的貢獻。 也可讓您根據所選的特定量度檢視12個月的管道趨勢。

## MPI與進階Report Builder之間有何差異？ {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

進階Report Builder （有時稱為RCE）是專為自助式（或臨機）報表所設計，通常由行銷作業完成。 MPI的設計可讓行銷主管和行銷人員按一下即可存取效能分析。 需要最少的設定。

## 貢獻日期篩選器中的「上一年」選項有什麼改變？ {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

我們已暫時移除「上一年」選取專案。 您仍然可以選擇使用「自訂日期範圍」選項來檢視整年的效能資料。
