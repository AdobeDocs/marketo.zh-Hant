---
unique-page-id: 3571890
description: 啟用模型效能分析（潛在客戶）的自訂欄位群組 — Marketo檔案 — 產品檔案
title: 啟用模型效能分析（銷售機會）的自訂欄位群組
exl-id: 417fd74f-d8f5-477b-b633-0fdfdd68b22b
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# 啟用模型效能分析（銷售機會）的自訂欄位群組 {#enable-custom-field-groups-for-model-performance-analysis-leads}

>[!PREREQUISITES]
>
>透過Marketo中的「欄位管理器」，將標準或自訂欄位分類為群組以便報告。 如需詳細資訊，請參閱[透過欄位組織器建立自訂欄位群組](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/field-organizers/create-custom-field-groups-using-the-field-organizer.md)。

<table> 
 <tbody> 
  <tr> 
   <td colspan="3" rowspan="1"><p align="center"><strong>啟用自訂欄位群組如何影響Revenue Cycle Explorer中的多個分析區域？</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>當……發生什麼情況？</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>它如何影響<span class="uicontrol">模型效能分析（銷售機會）</span>區域</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>如何影響銷售機會分析、行銷活動分析和銷售機會分析領域</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>當您啟用與標準銷售機會或公司欄位相關聯的自訂欄位群組時，會發生什麼情況？</strong></p></td> 
   <td colspan="1" rowspan="1"><p>此自訂欄位群組已在<span class="uicontrol">模型效能分析（銷售機會）</span>區域中啟用報告</p></td> 
   <td colspan="1" rowspan="1"><p>沒有影響</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>當您啟用與自訂人員或公司欄位相關聯的自訂欄位群組時，會發生什麼情況？</strong></p></td> 
   <td colspan="1" rowspan="1"><p>此自訂欄位群組已在<span class="uicontrol">模型效能分析（銷售機會）</span>區域中啟用報告</p></td> 
   <td colspan="1" rowspan="1"><p>自訂欄位本身已針對潛在客戶分析、行銷活動分析和商機分析區域中的報告啟用。</p><p><strong>注意：</strong>這些分析區域不支援自訂欄位群組，所以群組關聯不會顯示在Revenue Cycle Explorer—<em>only</em>自訂欄位中。</p></td> 
  </tr> 
 </tbody> 
</table>

請依照下列步驟，在[!UICONTROL Model Performance Analysis (Leads)]區域中啟用報表的自訂欄位群組。

1. 按一下「**[!UICONTROL Admin]**」。

   ![](assets/one-1.png)

1. 按一下「**[!UICONTROL Revenue Cycle Analytics]**」。

   ![](assets/two-1.png)

1. 按一下空白欄位群組旁的&#x200B;**[!UICONTROL None]**。 如果您已啟用三個欄位群組並想要進行編輯，請按一下您要修改的欄位群組的名稱。

   ![](assets/three.png)

1. 按一下&#x200B;**[!UICONTROL Field]**&#x200B;下拉式清單，然後選取您要的專案。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >此範例為標準欄位（狀態）啟用自訂欄位群組。 因此，只有[!UICONTROL Model Performance Analysis (Leads)]區域受到影響。 如果已啟用自訂人員或公司欄位的自訂欄位群組，則啟用的群組將顯示在Sync Summary索引標籤的[!UICONTROL Model Performance Analysis (Leads)]區段中，而Lead、Campaign和Opportunity Analysis的自訂欄位計數將增加1。

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/five-1.png)
