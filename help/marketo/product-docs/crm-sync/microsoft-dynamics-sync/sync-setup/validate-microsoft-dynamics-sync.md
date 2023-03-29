---
unique-page-id: 8783322
description: 驗證Microsoft Dynamics同步 — Marketo檔案 — 產品檔案
title: 驗證Microsoft Dynamics同步
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 驗證Microsoft Dynamics同步 {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>如果已為Dynamics同步啟用了多重身份驗證(MFA)，則必須禁用它，以便Dynamics與Marketo正確同步。 欲知更多資訊，請聯繫 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support).

## 在Marketo中執行驗證同步 {#run-validate-sync-in-marketo}

請務必執行驗證同步工具，以在兩者之間建立最終連線之前，確定您的Microsoft Dynamics與Marketo同步已正確設定。 此程式會產生七個設定步驟的檢查清單，以找出問題所在。 驗證是否正確可以節省大量時間。

1. 按一下 **管理** 標籤 **Microsoft Dynamics** 連結。

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. 選擇 **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. 按一下 **驗證同步設定** 標籤。

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. 輸入您的使用者名稱、密碼和URL（用戶端ID和用戶端密碼為選用）。 按一下 **下一個** 時才能使用。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >如果你之前同步過， **CRM** 在左樹中， **Microsoft Dynamics**，且可預先填入上述表單中的資料。

1. 如果一切正常，驗證同步會產生一個充滿綠色勾號的檢查清單 ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. 如果您看到 ![—](assets/delete.png)，則該步驟會有問題。 請參閱 [修正Dynamics驗證同步問題](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) 來識別並解決問題。 然後重新執行同步驗證步驟，直到結果看起來像上圖。

   >[!CAUTION]
   >
   >我們目前不支援Marketo Dynamics Sync的沙箱重新整理。 如果您需要重新整理Dynamics CRM沙箱，則需要新的Marketo沙箱。 如需詳細資訊，請連絡Adobe客戶團隊（您的客戶經理）。

>[!MORELIKETHIS]
>
>[修正Dynamics驗證同步問題](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
