---
unique-page-id: 12979858
description: 效能分析常見問題集 — Marketo檔案 — 產品檔案
title: 績效分析常見問題集
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 0%

---

# 績效分析常見問題集 {#performance-insights-faq}

## 「參與」標籤中「成功」的定義是什麼？ {#what-is-the-definition-of-success-in-the-engagement-tab}

成功是衡量Marketo中有意義互動的指標。 方案的目的是與人員或潛在客戶建立有意義的互動。 當人員達到達到該目標的狀態時，就會標示成功。 它可以參加網路研討會、按一下電子郵件中的連結，或填寫網路表單。 成功視節目管道而定。

>[!NOTE]
>
>在網路研討會方案中，可能有多種狀態，例如：受邀、註冊和參加。 「已邀請」或「已註冊」沒有意義的互動，因為人們實際上不會觀看網路研討會。 在此情況下，已出席次數會視為成功。

## MPI是否可與任何CRM一起使用？ {#will-mpi-work-with-any-crm}

是. 技術上，MPI不會直接與CRM進行資料同步。 MPI利用儲存在Marketo AnalyticsData Warehouse中的資料。 由於CRM同步會在銷售機會管理應用程式中進行，因此任何與銷售機會管理應用程式整合的Marketo支援CRM都會正確顯示資料。 但是，CRM機會欄位確實需要正確映射到Marketo機會欄位。

## 我沒有任何其他行銷分析產品（ARB、RCE、RCA、方案分析）。 MPI能為我效用嗎？ {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI是銷售機會管理應用程式的獨立插件。 不需要使用任何其他分析產品。

## RCA還顯示了程式效能資料。 MPI和RCA中顯示的資料之間是否有差異？ {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

否. MPI從與RCA相同的資料倉庫中來源資料。 因此，您不會看到兩者之間有任何資料差異。 RCA可讓您即時建立自己的報表。 MPI使您能夠訪問易於理解的可視儀表板。

## 我不希望我的某些程式（例如操作）在MPI中顯示。 如何控制特定程式的可見性？ {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

您可以將方案的Analytics行為設為「運作」，借此控制方案的可見性。 這會導致程式從分析計算中排除。

>[!NOTE]
>
>深入了解如何設定分析行為 [此處](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## 我正在為新產品發佈執行多管道行銷活動。 如何在一個位置檢視此促銷活動在所有不同管道中的績效？ {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

建議您針對這類行銷活動的方案部分，使用方案標籤。 程式標籤會自動同步到MPI，您可以在所有MPI控制面板中篩選這些標籤，以查看您的多通道促銷活動效能。

## 如果沒有RCA，我可以存取歸因設定嗎？ {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

如果您有MPI，無論您是否有RCA，都能存取歸因設定。

## 當我登入時，系統會在MPI中收到通知，告知我的歸因設定不正確。 怎麼了？ {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI計算是否所有機會都包括在分析中。 若未包含，系統會提示您考慮變更歸因設定（明確、隱含、混合），以納入更多商機。

由於程式成本在程式中丟失，您可能也會丟失機會。 請檢閱您方案的Analytics行為。 可以是：

1. 預設 — 預設行為是，只有在至少存在一個期間成本（即使分配了零美元）時，程式才會包含在MPI中。

1. 包含 — 此選項將確保程式在MPI中可用，而不管您是否已包括期間成本。

1. [操作](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs)  — 此選項會導致程式不顯示在MPI中。

>[!NOTE]
>
>期間成本 **has** 以在「參與」控制面板中為「成功與新名稱」報表進行設定。 此儀表板使用期間成本資料來匯總成功和新名稱。 如果未設定期間成本，無論上述Analytics行為設定為何，參與控制面板都無法正確報告。

## 為什麼我在MPI中漏掉了一些機會？ {#why-am-i-missing-some-opportunities-in-mpi}

在MPI中您可能缺少機會的兩個主要原因是：

1. 歸因設定設定為「顯式」，但未分配聯繫人角色
1. 期間成本不包含在您的方案中

MPI計算是否所有機會都包括在分析中。 若未包含，系統會提示您考慮變更歸因設定（明確、隱含、混合），以納入更多商機。

由於程式成本在程式中丟失，您可能也會丟失機會。 警報會出現，但不會指出哪些程式缺少成本。 請檢查您的程式設定以包括成本，以確保MPI中包含您的所有程式和機會。

## 為什麼在「參與」儀表板上看不到「自定義欄位」、「機會類型」和「ABM篩選器」？ {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

自定義欄位、機會類型和ABM篩選器都是與機會相關的屬性。 「參與」儀表板允許您測量您的參與和潛在客戶贏取，無論它們是否與業務機會關聯。 由於「參與」儀表板未考慮機會，因此「自定義欄位」、「機會類型」和「ABM過濾器」不適用。

## 我想使用自定義的Salesforce Opportunity欄位來報告收入，而不是標準的Salesforce Opportunity Amount欄位。 MPI允許我這樣做嗎？ {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

是. [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support) 只要欄位類型為貨幣，就能將Marketo的Opportunity Amount欄位重新映射到自定義的Salesforce Opportunity欄位。 由於MPI指向「Marketo機會」量欄位，因此MPI可以使用重新映射的自定義Salesforce欄位中的資料。

>[!NOTE]
>
>重新映射後，MPI將顯示未來的資料。 歷史數量不會更改。

## 如果我不利用機會，我還能使用MPI嗎？ {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI旨在讓您從漏斗頂部到收入影響，衡量程式效能。 如果您不使用機會，您仍可以：

* 檢視您培養受眾參與程式的效能。
* 查看潛在客戶獲取計畫的效能。
* 透過方案標籤檢視多通道行銷活動的效能。
* 查看過去12個月的受眾參與趨勢。
* 在PowerPoint中保存和導出效能資料。

## 我可以評估MPI中基於帳戶的策略的成功嗎？ {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

是. MPI與 [Marketo](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) 無縫地將ABM帳戶清單納入MPI。 您可以使用「ABM帳戶清單」篩選器來選擇所需的ABM清單，以依此篩選資料。

## 購買MPI時，歸因是否可立即使用？ {#is-attribution-instantly-available-when-i-purchase-mpi}

客戶購買MPI時，可使用Marketo歸因功能。 不過， [正確設定](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) 需要，以確保機會和程式資料正確地流入MPI。

## 設定歸因需要執行什麼動作？ {#what-do-i-have-to-do-to-set-up-attribution}

1. 機會設定

   1. 確保機會與CRM同步
   1. 如果「歸因」設定設定為「明確」，請確保填入了商機的聯繫人角色
   1. 建議您將「歸因」設定變更為「混合」
   1. 程式設定

      1. 將計畫成本納入您的計畫
      1. 檢閱分析行為，以指出是否應將程式納入分析
      1. 為您擁有的每個管道設定成功標準
      1. 將人員與方案關聯

         1. 請確定已為資料庫中的每個人設定贏取方案和贏取日期，以便首次接觸歸因運作。
         1. 確保您的程式正在為資料庫中的人員設定成功狀態

>[!TIP]
>
>所有所需的設定步驟在 [這篇文章](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## MPI和程式分析器之間有何區別？ {#whats-the-difference-between-mpi-and-the-program-analyzer}

程式分析器允許您將程式與多達四個度量進行比較。 MPI允許您分析對選定度量（如「成功」、「新建機會」等）的渠道和程式貢獻。 它也可讓您根據您選擇的特定量度，檢視12個月的管道趨勢。

## MPI與高級Report Builder有何不同？ {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

進階Report Builder（有時稱為RCE）專為自助（或臨機）報表而設計，通常由行銷營運完成。 MPI旨在讓行銷領導者和行銷人員按一下就能存取效能分析。 需要的設定最少。

## 貢獻的日期篩選條件中的「上一年」選項有什麼改變？ {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

我們暫時刪除了「前一年」選項。 您仍可以選擇使用「自訂日期範圍」選項來檢視整年的效能資料。
