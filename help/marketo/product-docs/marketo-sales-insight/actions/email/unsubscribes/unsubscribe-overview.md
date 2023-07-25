---
description: 取消訂閱概述 — Marketo檔案 — 產品檔案
title: 取消訂閱概述
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 取消訂閱概述 {#unsubscribe-overview}

組織遵守電子郵件隱私權法規變得越來越重要。 為了協助解決此問題，我們對取消訂閱體驗進行了一些增強。

* 從Marketo Sales和Salesforce傳送的所有電子郵件都會顯示取消訂閱連結（這不適用於從Outlook或Gmail傳送的自訂電子郵件）
* 管理員可以編輯整個團隊的取消訂閱訊息
* 取消訂閱資訊會儲存在PDV中
* 取消訂閱可以手動完成：點選連結、Salesforce同步和彈回
* 新的取消訂閱連結登陸頁面

## 取消訂閱連結登陸頁面 {#unsubscribe-link-landing-page}

當有人按一下您的取消訂閱連結時，系統將帶他們至取消訂閱登陸頁面，他們可在其中選擇想要取消訂閱的專案及原因。

![](assets/unsubscribe-overview-1.png)

此資訊將儲存至人員詳細資料檢視，以供稍後檢視。

## 取消訂閱群組 {#unsubscribe-group}

在一個位置檢視和管理所有已取消訂閱的人。

![](assets/unsubscribe-overview-2.png)

使用搜尋列來查詢任何已取消訂閱的人。

![](assets/unsubscribe-overview-3.png)

如果您是管理員，可以移至「取消訂閱」群組，依「帳戶取消訂閱」進行篩選，並檢視已在您的人員資料庫中收集的所有取消訂閱。

![](assets/unsubscribe-overview-4.png)

## 取消訂閱歷程記錄卡 {#unsubscribe-history-card}

「取消訂閱歷程記錄」卡片可協助管理員和使用者取得有關其連絡人取消訂閱歷程記錄的內容資訊。 前往「人員」標籤並選取人員，以導覽至該處。 它位於「人員詳細資訊」檢視中的「關於」標籤底部。

>[!NOTE]
>
>只有在以下情況下，才會有「取消訂閱歷程記錄」卡： _已重新訂閱_ 在某些時候。

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>日期</strong></td> 
   <td><p>顯示取消訂閱/重新訂閱發生的日期。</p></td> 
  </tr> 
  <tr> 
   <td><strong>詳細資料</strong></td> 
   <td><p>重新訂閱： Sales Connect管理員已手動從連絡人記錄中移除取消訂閱。 它也可能顯示與聯絡人取消訂閱原因相關的一些細節。</p><p>取消訂閱：連絡人已取消訂閱。</p></td> 
  </tr> 
  <tr> 
   <td><strong>來源</strong></td> 
   <td><p>Salesforce同步：同步處理從Salesforce擷取取消訂閱。</p><p>手動：使用者按一下取消訂閱按鈕以選擇退出。</p><p>點按連結：電子郵件的收件者點按了取消訂閱連結。</p><p>「管理員名稱」：當動作要重新訂閱連絡人時，將顯示管理員名稱。 這可讓使用者知道誰移除取消訂閱。</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[自訂取消訂閱連結訊息](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
