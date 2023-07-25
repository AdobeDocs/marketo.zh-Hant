---
unique-page-id: 4719294
description: 自訂活動同步 — Marketo檔案 — 產品檔案
title: 自訂活動同步
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 自訂活動同步 {#customize-activities-sync}

如果您沒有使用Marketo Sales Insight，Marketo可以為某些事件建立Salesforce活動歷程記錄。 以下說明啟用方法。

1. 前往 **管理員**.

   ![](assets/admin.png)

1. 按一下 **Salesforce**，然後按一下 **編輯同步選項**.

   ![](assets/two-1.png)

1. 勾選您要Marketo推送至Salesforce的活動旁的方塊，然後按一下 **儲存**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >啟用後，Marketo會推送三個月的活動歷史記錄。 根據資料量， _這可能需要幾天的時間才能完成_. 在初始活動推送期間發生的更新可能會延遲到初始活動同步完成後。

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
   <td>已點按電子郵件中的連結</td> 
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
   <td>銷售電子郵件已傳送</td> 
   <td>已透過Marketo Sales Insight傳送電子郵件</td> 
  </tr> 
  <tr> 
   <td>已開啟銷售電子郵件</td> 
   <td>已開啟透過Marketo Sales Insight傳送的電子郵件</td> 
  </tr> 
  <tr> 
   <td>按一下銷售電子郵件中的連結</td> 
   <td>按一下透過Marketo Sales Insight傳送之電子郵件中的連結</td> 
  </tr> 
  <tr> 
   <td>已收到銷售電子郵件</td> 
   <td>MSI Outlook外掛程式中的銷售代表已收到並記錄電子郵件</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>「已收到的銷售電子郵件」會 **not** 平均已傳遞。 透過Sales Insight傳送的電子郵件不會擷取傳遞狀態。

>[!TIP]
>
>如果您有興趣將更多Marketo資訊帶入Salesforce，請檢視我們的 [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) 產品。
