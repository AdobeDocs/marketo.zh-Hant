---
description: 執行Campaign - Marketo檔案 — 產品檔案
title: 執行促銷活動
exl-id: d550cf08-b295-4289-9bb0-79d81cabc245
source-git-commit: 3b2bd965e37779af3ee89f46e04f925a2f12f207
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---

# 執行促銷活動 {#execute-campaign}

可執行的促銷活動和其他促銷活動一樣，包含智慧清單、流量和排程。 與其他促銷活動不同，您實際上並未排程或啟動它。 只能由其他促銷活動透過「執行促銷活動流程」步驟來呼叫。 可執行促銷活動中的流程步驟會與上層促銷活動一併執行（不同於在個別觸發促銷活動中並行執行的請求促銷活動）。

>[!NOTE]
>
>可執行的促銷活動一律為呼叫這些促銷活動的（父）促銷活動的子項。

## 何時執行促銷活動 {#when-to-use-execute-campaign}

執行檔促銷活動有許多可用的功能。 它們旨在促進常見的操作任務，如銷售機會路由、生命週期管理和計分（等等），並且可用於從批次或觸發的促銷活動中執行相同的工作流程。

在需要運行單獨的流時，您也可以使用它們，但在後續流步驟選擇中需要依賴該流的結果（即，如果這樣，則執行）。

執行促銷活動是 [要求促銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/request-campaign.md)，因為它可以串聯或並行執行，而後者只能並行執行。

>[!NOTE]
>
>等待步驟和Webhook永遠不會與執行檔促銷活動相容。 對於這些，您將需要改用「請求促銷活動」。

## 如何建立可執行的促銷活動 {#how-to-create-an-executable-campaign}

1. 按一下右鍵所需的程式並選擇 **新智慧型行銷活動**.

   ![](assets/execute-campaign-1.png)

1. 請為其命名，選取 **執行檔** 核取方塊，然後按一下 **建立**.

   ![](assets/execute-campaign-2.png)

1. 與任何其他智慧型促銷活動一樣，定義智慧清單和流量。

您也可以複製現有的智慧型促銷活動。 如果複製現有的執行檔促銷活動，您仍須選取 **執行檔** 命名後核取方塊。

>[!NOTE]
>
>您無法複製包含觸發器的促銷活動。

## 使用上層促銷活動代號內容 {#use-parent-campaign-token-context}

設為true時，會將下列Token內容傳送至子促銷活動（要執行的促銷活動）:

* 我的代號
* 促銷活動代號
* 程式代號
* 成員令牌
* [觸發Token](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) （如果從觸發促銷活動呼叫）

**API互動**

使用排程或請求促銷活動時 [在API中](https://developers.marketo.com/rest-api/assets/smart-campaigns/#batch)，都可讓您傳遞「我的代號」的值，而覆寫您呼叫之促銷活動中為這些代號設定的值。 如果該促銷活動接著執行另一個促銷活動並將「使用父內容」設為「True」，則會使用透過API傳遞的值，而非應用程式中設定的值。

## 注意事項 {#things-to-note}

* 智慧清單會篩選不符合資格的任何人。 如果人員符合資格，則產生的「已執行促銷活動」活動記錄會將其列為「合格：TRUE」（若不是，則為FALSE）
* 套用排程促銷活動資格規則（「排程」標籤下的「智慧促銷活動設定」）
* 無法跨工作區呼叫可執行的促銷活動
* 如果您使用 [從流中刪除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) 以執行檔促銷活動為目標的流程動作，會將目標同時鎖定於子項和父項
* 善用代號繼承 — 例如，如果您有由多個不同資產觸發的單一通用計分流程，則您可以在子促銷活動和父促銷活動中定義預設的「我的代號」分數，以便您能覆寫父促銷活動的子分數促銷活動值（請參閱下方的視覺範例）
* 可執行的促銷活動可調用至深達三個層級（例如，父促銷活動>子促銷活動>子促銷活動>子促銷活動）

>[!CAUTION]
>
>請勿讓執行檔促銷活動的智慧清單失效，否則 **無人** 會符合。 最佳作法是建立個別的智慧清單資產、完整定義資產，並確認資產有效。 然後，在可執行促銷活動中使用「智慧清單成員」篩選器，以便交換智慧清單定義。

## 代號繼承範例 {#token-inheritance-example}

以下是一個可執行促銷活動和兩個上層促銷活動中代號繼承的視覺範例：將令牌上下文設定為 **True**，另一個 **False**.

具有標籤化變更分數的子促銷活動。

![](assets/execute-campaign-3.png)

子促銷活動的「我的代號」。

![](assets/execute-campaign-4.png)

**範例一 — True**

在第一個上層促銷活動的「執行促銷活動」流程步驟中，「使用上層促銷活動代號內容」設為 **True**.

![](assets/execute-campaign-5.png)

父促銷活動的「我的代號」。

![](assets/execute-campaign-6.png)

結果：分數按+10變更。

![](assets/execute-campaign-7.png)

**範例二：False**

在第二個上層促銷活動的「執行促銷活動」篩選器中，「使用上層促銷活動代號內容」設為 **False**.

![](assets/execute-campaign-8.png)

父促銷活動的「我的代號」。

![](assets/execute-campaign-9.png)

結果：分數未變，因為已使用子促銷活動的分數值+0。

![](assets/execute-campaign-10.png)
