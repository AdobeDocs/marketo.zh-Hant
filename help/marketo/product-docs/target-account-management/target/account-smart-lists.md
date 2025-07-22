---
unique-page-id: 11378814
description: 帳戶智慧清單 — Marketo檔案 — 產品檔案
title: 帳戶智慧清單
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 帳戶智慧清單 {#account-smart-lists}

以下說明如何快速準確地識別您的高價值帳戶。

>[!NOTE]
>
>此功能僅適用於同時具有[!UICONTROL Target Account Management]附加元件和已核發的TAM的使用者。

## 建立[!UICONTROL Account Smart List] {#create-an-account-smart-list}

1. 在Marketo中，移至&#x200B;**[!UICONTROL Marketing Activities]**。

   ![](assets/account-smart-lists-1.png)

1. 尋找並選取所需的程式。

   ![](assets/account-smart-lists-2.png)

1. 按一下&#x200B;**[!UICONTROL New]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL New Local Asset]**。

   ![](assets/account-smart-lists-3.png)

1. 按一下「**[!UICONTROL Account Smart List]**」。

   ![](assets/account-smart-lists-4.png)

1. 輸入名稱並按一下&#x200B;**[!UICONTROL Create]** （說明和標籤為選用）。

   ![](assets/account-smart-lists-5.png)

已建立您的[!UICONTROL Account Smart List]！ 如需定義其規則的步驟，請參閱下文。

## [!UICONTROL Account Smart List]個規則 {#account-smart-list-rules}

[!UICONTROL Account Smart Lists]的工作方式與標準智慧列示類似，但有顯著的例外狀況：容器。

1. 若要定義您的[!UICONTROL Account Smart List]，請按一下&#x200B;**[!UICONTROL Account Smart List Rules]**&#x200B;標籤。

   ![](assets/account-smart-lists-6.png)

1. 選擇您需要的帳戶篩選器。 在此範例中，我們選擇&#x200B;_[!UICONTROL Industry]為[!UICONTROL Healthcare]_。

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >在您的[帳戶分析排名與調整](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md)中使用的ICP指標資料，將顯示為自訂的帳戶屬性，以便在您的帳戶智慧清單中使用。 此自訂屬性資料是根據帳戶設定檔模型的建立/更新時間。

1. 選擇相符的人員篩選器。 在此範例中，我們選擇&#x200B;_加州為_。

   ![](assets/account-smart-lists-9.png)

**選擇性步驟**：容器由此而來。 如果您選擇其他相符人員篩選器，您可以將它拖放到第一個篩選器下方，或將&#x200B;_放在_&#x200B;中，以建立容器。 在此範例中，我們透過新增&#x200B;_職稱是CFO_&#x200B;來建立容器。

![](assets/account-smart-lists-10.png)

以下是容器的外觀。

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>建立篩選器的容器會建立「and」規則，這表示它只會傳回所有合併的結果。 在此範例中，帳戶擁有醫療保健產業，以及位於加州&#x200B;_和_，且某人被列為CFO。 如果您不想使用容器，只需將篩選器拖曳至現有篩選器的下方/上方。

就是這樣！ 請參閱下節以瞭解如何善用您的[!UICONTROL Account Smart List]。

>[!TIP]
>
>就像使用標準智慧列示一樣，您可以使用進階邏輯來進一步調整結果。 若要這麼做，您至少需要三個篩選器，而在[!UICONTROL Account Smart Lists]中，一個容器（無論其本身包含多少篩選器）等於一個篩選器。

## [!UICONTROL Account Smart List]個動作 {#account-smart-list-actions}

在[!UICONTROL Account Smart List]的「概觀」標籤中，您會注意到一些動作選項。

**[!UICONTROL Export]**：這會將您[!UICONTROL Account Smart List]的結果匯出為CSV。

**[!UICONTROL Clone]**：製作您的[!UICONTROL Account Smart List]復本。

**[!UICONTROL Send to Ad Network]**：將清單當作新的相符對象傳送給[!DNL LinkedIn]。

您也可以使用[!UICONTROL Account Smart List]篩選器，在標準智慧行銷活動/清單中參考您的&#x200B;_[!UICONTROL People Member of Account Smart List]_。

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>[!UICONTROL People Member of Account Smart List]的結果將顯示已識別帳戶中的每個人，而不僅僅是透過帳戶智慧清單中的相符人員篩選器找到的人。

>[!NOTE]
>
>**定義**
>
>**[!UICONTROL People Member of Account Smart List]**：在此案例中，「會員」一詞是指帳戶本身，因此「人員會員」是指這些帳戶中的實際人員(Marketo記錄)。
