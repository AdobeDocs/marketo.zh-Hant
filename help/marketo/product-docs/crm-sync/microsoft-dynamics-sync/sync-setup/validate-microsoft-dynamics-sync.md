---
unique-page-id: 8783322
description: 驗證 [!DNL Microsoft Dynamics] 同步 — Marketo檔案 — 產品檔案
title: 驗證 [!DNL Microsoft Dynamics] 同步
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# 驗證[!DNL Microsoft Dynamics]同步 {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>如果您為[!DNL Dynamics]同步處理啟用多重驗證(MFA)，您必須停用它才能讓[!DNL Dynamics]與Marketo正確同步。 如需其他資訊，請連絡[Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support)。

## 在Marketo中執行驗證同步 {#run-validate-sync-in-marketo}

執行「驗證同步」工具非常重要，以確定您與Marketo的[!DNL Microsoft Dynamics]同步已正確設定，然後再建立兩者之間的最終連線。 此程式會產生包含七個設定步驟的核對清單，以找出問題的所在。 確認這些操作正確無誤，可節省大量之後的時間。

1. 按一下「**[!UICONTROL Admin]**」標籤，然後按一下「整合」區域中的&#x200B;**[!DNL Microsoft Dynamics]**&#x200B;連結。

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. 選擇「**[!DNL Microsoft]**」。

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. 按一下「**[!UICONTROL Validate Sync Setup]**」標籤。

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. 輸入您的使用者名稱、密碼和URL （使用者端ID和使用者端密碼為選用）。 完成時，按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >如果您之前已同步處理，則左側樹狀結構中的&#x200B;**CRM**&#x200B;將會讀取&#x200B;**[!DNL Microsoft Dynamics]**，而且可能會預先填入上述表單中的資料。

1. 如果一切正常，驗證同步處理會產生一個包含綠色核取記號![—](assets/check.png)的核取清單。

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. 如果您看到![—](assets/delete.png)，則表示該步驟有問題。 請參閱[修正 [!DNL Dynamics] 驗證同步問題](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)以識別並修正問題。 然後重新執行同步驗證步驟，直到結果如上圖所示。

   >[!CAUTION]
   >
   >我們目前不支援[!DNL Marketo Dynamics]同步處理的沙箱重新整理。 如果您需要重新整理[!DNL Dynamics] CRM沙箱，則需要新的Marketo沙箱。 請聯絡您的客戶成功案例經理，以瞭解更多詳細資訊。

>[!MORELIKETHIS]
>
>[修正 [!DNL Dynamics] 驗證同步處理問題](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
