---
description: 取消訂閱概述 — Marketo文檔 — 產品文檔
title: 取消訂閱概述
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 取消訂閱概述 {#unsubscribe-overview}

對於公司來說，遵守電子郵件隱私法變得越來越重要。 為了幫助解決此問題，我們對取消訂閱體驗進行了一些增強。

* 取消訂閱連結會放在從MarketoSales and Salesforce發送的所有電子郵件上（這不適用於從Outlook或Gmail發送的自定義電子郵件）
* 管理員可以編輯其整個團隊的取消訂閱消息
* 取消訂閱資訊儲存在PDV中
* 可以手動執行取消訂閱：已按一下連結、Salesforce同步和彈出
* 新建取消訂閱連結登錄頁

## 取消訂閱連結登錄頁 {#unsubscribe-link-landing-page}

當某人按一下您的取消訂閱連結時，他們將被帶到取消訂閱登錄頁，在該登錄頁中，他們可以選擇要取消訂閱的內容以及原因。

![](assets/unsubscribe-overview-1.png)

此資訊將保存到人員詳細資訊視圖，以供以後查看。

## 取消訂閱組 {#unsubscribe-group}

在一個位置查看和管理所有未訂閱的人員。

![](assets/unsubscribe-overview-2.png)

使用搜索欄查找任何未訂閱的人員。

![](assets/unsubscribe-overview-3.png)

如果您是管理員，您可以轉到取消訂閱組按帳戶取消訂閱進行篩選，並查看在您的人員資料庫中收集的所有取消訂閱。

![](assets/unsubscribe-overview-4.png)

## 取消訂閱歷史記錄卡 {#unsubscribe-history-card}

取消訂閱歷史記錄卡可幫助管理員和用戶獲取有關其聯繫人取消訂閱歷史記錄的上下文資訊。 轉到「人員」頁籤並選擇人員，在該位置導航。 它位於「人員詳細資訊」視圖的「關於」頁籤的底部。

>[!NOTE]
>
>只有當用戶具有 _已訂閱_ 在某個時候。

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
   <td><strong>詳細資訊</strong></td> 
   <td><p>重新訂閱：Sales Connect管理員手動從聯繫人記錄中刪除了取消訂閱。 它還可能顯示一些與聯繫人取消訂閱原因有關的詳細資訊。</p><p>取消訂閱：聯繫人已取消訂閱。</p></td> 
  </tr> 
  <tr> 
   <td><strong>來源</strong></td> 
   <td><p>Salesforce同步：Salesforce的同步捕獲了取消訂閱。</p><p>手動：用戶按一下取消訂閱按鈕以選擇退出。</p><p>已按一下連結：電子郵件的收件人已按一下取消訂閱連結。</p><p>"管理員名稱":管理員的名稱將顯示何時重新訂閱聯繫人的操作。 這樣，用戶就能知道誰刪除了取消訂閱。</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[自定義取消訂閱連結消息](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
