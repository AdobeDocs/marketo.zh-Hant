---
description: Salesforce同步錯誤 — Marketo檔案 — 產品檔案
title: Salesforce同步錯誤
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 1%

---

# Salesforce同步錯誤 {#salesforce-sync-errors}

檢視同步處理期間遇到的錯誤摘要。 這包括同步處理不相容資料失敗所造成的錯誤。

>[!NOTE]
>
>**需要管理員許可權**

## 檢視同步處理錯誤 {#view-sync-errors}

1. 按一下 **[!UICONTROL 管理員]**.

   ![](assets/salesforce-sync-errors-1.png)

1. 在整合底下，按一下 **Salesforce**，然後 **[!UICONTROL 同步錯誤]** 標籤。

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>所列的錯誤範圍介於目前時間到目前同步之前5天。

| 欄位 | 說明 |
|---|---|
| 失敗於 | 記錄層級 _或_ 工作層級 |
| 失敗的日期/時間 | 錯誤詳細資料 |
| 錯誤型別 | SFDC傳回訊息 |

>[!TIP]
>
>按一下記錄層級記錄會顯示相關物件的Marketo和Salesforce ID。 在某些情況下，記錄上的訊息和工作層級錯誤是直接從Salesforce取得。 線上搜尋可能會提供其他詳細資料。

## 篩選器同步錯誤 {#filter-sync-errors}

1. 若要篩選資料，請按一下頁面最右側的篩選圖示。

   ![](assets/salesforce-sync-errors-3.png)

1. 選取您的日期與時間範圍，然後依「錯誤型別」（「工作層次」或「記錄層次」）進行篩選。 按一下 **[!UICONTROL 套用]** 完成時。

   ![](assets/salesforce-sync-errors-4.png)

**選擇性步驟**：若要匯出同步錯誤，請按一下 **[!UICONTROL 匯出]**. 資料將會匯出為CSV檔。

![](assets/salesforce-sync-errors-5.png)
