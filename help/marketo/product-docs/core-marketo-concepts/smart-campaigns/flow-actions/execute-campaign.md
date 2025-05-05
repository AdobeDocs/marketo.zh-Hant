---
description: 執行行銷活動 — Marketo檔案 — 產品檔案
title: 執行行銷活動
exl-id: d550cf08-b295-4289-9bb0-79d81cabc245
feature: Smart Campaigns
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# 執行行銷活動 {#execute-campaign}

與其他行銷活動一樣，可執行行銷活動包含智慧清單、流量和排程。 不像其他行銷活動，您實際上並不會排程或啟用它。 它只能由其他行銷活動透過執行行銷活動流程步驟呼叫。 可執行行銷活動中的流程步驟會與父行銷活動串連執行（不同於要求行銷活動，後者會在個別的觸發行銷活動中並行執行）。

>[!NOTE]
>
>可執行行銷活動一律為呼叫它們的（父）行銷活動的子系。

## 何時使用執行行銷活動 {#when-to-use-execute-campaign}

您可以使用可執行促銷活動執行許多作業。 它們旨在協助執行常見的營運任務，例如銷售機會路由、生命週期管理和評分（等等），並可用於從批次或觸發的行銷活動中執行相同的工作流程。

當您需要執行個別的流程時，也可以使用它們，但您必須在後續的流程步驟選擇中依賴該流程的結果（亦即，如果是，則需這樣做）。

執行行銷活動是[要求行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/request-campaign.md)的改進，因為它可以串列執行，而後者只能平行執行。

>[!NOTE]
>
>等待步驟和Webhook絕不會與可執行行銷活動相容。 若要使用這些工具，您需要改用「請求行銷活動」。

## 如何建立可執行的行銷活動 {#how-to-create-an-executable-campaign}

1. 用滑鼠右鍵按一下您想要的程式，然後選取&#x200B;**[!UICONTROL 新增Smart Campaign]**。

   ![](assets/execute-campaign-1.png)

1. 指定名稱，選取&#x200B;**[!UICONTROL 可執行檔]**&#x200B;核取方塊，然後按一下&#x200B;**[!UICONTROL 建立]**。

   ![](assets/execute-campaign-2.png)

1. 定義智慧列示和流量，就像任何其他Smart Campaign。

您也可以複製現有的Smart Campaign。 如果您複製現有的「可執行檔行銷活動」，您仍需在命名後選取「**[!UICONTROL 可執行檔]**」核取方塊。

>[!NOTE]
>
>您無法複製包含觸發器的行銷活動。

## 使用父級行銷活動代號內容 {#use-parent-campaign-token-context}

設為true時，系統會將下列權杖內容傳送至子行銷活動（正在執行的行銷活動）：

* 我的Token
* 行銷活動Token
* 計畫權杖
* 成員Token
* [觸發權杖](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) （若是從已觸發的行銷活動呼叫）

**API互動**

在API[&#128279;](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/assets/smart-campaigns#batch)中使用排程或請求促銷活動時，兩者都可以讓您傳遞「我的Token」的值，這會覆寫在您呼叫之促銷活動中為這些Token設定的值。 如果該行銷活動接著執行另一個行銷活動並設定「使用父項內容為True」，則它會使用透過API傳遞的值，而不是應用程式中設定的值。

## 注意事項 {#things-to-note}

* 智慧清單會篩選出不符合資格的任何人。 如果有人符合資格，則產生的已執行行銷活動記錄會將其列為「合格：TRUE」（否則為FALSE）
* 套用排程行銷活動資格規則（「排程」標籤下的「智慧型行銷活動設定」）
* 無法跨工作區呼叫可執行行銷活動
* 如果您使用以可執行檔促銷活動為目標的[從流量中移除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md)流量動作，則會同時以子項和父項為目標
* 善用代號繼承 — 例如，如果您有一個由多個不同資產觸發的通用評分流程，您可以在子行銷活動和父行銷活動中定義預設的「我的代號」分數，以便您可以覆寫父行銷活動的子級分數行銷活動值（請參閱以下視覺範例）
* 可執行行銷活動最多可呼叫三層深（例如，父行銷活動>子項>子項>子項）

>[!CAUTION]
>
>切勿讓可執行行銷活動的智慧清單無效，否則&#x200B;_沒有人_&#x200B;符合資格。 最佳實務建議建立個別的智慧清單資產、完整定義資產，並確保其有效。 然後，使用可執行促銷活動中的「智慧列示成員」篩選器，以交換智慧列示定義。

## 權杖繼承範例 {#token-inheritance-example}

以下是一個可執行行銷活動和兩個父行銷活動中的權杖繼承的視覺範例：一個權杖內容設為&#x200B;**[!UICONTROL True]**，另一個設為&#x200B;**[!UICONTROL False]**。

具有代碼化變更分數的子行銷活動。

![](assets/execute-campaign-3.png)

兒童行銷活動的My Token。

![](assets/execute-campaign-4.png)

### 範例一 — True {#example-one-true}

在第一個父級促銷活動的「執行促銷活動」流程步驟中，「使用父級促銷活動代號內容」設為&#x200B;**True**。

![](assets/execute-campaign-5.png)

父級行銷活動的「我的Token」。

![](assets/execute-campaign-6.png)

結果：分數已變更+10。

![](assets/execute-campaign-7.png)

### 範例二：False {#example-two-false}

在第二個父級促銷活動的「執行促銷活動」流程步驟中，「使用父級促銷活動代號內容」設為&#x200B;**False**。

![](assets/execute-campaign-8.png)

父級行銷活動的「我的Token」。

![](assets/execute-campaign-9.png)

結果：分數未變更，因為已使用子行銷活動的分數值+0。

![](assets/execute-campaign-10.png)
