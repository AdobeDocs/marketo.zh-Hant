---
unique-page-id: 11378814
description: 帳戶智慧清單 — Marketo檔案 — 產品檔案
title: 帳戶智慧清單
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
source-git-commit: e4d581ab258a875747a6d5323764e8b4a3949cba
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 帳戶智慧清單 {#account-smart-lists}

以下說明如何快速準確地識別您的高價值客戶。

>[!NOTE]
>
>此功能僅適用於具有Target帳戶管理附加元件和已核發TAM授權的使用者。

## 建立帳戶智慧清單 {#create-an-account-smart-list}

1. 在Marketo中，前往 **行銷活動**.

   ![](assets/account-smart-lists-1.png)

1. 尋找並選取您想要的方案。

   ![](assets/account-smart-lists-2.png)

1. 按一下 **新增** 下拉式清單並選取 **新本機資產**.

   ![](assets/account-smart-lists-3.png)

1. 按一下 **帳戶智慧清單**.

   ![](assets/account-smart-lists-4.png)

1. 輸入名稱，然後按一下 **建立** （說明和標籤為選用）。

   ![](assets/account-smart-lists-5.png)

已建立您的帳戶智慧清單！ 請參閱下方，了解定義其規則的步驟。

## 帳戶智慧清單規則 {#account-smart-list-rules}

帳戶智慧清單的運作方式與標準智慧清單類似，但有一個明顯的例外：容器。

1. 要定義帳戶智慧清單，請按一下 **帳戶智慧清單規則** 標籤。

   ![](assets/account-smart-lists-6.png)

1. 選擇您想要的帳戶篩選器。 在這個例子中，我們 _行業就是醫療保健_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

1. 選擇您的相符人員篩選器。 在這個例子中，我們 _加州_.

   ![](assets/account-smart-lists-9.png)

**可選步驟**:這裡是容器的入口。 如果您選擇其他「符合的人員篩選」，您可以將其拖曳至第一個篩選下，或 _in_ 建立容器。 在此範例中，我們是透過新增 _職銜是首席財務官_.

![](assets/account-smart-lists-10.png)

容器的外觀如下。

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>建立篩選器的容器會建立「和」規則，這表示它只會傳回所有結合的結果。 在此範例中，說明醫療保健產業以及位於加州 _和_ 被列為首席財務官的人。 如果您不想使用容器，只需將篩選器拖曳至現有篩選器的下方/上方即可。

就這樣！ 請查看以下小節，了解如何運用您的帳戶智慧清單。

>[!TIP]
>
>就像標準智慧清單一樣，您可以使用進階邏輯來進一步調整結果。 您至少需要三個篩選器才能執行此操作，而在「帳戶智慧清單」中，一個容器（無論其本身包含多少個篩選器）等於一個篩選器。

## 帳戶智慧清單動作 {#account-smart-list-actions}

在「帳戶智慧清單」的「概述」標籤中，您會注意到一些動作選項。

**匯出**:這會將「帳戶智慧清單」的結果匯出為CSV。

**原地複製**:製作帳戶智慧清單的副本。

**傳送至廣告網路**:將清單以新的「相符對象」形式傳送至LinkedIn。

您也可以使用 _帳戶智慧清單的人員成員_ 篩選。

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>帳戶智慧清單的人員成員結果會顯示已識別帳戶中的每個人，而不只是透過帳戶智慧清單中的相符人員篩選器找到的人員。

>[!NOTE]
>
>**定義**
>
>**帳戶智慧清單的人員成員**:在這種情況下，「成員」一詞指的是帳戶本身，因此「人員成員」是指這些帳戶中的實際人員(Marketo記錄)。
