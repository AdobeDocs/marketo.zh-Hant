---
unique-page-id: 4719294
description: 自訂活動同步 — Marketo檔案 — 產品檔案
title: 自訂活動同步
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 自訂活動同步 {#customize-activities-sync}

如果您沒有使用Marketo Sales Insight,Marketo可以為某些事件建立Salesforce活動歷史記錄。 這是如何啟用它們。

1. 前往 **管理**.

   ![](assets/admin.png)

1. 按一下 **Salesforce**，然後按一下 **編輯同步選項**.

   ![](assets/two-1.png)

1. 勾選您要Marketo推送至Salesforce之活動旁的方塊，然後按一下 **儲存**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >啟用後，Marketo會推送三個月的活動記錄。 根據資料量， _可能需要數天才能完成_. 在初始活動推播期間發生的更新可能會延遲到初始活動同步完成之後。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>活動類型</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>填寫的表單</td> 
   <td>填寫任何Marketo表單</td> 
  </tr> 
  <tr> 
   <td>新增至清單</td> 
   <td><p>流量步驟：已新增至靜態清單</p></td> 
  </tr> 
  <tr> 
   <td>已傳送電子郵件</td> 
   <td>流量步驟：已傳送電子郵件</td> 
  </tr> 
  <tr> 
   <td>電子郵件傳送</td> 
   <td>收到電子郵件（未退信）</td> 
  </tr> 
  <tr> 
   <td>已開啟電子郵件</td> 
   <td>開啟電子郵件（不封鎖影像）</td> 
  </tr> 
  <tr> 
   <td>已點按電子郵件中的連結</td> 
   <td>按一下Marketo所傳送電子郵件中的連結</td> 
  </tr> 
  <tr> 
   <td>從清單中移除</td> 
   <td>流量步驟：已從靜態清單中移除</td> 
  </tr> 
  <tr> 
   <td>從流中刪除</td> 
   <td>流量步驟：從流中刪除</td> 
  </tr> 
  <tr> 
   <td>已發送銷售電子郵件</td> 
   <td>已透過Marketo Sales Insight傳送電子郵件</td> 
  </tr> 
  <tr> 
   <td>已開啟銷售電子郵件</td> 
   <td>開啟透過Marketo Sales Insight傳送的電子郵件</td> 
  </tr> 
  <tr> 
   <td>按一下銷售電子郵件中的連結</td> 
   <td>按一下透過Marketo Sales Insight傳送之電子郵件中的連結</td> 
  </tr> 
  <tr> 
   <td>收到銷售電子郵件</td> 
   <td>銷售代表在MSI Outlook插件中收到並記錄了電子郵件</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>「收到銷售電子郵件」 **not** 平均傳遞。 不會針對透過Sales Insight傳送的電子郵件擷取傳送狀態。

>[!TIP]
>
>如果您想要將更多Marketo資訊帶入Salesforce，請查看我們的 [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) 產品。
