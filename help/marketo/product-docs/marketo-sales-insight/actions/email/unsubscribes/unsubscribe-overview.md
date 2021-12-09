---
description: 取消訂閱概述 — Marketo檔案 — 產品檔案
title: 取消訂閱概述
hide: true
hidefromtoc: true
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 取消訂閱概述 {#unsubscribe-overview}

對於組織來說，遵守電子郵件隱私法變得越來越重要。 為了提供這些協助，我們已對取消訂閱的體驗進行了一些增強功能。

* 從Marketo Sales和Salesforce傳送的所有電子郵件都會放置取消訂閱連結（這不適用於從Outlook或Gmail傳送的自訂電子郵件）
* 管理員可以編輯其整個團隊的取消訂閱訊息
* 取消訂閱資訊儲存在PDV中
* 取消訂閱可手動完成：按一下連結、Salesforce同步和跳出
* 新的取消訂閱連結登陸頁面

## 取消訂閱連結登陸頁面 {#unsubscribe-link-landing-page}

當使用者按一下您的取消訂閱連結時，將會帶他們進入取消訂閱的登陸頁面，讓他們可以選取想要取消訂閱的項目及其原因。

![](assets/unsubscribe-overview-1.png)

此資訊將保存到人員詳細資訊視圖，以供稍後查看。

## 取消訂閱組 {#unsubscribe-group}

在一個位置查看和管理所有未訂閱的人員。

![](assets/unsubscribe-overview-2.png)

使用搜尋列來查詢任何未訂閱的訪客。

![](assets/unsubscribe-overview-3.png)

如果您是管理員，可以前往「取消訂閱」群組，依「帳戶取消訂閱」來篩選，並查看人員資料庫中收集的所有取消訂閱。

![](assets/unsubscribe-overview-4.png)

## 取消訂閱歷史記錄卡 {#unsubscribe-history-card}

「取消訂閱歷史記錄」卡可協助管理員和使用者取得其聯絡人取消訂閱歷史記錄的相關內容資訊。 前往「人員」標籤並選取人員，即可導覽至該處。 它位於「人員詳細資訊」視圖中「關於」頁簽的底部。

>[!NOTE]
>
>只有當人員擁有 _重新訂閱_ 在某個時候。

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>日期</strong></td> 
   <td><p>顯示取消訂閱/重新訂閱的發生日期。</p></td> 
  </tr> 
  <tr> 
   <td><strong>詳細資料</strong></td> 
   <td><p>重新訂閱：Sales Connect管理員從聯繫記錄中手動刪除取消訂閱。 它也可能顯示與取消訂閱聯繫人原因相關的一些詳細資訊。</p><p>取消訂閱：該聯繫人已取消訂閱。</p></td> 
  </tr> 
  <tr> 
   <td><strong>來源</strong></td> 
   <td><p>Salesforce同步：取消訂閱是由Salesforce的同步捕獲的。</p><p>手動：使用者按一下取消訂閱按鈕以選擇退出。</p><p>已點按連結：電子郵件的收件者按一下取消訂閱連結。</p><p>"管理員名稱":管理員的名稱會顯示動作要重新訂閱連絡人的時間。 這可讓使用者知道誰移除了取消訂閱。</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[自訂取消訂閱連結訊息](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
