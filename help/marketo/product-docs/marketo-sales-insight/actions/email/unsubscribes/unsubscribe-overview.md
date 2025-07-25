---
description: 取消訂閱概述 — Marketo檔案 — 產品檔案
title: 取消訂閱總覽
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# 取消訂閱總覽 {#unsubscribe-overview}

遵守電子郵件隱私權法規對組織而言越來越重要。 為了協助解決此問題，我們對取消訂閱體驗進行了一些增強功能。

* 從[!DNL Marketo Sales]和[!DNL Salesforce]傳送的所有電子郵件都會放置取消訂閱連結（這不適用於從[!DNL Outlook]或Gmail傳送的自訂電子郵件）
* 管理員可以編輯整個團隊的取消訂閱訊息
* 取消訂閱資訊儲存在PDV中
* 取消訂閱可以手動完成：點選連結、[!DNL Salesforce]同步和退回
* 新的取消訂閱連結登陸頁面

## 取消訂閱連結登陸頁面 {#unsubscribe-link-landing-page}

當人員按一下您的取消訂閱連結時，系統將帶他們至取消訂閱登陸頁面，在此頁面中他們可選擇要取消訂閱的專案及原因。

![](assets/unsubscribe-overview-1.png)

此資訊將儲存到人員詳細資料檢視以供稍後檢視。

## 取消訂閱群組 {#unsubscribe-group}

在一個位置檢視和管理所有已取消訂閱的朋友。

![](assets/unsubscribe-overview-2.png)

使用搜尋列來查詢任何已取消訂閱的人員。

![](assets/unsubscribe-overview-3.png)

如果您是管理員，您可以移至取消訂閱群組來依[!UICONTROL Account Unsubscribes]篩選，並檢視已在您的人員資料庫中收集的所有取消訂閱。

![](assets/unsubscribe-overview-4.png)

## 取消訂閱歷程記錄卡 {#unsubscribe-history-card}

[!UICONTROL Unsubscribe History]卡片可協助管理員和使用者取得有關其連絡人取消訂閱歷程記錄的內容資訊。 前往「[!UICONTROL People]」標籤並選取人員，以導覽至該處。 它位於人員詳細資料檢視中[!UICONTROL About]索引標籤的底部。

>[!NOTE]
>
>如果人員有[!UICONTROL Unsubscribe History]重新訂閱&#x200B;_，則只會有_&#x200B;卡片。

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Date]</strong></td> 
   <td><p>顯示取消訂閱/重新訂閱發生的日期。</p></td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Details]</strong></td> 
   <td><p>重新訂閱： [!DNL Sales Connect]管理員已手動從連絡人記錄中移除取消訂閱。 它也可能顯示與聯絡人取消訂閱原因相關的一些細節。</p><p>取消訂閱：連絡人已取消訂閱。</p></td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Source]</strong></td> 
   <td><p>[!DNL Salesforce] 同步：同步處理從[!DNL Salesforce]擷取取消訂閱。</p><p>手動：使用者按一下取消訂閱按鈕以選擇退出。</p><p>點按連結：電子郵件收件者點按取消訂閱連結。</p><p>「管理員名稱」：當動作要重新訂閱連絡人時，會顯示管理員名稱。 這可讓使用者知道誰移除取消訂閱。</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[自訂取消訂閱連結訊息](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
