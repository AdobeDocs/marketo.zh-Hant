---
unique-page-id: 4719294
description: 自訂活動同步-Marketo文檔——產品文檔
title: 自訂活動同步
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 自訂活動同步{#customize-activities-sync}

如果您不使用「Marketo銷售分析」,Marketo可以為某些事件建立「Salesforce活動歷史記錄」。 以下是如何啟用它們。

1. 前往&#x200B;**Admin**。

   ![](assets/admin.png)

1. 按一下「**Salesforce**」，然後按一下「編輯同步選項&#x200B;**」。**

   ![](assets/two-1.png)

1. 勾選您要Marketo推送至Salesforce之活動旁的方塊，然後按一下「儲存」。****

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >一旦啟用，Marketo將推出3個月的活動歷史。 根據資料量，_完成_&#x200B;可能需要數天。 在初始「活動」推播期間發生的更新可能會延遲到初始「活動」同步完成後。

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
   <td>填寫表格</td> 
   <td>填寫任何Marketo表格</td> 
  </tr> 
  <tr> 
   <td>新增至清單</td> 
   <td><p>流程步驟：已新增至靜態清單</p></td> 
  </tr> 
  <tr> 
   <td>電子郵件已傳送</td> 
   <td>流程步驟：已傳送電子郵件</td> 
  </tr> 
  <tr> 
   <td>電子郵件傳送</td> 
   <td>已收到電子郵件（未反彈）</td> 
  </tr> 
  <tr> 
   <td>已開啟電子郵件</td> 
   <td>開啟電子郵件（不封鎖影像）</td> 
  </tr> 
  <tr> 
   <td>已點按電子郵件中的連結</td> 
   <td>按一下Marketo寄送之電子郵件中的連結</td> 
  </tr> 
  <tr> 
   <td>已從清單中移除</td> 
   <td>流程步驟：已從靜態清單中移除</td> 
  </tr> 
  <tr> 
   <td>從流中移除</td> 
   <td>流程步驟：從流中移除</td> 
  </tr> 
  <tr> 
   <td>銷售電子郵件已傳送</td> 
   <td>是透過Marketo銷售分析寄送電子郵件</td> 
  </tr> 
  <tr> 
   <td>已開啟銷售電子郵件</td> 
   <td>開啟透過Marketo銷售分析傳送的電子郵件</td> 
  </tr> 
  <tr> 
   <td>按一下銷售電子郵件中的連結</td> 
   <td>按一下透過Marketo銷售分析所傳送之電子郵件中的連結</td> 
  </tr> 
  <tr> 
   <td>收到銷售電子郵件</td> 
   <td>銷售代表在MSI Outlook外掛程式中收到並記錄電子郵件</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>「收到銷售電子郵件」**not**&#x200B;表示已送達。 透過Sales Insight傳送的電子郵件不會擷取傳送狀態。

>[!TIP]
>
>如果您想要將更多Marketo資訊匯入Salesforce，請查看我們的[Marketo銷售分析](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)產品。
