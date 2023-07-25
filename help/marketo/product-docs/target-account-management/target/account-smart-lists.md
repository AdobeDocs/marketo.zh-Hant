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
>此功能僅適用於同時具有Target帳戶管理附加元件和已核發的TAM授權的使用者。

## 建立帳戶智慧清單 {#create-an-account-smart-list}

1. 在Marketo中，前往 **行銷活動**.

   ![](assets/account-smart-lists-1.png)

1. 尋找並選取您需要的程式。

   ![](assets/account-smart-lists-2.png)

1. 按一下 **新增** 下拉式清單並選取 **新增本機資產**.

   ![](assets/account-smart-lists-3.png)

1. 按一下 **帳戶智慧清單**.

   ![](assets/account-smart-lists-4.png)

1. 輸入名稱並按一下 **建立** （說明和標籤為選用）。

   ![](assets/account-smart-lists-5.png)

您的帳戶智慧清單已建立！ 如需定義其規則的步驟，請參閱下文。

## 帳戶智慧清單規則 {#account-smart-list-rules}

帳戶智慧列示的運作方式與標準智慧列示類似，但有顯著的例外：容器。

1. 若要定義您的帳戶智慧清單，請按一下 **帳戶智慧清單規則** 標籤。

   ![](assets/account-smart-lists-6.png)

1. 選擇所需的帳戶篩選器。 在此範例中，我們選擇 _產業是醫療保健_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >您所使用的內部版本指示器資料 [帳戶設定檔排名與調整](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) 將顯示為自訂帳戶屬性，以便在您的帳戶智慧清單中使用。 此自訂屬性資料是根據帳戶設定檔模型的建立/更新時間。

1. 選擇相符的人員篩選器。 在此範例中，我們選擇 _州為加州_.

   ![](assets/account-smart-lists-9.png)

**選擇性步驟**：容器可在此使用。 如果您選擇其他相符人員篩選器，可將其拖曳至第一個篩選器下方，或 _在_ 建立容器。 在此範例中，我們透過新增以下內容來建立容器 _職稱是CFO_.

![](assets/account-smart-lists-10.png)

以下是容器的外觀。

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>建立篩選器容器會建立「與」規則，這表示它只會傳回所有合併的結果。 在此範例中，帳戶位於加州且擁有醫療保健產業 _和_ 而某位新同事被列為CFO。 如果您不想使用容器，只需將篩選器拖曳至現有篩選器的下方/上方。

就是這樣！ 請參閱下節，瞭解如何善用您的帳戶智慧清單。

>[!TIP]
>
>就像使用標準智慧列示一樣，您可以使用進階邏輯來進一步調整結果。 您至少需要三個篩選器才能這麼做，而在帳戶智慧清單中，一個容器（無論其本身包含多少個篩選器）等於一個篩選器。

## 帳戶智慧清單動作 {#account-smart-list-actions}

在「帳戶智慧清單」的「概述」標籤中，您會注意到一些動作選項。

**匯出**：這會將「帳戶智慧清單」的結果匯出為CSV。

**原地複製**：為您的帳戶智慧清單製作副本。

**傳送至Ad Network**：將清單當作新的相符對象傳送至LinkedIn。

您也可以使用「 」，在標準智慧行銷活動/清單中參照帳戶智慧清單。 _帳戶智慧清單的人員成員_ 篩選。

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>「帳戶智慧清單中的人員」成員的結果將顯示已識別帳戶中的每個人，而不僅僅是透過帳戶智慧清單中的相符人員篩選器找到的人員。

>[!NOTE]
>
>**定義**
>
>**帳戶智慧清單的人員成員**：在此案例中，「會員」一詞是指帳戶本身，因此「人民會員」是指這些帳戶中的實際人民(Marketo記錄)。
