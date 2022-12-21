---
description: Salesforce同步錯誤 — Marketo檔案 — 產品檔案
title: Salesforce同步錯誤
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 1%

---

# Salesforce同步錯誤 {#salesforce-sync-errors}

查看同步過程中遇到的錯誤的摘要。 這包括因同步不相容資料失敗而導致的錯誤。

>[!NOTE]
>
>**需要管理權限**

## 查看同步錯誤 {#view-sync-errors}

1. 按一下 **管理**.

   ![](assets/salesforce-sync-errors-1.png)

1. 在整合下方，按一下 **Salesforce**，則 **同步錯誤** 標籤。

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>列出的錯誤範圍從當前時間到當前同步前的5天。

| 欄位 | 說明 |
|---|---|
| 失敗於 | 記錄級別 _或_ 作業層級 |
| 失敗日期/時間 | 錯誤詳細資訊 |
| 錯誤類型 | SFDC返回消息 |

>[!TIP]
>
>按一下記錄層級記錄，會顯示相關物件的Marketo和Salesforce ID。 在某些情況下，記錄和作業層級錯誤上的訊息會直接來自Salesforce。 線上搜索可能提供更多細節。

## 篩選同步錯誤 {#filter-sync-errors}

1. 若要篩選資料，請按一下頁面最右側的篩選圖示。

   ![](assets/salesforce-sync-errors-3.png)

1. 選擇日期和時間範圍，然後按錯誤類型（任務層或記錄層）篩選。 按一下 **套用** 時才能使用。

   ![](assets/salesforce-sync-errors-4.png)

**可選步驟**:要導出同步錯誤，請按一下 **匯出**. 資料將匯出為CSV。

![](assets/salesforce-sync-errors-5.png)
