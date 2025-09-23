---
unique-page-id: 2951220
description: 使用Mobile Platform欄建立人員績效報表 — Marketo檔案 — 產品檔案
title: 使用行動平台欄建置人員績效報告
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 8%

---

# 使用行動平台欄建置人員績效報告 {#build-a-people-performance-report-with-mobile-platform-columns}

請依照下列步驟，使用Mobile Platform (iOS/Android)欄建立人員績效報表。

## 建立行動裝置智慧清單 {#create-mobile-smart-lists}

1. 移至&#x200B;**[!UICONTROL Marketing Activities]**。

   ![](assets/ma.png)

1. 選擇程式。

   ![](assets/two-1.png)

1. 在&#x200B;**[!UICONTROL New]**&#x200B;下，選取&#x200B;**[!UICONTROL New Local Asset]**。

   ![](assets/three-1.png)

1. 按一下「**[!UICONTROL Smart List]**」。

   ![](assets/four-1.png)

1. 輸入名稱並按一下&#x200B;**[!UICONTROL Create]**。

   ![](assets/five-1.png)

1. 尋找[!UICONTROL Opened Email]篩選器並拖曳到畫布中。

   ![](assets/six-1.png)

1. 將電子郵件設定為&#x200B;**[!UICONTROL is any]**。

   ![](assets/seven.png)

1. 按一下&#x200B;**[!UICONTROL Add Constraint]**&#x200B;並選取&#x200B;**[!UICONTROL Platform]**。

   ![](assets/eight.png)

   >[!TIP]
   >
   >在此範例中，我們使用了[!UICONTROL Opened Email]篩選器。 您也可以使用[!UICONTROL Clicked Email]篩選器，因為它具有Platform條件約束。

1. 將[!UICONTROL Platform]設為&#x200B;**[!UICONTROL iOS]**。

   ![](assets/nine.png)

   >[!NOTE]
   >
   >必須至少有一個人在iOS裝置上開啟了您的其中一個電子郵件，Marketo的自動建議才能找到它。 如果未顯示，您可以手動輸入並儲存。

   現在為「Android」平台建立第二個智慧清單。 完成後，移至下一個區段。

## 建立人員績效報表 {#create-a-people-performance-report}

1. 在行銷活動底下，選取容納您&#x200B;**[!UICONTROL iOS]**&#x200B;和&#x200B;**[!UICONTROL Android]**&#x200B;智慧清單的方案。

   ![](assets/ten.png)

1. 在&#x200B;**[!UICONTROL New]**&#x200B;下，選取&#x200B;**[!UICONTROL New Local Asset]**。

   ![](assets/eleven.png)

1. 按一下「**[!UICONTROL Report]**」。

   ![](assets/twelve.png)

1. 設定型別為&#x200B;**[!UICONTROL People Performance]**。

   ![](assets/thirteen.png)

1. 按一下「**[!UICONTROL Create]**」。

   ![](assets/fourteen.png)

   您做得很好！ 現在來看看下一節。

## 將行動智慧列示新增為欄 {#add-mobile-smart-lists-as-columns}

1. 在您剛建立的報表中，按一下&#x200B;**[!UICONTROL Setup]**，然後將&#x200B;**[!UICONTROL Custom Columns]**&#x200B;拖曳至畫布。

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >依預設，「人員效能」報表會檢視過去7天。 您可以按兩下時間範圍以變更時間範圍。

1. 尋找並選取您先前建立的智慧列示，然後按一下&#x200B;**[!UICONTROL Apply]**。

   ![](assets/sixteen.png)

1. 按一下&#x200B;**[!UICONTROL Report]**&#x200B;以執行報告並檢視您的資料。

   ![](assets/seventeen.png)

   很酷吧？ 做得很好！
