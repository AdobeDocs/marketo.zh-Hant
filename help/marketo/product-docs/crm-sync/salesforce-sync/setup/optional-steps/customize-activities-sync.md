---
unique-page-id: 4719294
description: 自訂活動同步 — Marketo檔案 — 產品檔案
title: 自訂活動同步
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 6293a11b9d48a20da4cb2448c8374c469679abdb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 2%

---

# 自訂活動同步 {#customize-activities-sync}

如果您沒有使用Marketo Sales Insight，Marketo Engage可以為某些事件建立Salesforce活動歷程記錄。 以下說明啟用方法。

>[!NOTE]
>
>Salesforce/Marketo Engage同步不會將任何人推送至Salesforce前發生的任何活動推送至Salesforce。

1. 移至&#x200B;**[!UICONTROL Admin]**。

   ![](assets/customize-activities-sync-1.png)

1. 按一下「**[!DNL Salesforce]**」，然後按一下「**[!UICONTROL Edit Sync Options]**」。

   ![](assets/two-1.png)

1. 勾選您要Marketo推送至Salesforce的活動旁的方塊，然後按一下「**[!UICONTROL Save]**」。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >啟用後，Marketo會推送三個月的活動歷史記錄。 根據資料量，_這可能需要數天才能完成_。 在初始活動推送期間發生的更新可能會延遲到初始活動同步完成後。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>活動型別</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>已填寫表單</td> 
   <td>填寫任何Marketo表單</td> 
  </tr> 
  <tr> 
   <td>已新增至清單</td> 
   <td><p>流程步驟：已新增至靜態清單</p></td> 
  </tr> 
  <tr> 
   <td>電子郵件已傳送</td> 
   <td>流程步驟：已傳送電子郵件</td> 
  </tr> 
  <tr> 
   <td>電子郵件已傳遞</td> 
   <td>已收到電子郵件（未退回）</td> 
  </tr> 
  <tr> 
   <td>電子郵件已開啟</td> 
   <td>已開啟電子郵件（未封鎖影像）</td> 
  </tr> 
  <tr> 
   <td>電子郵件中的點選連結</td> 
   <td>按一下Marketo所傳送電子郵件中的連結</td> 
  </tr> 
  <tr> 
   <td>已從清單中移除</td> 
   <td>流程步驟：已從靜態清單中移除</td> 
  </tr> 
  <tr> 
   <td>從流程移除</td> 
   <td>流程步驟：從流程中移除</td> 
  </tr> 
  <tr> 
   <td>已傳送銷售電子郵件</td> 
   <td>已透過Marketo Sales Insight傳送電子郵件</td> 
  </tr> 
  <tr> 
   <td>已開啟銷售電子郵件</td> 
   <td>已開啟透過Marketo Sales Insight傳送的電子郵件</td> 
  </tr> 
  <tr> 
   <td>按一下銷售電子郵件中的連結</td> 
   <td>按一下透過Marketo Sales Insight傳送的電子郵件中的連結</td> 
  </tr> 
  <tr> 
   <td>已收到銷售電子郵件</td> 
   <td>MSI Outlook外掛程式中的銷售代表已收到並記錄電子郵件</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>「已收到銷售電子郵件」的&#x200B;_不是_&#x200B;表示已傳遞。 對於透過Sales Insight傳送的電子郵件，不會擷取傳遞狀態。

>[!TIP]
>
>如果您有興趣在Salesforce中取得更多Marketo資訊，請參閱我們的[Marketo銷售Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}產品。
