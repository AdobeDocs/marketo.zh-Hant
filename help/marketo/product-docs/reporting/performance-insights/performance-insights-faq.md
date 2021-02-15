---
unique-page-id: 12979858
description: 效能分析常見問答集——行銷人員檔案——產品檔案
title: 效能分析常見問答集
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 0%

---


# 效能分析常見問答{#performance-insights-faq}

## 「參與」標籤中「成功」的定義為何？{#what-is-the-definition-of-success-in-the-engagement-tab}

成功是Marketo中有意義互動的度量。 程式的目的，是與人或潛在客戶建立有意義的互動。 當某人達到達到該目標的狀態時，就會標籤成功。 它可以參加網路研討會、按一下電子郵件中的連結，或填寫網頁表格。 成功視程式管道而定。

>[!NOTE]
>
>**範例**
>
>在網路研討會課程中，可能有多種狀態，例如：已邀請、已註冊及已參加。 「已邀請」或「已註冊」並不是有意義的互動，因為人們實際上不會觀看網路研討會。 在此案例中，參與者被視為成功。

## MPI是否可與任何CRM搭配運作？{#will-mpi-work-with-any-crm}

是的。 從技術上講，MPI不直接與CRM進行資料同步。 MPI運用儲存在Marketon Analytics資料倉庫中的資料。 由於CRM同步發生在銷售機會管理應用程式中，因此與銷售機會管理應用程式整合的任何由行銷人員支援的CRM都會正確顯示資料。 但是， CRM業務機會欄位確實需要正確映射到Marketo業務機會欄位。

## 我沒有其他任何行銷分析產品（ARB、RCE、RCA、計劃分析）。 MPI是否適合我？{#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI是銷售線索管理應用程式的獨立附加模組。 它不需要使用任何其他分析產品。

## RCA也顯示了程式效能資料。 MPI和RCA中顯示的資料是否有差異？{#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

不。 MPI從與RCA相同的資料倉庫中收集資料。 因此，您不會看到兩者之間的資料差異。 RCA可讓您即時建立自己的報表。 MPI可讓您存取簡單明瞭的視覺控制面板。

## 我不希望我的某些程式（例如操作）在MPI中顯示。 如何控制特定程式的可見度？{#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

您可以將程式的Analytics行為設為「營運」，以控製程式的可見度。 這會導致程式被排除在分析計算之外。

>[!NOTE]
>
>進一步瞭解如何設定分析行為[這裡](https://docs.marketo.com/display/public/DOCS/Edit+Analytics+Behavior+Settings)。

## 我正在執行多通道促銷活動，以推出新產品。 我要如何在一個位置檢視此促銷活動在所有不同通道的績效？{#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

我們建議您針對此類促銷活動中的方案，使用方案標籤。 程式標籤會自動同步至MPI，您可以在所有MPI儀表板中篩選，以檢視多通道促銷活動效能。

## 如果沒有RCA，我是否可存取歸因設定？{#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

如果您有MPI，無論您是否有RCA，都可以訪問歸因設定。

## 當我登入時，在MPI中會收到警告，告知我的歸因設定不正確。 有什麼問題？{#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI會計算您的所有機會是否都包含在分析中。 如果沒有，系統會提示您考慮變更歸因設定（明確、隱含、混合），以包含更多機會。

您也可能因為方案成本遺失而錯失了機會。 請檢閱您程式的Analytics行為。 它們可以是：

1. 預設——預設行為是，只有在至少有一個期間成本（即使分配了零美元）時，程式才會包括在MPI中。
1. 包含——此選項將確保程式在MPI中可用，無論您是否已包括期間成本。
1. [Operational](https://docs.marketo.com/display/DOCS/Best+Practice%3A+How+to+Organize+your+Programs#BestPractice:HowtoOrganizeyourPrograms-OperationalPrograms)  —— 此選項導致程式不顯示在MPI中。

>[!NOTE]
>
>期間成本&#x200B;**有**&#x200B;要在「參與」儀表板中為「成功」和「新名稱」報告設定。 此控制面板利用期間成本資料來匯總成功和新名稱。 如果未設定「期間成本」，無論上述Analytics行為設定為何，參與控制面板都無法正確報告。

## 我為什麼在MPI中錯失了一些機會？{#why-am-i-missing-some-opportunities-in-mpi}

MPI中可能缺少機會的兩個主要原因是：

1. 歸因設定設定為「明確」，但業務機會沒有分配「聯繫人角色」
1. 期間成本不包含在您的方案中

MPI會計算您的所有機會是否都包含在分析中。 如果沒有，系統會提示您考慮變更歸因設定（明確、隱含、混合），以包含更多機會。

您也可能因為方案成本遺失而錯失了機會。 警報會出現，但不會指出哪些程式缺少成本。 請查看您的程式設定以包括成本，以確保MPI中包含您的所有程式和機會。

## 為什麼我在「參與」儀表板上看不到「自定義欄位」、「機會類型」和「ABM」篩選器？{#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

自定義欄位、業務機會類型和ABM篩選器都是與業務機會相關的所有屬性。 「參與」儀表板允許您衡量您的參與和潛在客戶獲取，無論它們是否與業務機會關聯。 由於「參與」儀表板不考慮機會，因此不適用「自定義欄位」、「機會類型」和「ABM篩選器」。

## 我想使用自訂的Salesforce Opportunity欄位來報告收入，而非標準的Salesforce Opportunity Amount欄位。 MPI是否允許我這樣做？{#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

是的。 [只要](https://docs.marketo.com/cdn-cgi/l/email-protection#b5c6c0c5c5dac7c1f5d8d4c7ded0c1da9bd6dad8) 欄位類型是貨幣，Marketo Supportion就能將Marketo的Opportunity Amount欄位重新對應至自訂的Salesforce Opportunity欄位。由於MPI指向Marketo Opportunity金額欄位，因此MPI可以使用重新映射的自訂Salesforce欄位中的資料。

>[!NOTE]
>
>在重新映射後，MPI將顯示資料。 歷史數量不會改變。

## 如果我不利用機會，我是否仍能使用MPI?{#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI旨在讓您從漏斗頂部到收入影響，衡量程式效能。 如果您不使用機會，您仍能：

* 檢視您的培養計畫的效能，以吸引受眾。
* 檢視您的潛在客戶獲取計畫的效能。
* 透過方案標籤檢視多通道促銷活動的效能。
* 查看過去12個月的受眾參與趨勢。
* 在PowerPoint中儲存和匯出效能資料。

## 我可以衡量MPI中基於帳戶的策略的成功嗎？{#can-i-measure-the-success-of-account-based-strategies-in-mpi}

是的。 MPI與[Marketo ABM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview)整合，將ABM帳戶清單順暢地匯入MPI。 您可以使用「ABM帳戶清單」篩選器來選擇所需的ABM清單以篩選資料。

## 我購買MPI時是否可立即使用歸因？{#is-attribution-instantly-available-when-i-purchase-mpi}

客戶購買MPI時，可使用Marketo Attribution功能。 但是，需要[正確設定](https://docs.marketo.com/x/mRPG)以確保機會和程式資料正確地流入MPI。

## 我要如何設定歸因？{#what-do-i-have-to-do-to-set-up-attribution}

1. 業務機會設定

   1. 確保機會與您的CRM同步
   1. 如果您的「歸因」設定設定為「明確」，請確定已填入商機的聯絡角色
   1. 我們建議將「歸因」設定變更為Hybrid
   1. 方案設定

      1. 將方案成本納入您的方案
      1. 檢閱分析行為，以指出應否將程式納入分析
      1. 為您擁有的每個渠道設定成功標準
      1. 將人員與程式系結

         1. 請確定已為資料庫中的每個人設定「贏取計畫」和「贏取日期」，以便「首次接觸歸因」運作。
         1. 確保您的程式正在為資料庫中的人員設定成功狀態

>[!TIP]
>
>[本文](https://docs.marketo.com/x/mRPG)中詳細說明了所需的所有設定步驟。

## MPI和程式分析器之間有何區別？{#whats-the-difference-between-mpi-and-the-program-analyzer}

Program Analyzer允許您最多比較四個度量的程式。 MPI可讓您分析您的渠道和程式對選定度量的貢獻，如「成功」、「已建立的新機會」等。 它也可讓您根據您選擇的一個特定度量，檢視12個月的渠道趨勢。

## MPI和進階報告建立工具之間有何差異？{#whats-the-difference-between-mpi-and-the-advanced-report-builder}

進階報表產生器（有時稱為RCE）是專為自助（或臨機）報表而設計，通常由行銷營運部門完成。 MPI旨在讓行銷領導者和行銷人員只需按一下即可存取效能分析。 需要最少的設定。

## 貢獻的日期篩選中的「上一年」選項有何改變？{#what-happened-to-the-previous-year-option-in-contributions-date-filter}

我們暫時移除了&quot;上一年&quot;的選項。 您仍然可以選擇使用「自訂日期範圍」選項來檢視全年的效能資料。
