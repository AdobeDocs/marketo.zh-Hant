---
unique-page-id: 2951220
description: 使用行動平台欄建立人員效能報表 — Marketo檔案 — 產品檔案
title: 使用行動平台欄建立人員效能報表
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 使用行動平台欄建立人員效能報表 {#build-a-people-performance-report-with-mobile-platform-columns}

請依照下列步驟，使用行動平台(iOS/Android)建立「人員效能報表」欄。

## 建立行動智慧清單 {#create-mobile-smart-lists}

1. 前往 **行銷活動**.

   ![](assets/ma.png)

1. 選擇方案。

   ![](assets/two-1.png)

1. 在 **新增**，選取 **新本機資產**.

   ![](assets/three-1.png)

1. 按一下 **智慧清單**.

   ![](assets/four-1.png)

1. 輸入名稱，然後按一下 **建立**.

   ![](assets/five-1.png)

1. 尋找「已開啟的電子郵件」篩選器並拖曳至畫布中。

   ![](assets/six-1.png)

1. 將電子郵件設定為 **是**.

   ![](assets/seven.png)

1. 按一下 **添加約束** 選取 **平台**.

   ![](assets/eight.png)

   >[!TIP]
   >
   >在此範例中，我們使用「已開啟的電子郵件」篩選器。 您也可以使用「已點按電子郵件」篩選器，因為篩選器具有Platform限制。

1. 將平台設定為 **iOS**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >至少必須有一人已在iOS裝置上開啟您的其中一封電子郵件，Marketo才會自動建議您找到。 如果畫面未顯示，您可以手動輸入並儲存。

   現在為「Android」平台建立第二個智慧清單。 完成後，請移至下一節。

## 建立人員績效報表 {#create-a-people-performance-report}

1. 在「行銷活動」下方，選取容納您的 **iOS** 和 **Android** 智慧清單。

   ![](assets/ten.png)

1. 在 **新增**，選取 **新本機資產**.

   ![](assets/eleven.png)

1. 按一下 **報表**.

   ![](assets/twelve.png)

1. 將類型設定為 **人員績效**.

   ![](assets/thirteen.png)

1. 按一下 **建立**。

   ![](assets/fourteen.png)

   你做得很好！ 接下來的部分。

## 將行動智慧清單新增為欄 {#add-mobile-smart-lists-as-columns}

1. 在您剛建立的報表中，按一下 **設定**，然後拖曳 **自訂欄** 進入畫布。

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >依預設，「人員績效」報表會查看最近7天。 按兩下可以變更時間範圍。

1. 查找並選擇您先前建立的智慧清單，然後按一下 **套用**.

   ![](assets/sixteen.png)

1. 按一下 **報表** 執行報表並查看資料。

   ![](assets/seventeen.png)

   挺酷的，對吧？ 幹得好！
