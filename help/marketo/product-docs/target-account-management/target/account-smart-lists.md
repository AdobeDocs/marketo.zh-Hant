---
unique-page-id: 11378814
description: 帳戶智慧清單 — Marketo檔案 — 產品檔案
title: 帳戶智慧清單
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
feature: Target Account Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# 帳戶智慧清單 {#account-smart-lists}

以下說明如何快速準確地識別您的高價值帳戶。

>[!NOTE]
>
>此功能僅適用於同時具有Target帳戶管理附加元件和已核發TAM授權的使用者。

## 建立帳戶智慧清單 {#create-an-account-smart-list}

1. 在Marketo中，移至&#x200B;**行銷活動**。

   ![](assets/account-smart-lists-1.png)

1. 尋找並選取所需的程式。

   ![](assets/account-smart-lists-2.png)

1. 按一下&#x200B;**新增**&#x200B;下拉式清單，然後選取&#x200B;**新增本機資產**。

   ![](assets/account-smart-lists-3.png)

1. 按一下&#x200B;**帳戶智慧清單**。

   ![](assets/account-smart-lists-4.png)

1. 輸入名稱，然後按一下&#x200B;**建立** （說明和標籤是選擇性的）。

   ![](assets/account-smart-lists-5.png)

您的帳戶智慧清單已建立！ 如需定義其規則的步驟，請參閱下文。

## 帳戶智慧清單規則 {#account-smart-list-rules}

帳戶智慧列示的運作方式與標準智慧列示類似，但有顯著的例外：容器。

1. 若要定義您的帳戶智慧清單，請按一下&#x200B;**帳戶智慧清單規則**&#x200B;標籤。

   ![](assets/account-smart-lists-6.png)

1. 選擇您需要的帳戶篩選器。 在此範例中，我們選擇&#x200B;_產業是醫療保健_。

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

就是這樣！ 請參閱下節，瞭解如何運用您的帳戶智慧清單。

>[!TIP]
>
>就像使用標準智慧列示一樣，您可以使用進階邏輯來進一步調整結果。 若要這麼做，您至少需要三個篩選器，而在「帳戶智慧清單」中，一個容器（無論其本身包含多少篩選器）等於一個篩選器。

## 帳戶智慧清單動作 {#account-smart-list-actions}

在帳戶智慧清單的「概觀」標籤中，您會注意到一些動作選項。

**匯出**：這會將您帳戶智慧清單的結果匯出為CSV。

**複製**：製作帳戶智慧清單的復本。

**傳送至廣告網路**：將清單作為新的相符對象傳送至LinkedIn。

您也可以使用&#x200B;_帳戶智慧清單的人員_&#x200B;篩選器，在標準智慧行銷活動/清單中參考您的帳戶智慧清單。

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>「帳戶智慧清單中的人員」成員的結果將顯示已識別帳戶中的每個人，而不僅僅是透過帳戶智慧清單中的相符人員篩選器找到的人員。

>[!NOTE]
>
>**定義**
>
>**帳戶智慧清單的人員成員**：在此案例中，「成員」一詞是指帳戶本身，因此「人員成員」是指這些帳戶中的實際人員(Marketo記錄)。
