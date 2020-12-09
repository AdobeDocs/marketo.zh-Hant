---
title: 瞭解目標跟蹤和預測註冊
description: 瞭解目標追蹤和預計註冊
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 0%

---


# 瞭解目標追蹤和預計註冊

<br> 

在設 [定活動目標](/help/sky/setting-event-goals.md)，並透過智慧型促銷活動傳送邀 [請後](/help/sky/create-a-smart-campaign.md)，以下說明如何追蹤目標進度並瞭解Marketo的預測。

>[!NOTE]
>
>在Marketo Classic中建立事件程式時，事件開始日期目前預設為事件建立日期。 由於預計註冊會考量事件開始日期之前的時間，因此如果開始日期和建立日期相同，這些數字可能不正確（除非有意設定）。

## 目標追蹤和預計註冊

1. 您可以在事件程式的標籤中找 **[!UICONTROL Reports]** 到目標追蹤詳細資訊。 在這個具體例子中，到目前為止有150名註冊會員，而目標是200(75%)。

   ![影像一](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-1.png)

您也會看到您的注 **[!UICONTROL Projected]** 冊。 將滑鼠指標暫留在資訊圖示上，即可檢視此數字的「似然」區段劃分。

![影像2](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>「已出席」和「較高」圖表在活動當天之前仍為空。

1. 按一下圖表切換，可依註冊可能性切換至成員的劃分。 您會看到每個區段的目前註冊百分比，與過去方案中該區段的平均百分比相比。

   ![影像三](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-3.png)

所有成員（已註冊且尚未註冊）都會根據其註冊可能性分類。 將滑鼠指標暫留在資訊圖示上，以檢視這些可能性類別的定義方式。

![影像4](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-4.png)

>[!NOTE]
>
>預測數字會每24小時更新一次，直到事件發生當日為止。 列為「處理」(_Processing_)的任何成員都將包括在下一個計算週期中。

## 類似方案

您可以檢視過去執行的類似程式，從而深入瞭解目前的事件。 本節顯示自過去6個月以來最多5個類似方案，以及註冊或更高的成&#x200B;_員_ /百分比。

在計算類似程式時，主要包括以下因素：

* 程式類型
* 節目頻道
* 受眾規模
* 方案標籤
* 從事件建立到事件開始的持續時間
* 事件持續時間

   ![影像5](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-5.png)

## 建議

在「報表」頁面的頂端，您可以根據您的進度尋找AI/ML導向的建議。 請定期回訪，以取得有用的提示和見解！

![影像6](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-6.png)

## 人員層級預測

按一下該&#x200B;**[!UICONTROL Members]** 頁籤可查看您的所有方案成員。 將滑鼠指標暫留 **[!UICONTROL Registration Likelihood]** 在或 **[!UICONTROL Attendance Likelihood]** 長條上，以檢視確切的百分比和分類。 然後，您可以針對特定類別的會員採取行動（例如，「不太可能」註冊類別的每個會員），並特別鎖定他們以提高註冊人數。

![影像7](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-7.png)

>[!NOTE]
>
>個人可能性會考慮40個以上的人員因素，包括個人檔案屬性、人員活動，以及過去受邀／註冊／參加的活動。

## 常見問答集

**問：什麼是區段？**

答：註冊的可能值為0到100。 每個參與活動計畫的人都能獲得0到100之間的可能性值。

我們將似然值放入三個區段：

* 註冊的可能性>50% =高可能性區段
* 註冊的可能性>25%到&lt;50% =可能區段
* 註冊的可能性&lt;25% =可能性較低的區段

當某人有可能註冊時，預測會落入其中一個區段（每個參與計畫的人都會落入其中一個區段）。 例如，如果某個事件程式根據可能性預測有1000個成員，則這1000個成員會分發至「極可能 _」、「_&#x200B;可能 _」或「_&#x200B;較不可能 __ 」區段。

因此，「極可能性」區段的使用者註冊活動的機率較高。

轉換為註冊=區段中註冊的人數除以區段中的人數（例如，如果有100人進入「極可能」區段，而有60人註冊，則轉換率為60%）。

要註冊的轉換%將遵循以下模式：極有可能>可能>較不可能。

**問：我要如何運用見解？**

答：最佳做法包括：

i.您建立程式，然後智慧型促銷活動會使用「大於X」的預測性篩選器，這會導致特定人數（例如1000人），而您執行促銷活動。

ii. 在24小時後，您可 [!UICONTROL Reports] 以在標籤中看到根據註冊目前受邀人士的值的可能性而計算的預計註冊。

iii. 如果預計的註冊數低於目標，您必須邀請更多人。 目前，您可以看到這些洞見，告訴您過去的計畫有什麼成效。

![影像8](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-8.png)

iv. 您可以建立具有此臨界值的新智慧型促銷活動，以邀請更多人。

v.如果您想瞭解預測數目顯示的原因，您可以在任何時間點切換，以檢視跨區段的受眾分佈、過去的轉換率，並將這些轉換率套用至目前的受眾（請參閱下方的螢幕擷取）。

**問：什麼是「依註冊區分」圖表？**

答：三個橫條，每個橫條代表一個區段（極可能、極可能、極不可能）。

**紫色虛線：** 該區段中註冊的平均對話率（根據過去的類似方案）。

**藍條：** 該區段中所有人的註冊百分比。

![影像9](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-9.png)

例如，假設100人有可能註冊超過50%，而100人中有60人註冊。 極有可能轉換率為60%。 因此，加入程式的所有成員都可獲得註冊值的可能性，然後將它們放入區段中，並依每個區段轉換率中註冊的人數計算。

**問：「註冊及更高」是什麼意思？**

答：列為已註冊的人員，或具有等於或更高步驟編號的任何其他狀態。

您可以為事件程式建立新的晉升狀態，但我們會映射那些具有標準狀態的狀態。 請考慮某個人從被邀請到被提醒的情況，這比註冊要高。 此人也會被視為已註冊，並顯示在目標追蹤中。

![影像十](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-10.png)

**問：如何計算預計註冊？**

答：請參閱以下內容。

![影像十一](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-11.png)
