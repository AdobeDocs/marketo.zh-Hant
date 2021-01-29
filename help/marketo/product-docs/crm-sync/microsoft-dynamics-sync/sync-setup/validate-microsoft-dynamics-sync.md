---
unique-page-id: 8783322
description: 驗證Microsoft Dynamics Sync —— 行銷檔案——產品檔案
title: 驗證Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: 20d4c8a079916f47267df3dab5a8e663f6eb019b
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# 驗證Microsoft Dynamics Sync {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>如果您的Dynamics Sync已啟用多因素驗證(MFA)，則必須停用它，Dynamics才能與Marketo正確同步。 如需詳細資訊，請聯絡[行銷支援](https://nation.marketo.com/t5/Support/ct-p/Support)。

## 在Marketo {#run-validate-sync-in-marketo}中執行驗證同步

請務必執行「驗證同步」工具，以確保您的Microsoft Dynamics Sync with Marketo已正確設定，然後再進行最終連線。 此程式會產生七個設定步驟的檢查清單，以找出問題所在。 驗證這些動作是否正確可節省許多時間。

1. 按一下「整合」區域中的&#x200B;**Admin**&#x200B;標籤和&#x200B;**Microsoft Dynamics**&#x200B;連結。

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. 選擇&#x200B;**Microsoft**。

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. 按一下&#x200B;**驗證同步設定**&#x200B;頁籤。

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. 輸入您的使用者名稱、密碼和URL（用戶端ID和用戶端密碼為選用）。 完成時，按一下「下一步」。****

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >如果您之前已同步，左側樹狀結構中的&#x200B;**CRM**&#x200B;將會讀取&#x200B;**Microsoft Dynamics**，且上表格的資料可能已預先填入。

1. 如果一切正常，驗證同步將生成一個包含綠色複選標籤![—](assets/check.png)的檢查清單。

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. 如果您看到![—](assets/delete.png)，則該步驟會發生問題。 請參閱[修正動態驗證同步問題](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)以識別並修正問題。 然後重新執行同步驗證步驟，直到結果看起來與上述影像相同。

   >[!CAUTION]
   >
   >我們目前不支援Marketo Dynamics Sync的沙盒重新整理。 如果您需要重新整理Dynamics CRM沙盒，將需要新的Marketo沙盒。 如需詳細資訊，請連絡您的客戶成功經理。

>[!MORELIKETHIS]
>
>[修正動態驗證同步問題](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
