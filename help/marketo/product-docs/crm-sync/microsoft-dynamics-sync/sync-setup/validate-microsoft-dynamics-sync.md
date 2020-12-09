---
unique-page-id: 8783322
description: 驗證Microsoft Dynamics Sync —— 行銷檔案——產品檔案
title: 驗證Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# 驗證Microsoft Dynamics Sync {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>如果您的Dynamics Sync已啟用多因素驗證(MFA)，則必須停用它，Dynamics才能與Marketo正確同步。 如需詳細資訊，請聯絡 [行銷支援](http://nation.marketo.com/community/support_solutions)。

## 在Marketo中執行驗證同步 {#run-validate-sync-in-marketo}

請務必執行「驗證同步」工具，以確保您的Microsoft Dynamics Sync with Marketo已正確設定，然後再進行最終連線。 此程式會產生七個設定步驟的檢查清單，以找出問題所在。 驗證這些動作是否正確可節省許多時間。

1. 按一下「 **管理** 」標籤，然後在「整 **合」區域中按一下「Microsoft Dynamics** 」連結。

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. 選擇 **Microsoft**。

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. 按一下「驗 **證同步設定** 」頁籤。

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. 輸入您的使用者名稱、密碼和URL（用戶端ID和用戶端密碼為選用）。 完成時 **按一下** 「下一步」。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >如果您之前已同步，左 **樹狀結構中的CRM** 將會讀取 **Microsoft Dynamics**，而上表格中的資料可能已預先填入。

1. 如果一切正常，驗證同步將生成一個充滿綠色複選標籤的檢 ![查表](assets/check.png)。

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. 如果您看到…… ![](assets/delete.png)，則該步驟會出現問題。 請參 [閱修正動態驗證同步問題](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) ，以識別並修正問題。 然後重新執行同步驗證步驟，直到結果看起來與上述影像相同。

   >[!CAUTION]
   >
   >我們目前不支援Marketo Dynamics Sync的沙盒重新整理。 如果您需要重新整理Dynamics CRM沙盒，將需要新的Marketo沙盒。 如需詳細資訊，請連絡您的客戶成功經理。

>[!MORELIKETHIS]
>
>[修正動態驗證同步問題](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)

