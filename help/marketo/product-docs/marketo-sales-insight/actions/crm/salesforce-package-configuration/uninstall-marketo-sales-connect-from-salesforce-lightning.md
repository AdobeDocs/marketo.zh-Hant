---
description: 從Salesforce Lightning解除安裝Marketo Sales Connect - Marketo檔案 — 產品檔案
title: 從Salesforce Lightning解除安裝Marketo Sales Connect
exl-id: 4af89222-22b1-4c08-8081-3dab89d1985b
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '1192'
ht-degree: 5%

---

# 從Salesforce Lightning解除安裝Marketo Sales Connect {#uninstall-marketo-sales-connect-from-salesforce-lightning}

以下說明當您開始使用Sales Insight Actions時，如何從Salesforce帳戶解除安裝Marketo Sales Connect套件。

## 從頁面配置移除Sales Connect欄位 {#remove-sales-connect-fields-from-page-layout}

1. 在Salesforce Lightning中，按一下齒輪圖示並選取&#x200B;**設定**。

   ![](assets/uninstall-salesforce-lightning-customization-package-1.png)

1. 按一下&#x200B;**物件管理員**。

   ![](assets/uninstall-salesforce-lightning-customization-package-2.png)

1. 向下捲動至並選取&#x200B;**銷售機會**。

   ![](assets/uninstall-salesforce-lightning-customization-package-3.png)

1. 按一下&#x200B;**頁面配置**。

   ![](assets/uninstall-salesforce-lightning-customization-package-4.png)

1. 按一下&#x200B;**銷售機會配置**。

   ![](assets/uninstall-salesforce-lightning-customization-package-5.png)

   >[!NOTE]
   >
   >尚未在Salesforce Lightning中更新「編輯頁面配置」檢視。

1. 在主控台中，選取&#x200B;**欄位**。 在「快速尋找」中搜尋「MSC」。 所有灰色的欄位已新增至您的頁面配置。 您必須刪除這些專案。

   ![](assets/uninstall-salesforce-lightning-customization-package-6.png)

   >[!NOTE]
   >
   >如果沒有欄位顯示為灰色，表示您尚未將其新增至頁面配置。 您可以略過本節。

1. 捲動至包含您的Sales Connect自訂欄位的區段。

   ![](assets/uninstall-salesforce-lightning-customization-package-7.png)

1. 有10種型別的MSC欄位可以新增至此區段。 移除所有新增的欄位，或直接刪除整個區段。

1. 完成時，按一下&#x200B;**快速儲存**。

   ![](assets/uninstall-salesforce-lightning-customization-package-8.png)

## 從頁面配置移除Sales Connect按鈕 {#remove-sales-connect-buttons-from-page-layouts}

1. 在主控台（上述步驟4）中，選取&#x200B;**按鈕**。 搜尋「MSC」。 所有灰色的按鈕已新增到您的自訂按鈕區段。 您必須刪除這些專案。

   ![](assets/uninstall-salesforce-lightning-customization-package-9.png)

   >[!NOTE]
   >
   >如果沒有任何按鈕呈現灰色，表示您尚未新增這些按鈕。 您可以略過本節。

1. 將MSC按鈕從「自訂按鈕」區段拖放至主控台。

   ![](assets/uninstall-salesforce-lightning-customization-package-10.png)

1. 完成時，按一下&#x200B;**快速儲存**。

   ![](assets/uninstall-salesforce-lightning-customization-package-11.png)

## 從活動歷史記錄區段中移除Sales Connect欄位 {#remove-sales-connect-fields-from-activity-history-section}

1. 捲動至頁面底部至「活動歷史記錄」相關清單區段，然後按一下「扳手」圖示。

   ![](assets/uninstall-salesforce-lightning-customization-package-12.png)

1. 從「選取的欄位」區域中選取「銷售連線欄位」，然後按一下「移除」箭頭。 完成時，按一下&#x200B;**確定**。

   ![](assets/uninstall-salesforce-lightning-customization-package-13.png)

   >[!NOTE]
   >
   >縮寫MSE _是_ Sales Connect。 它只是先前名稱「Marketo銷售參與」。

1. 完成Leads頁面時，按一下&#x200B;**儲存**。

## 從潛在客戶清單檢視中移除Sales Connect大量作業按鈕 {#remove-sales-connect-bulk-action-buttons-from-lead-list-view}

1. 在Salesforce Lightning中，按一下齒輪圖示並選取&#x200B;**設定**。

   ![](assets/uninstall-salesforce-lightning-customization-package-14.png)

1. 按一下&#x200B;**物件管理員**。

   ![](assets/uninstall-salesforce-lightning-customization-package-15.png)

1. 向下捲動至並選取&#x200B;**銷售機會**。

   ![](assets/uninstall-salesforce-lightning-customization-package-16.png)

1. 按一下&#x200B;**搜尋配置**。

   ![](assets/uninstall-salesforce-lightning-customization-package-17.png)

1. 按一下[清單檢視]旁的箭頭，然後選取&#x200B;**編輯**。

   ![](assets/uninstall-salesforce-lightning-customization-package-18.png)

1. 選取&#x200B;**新增至MSC促銷活動**、**含MSC的電子郵件**&#x200B;和&#x200B;**推送至MSC**，然後按一下[移除]箭頭。 然後按一下[儲存]。****

   ![](assets/uninstall-salesforce-lightning-customization-package-19.png)

您應該不會再看到潛在客戶清單檢視上的按鈕。

## 移除連絡人的MSC設定 {#remove-msc-configuration-for-contacts}

1. 在Salesforce Lightning中，按一下齒輪圖示並選取&#x200B;**設定**。

1. 按一下&#x200B;**物件管理員**。

1. 向下捲動至並選取&#x200B;**連絡人**。

1. 按一下&#x200B;**頁面配置**。

1. 按一下&#x200B;**連絡人配置**。

1. 從所有三個區段重複步驟。

## 移除商機的MSC設定 {#remove-msc-configuration-for-opportunity}

1. 在Salesforce Lightning中，按一下齒輪圖示並選取&#x200B;**設定**。

1. 按一下&#x200B;**物件管理員**。

1. 向下捲動至並選取&#x200B;**機會**。

1. 按一下&#x200B;**頁面配置**。

1. 按一下&#x200B;**機會配置**。

機會檢視只有一個按鈕 — 「傳送MSE電子郵件」和以下欄位：

![](assets/uninstall-salesforce-lightning-customization-package-20.png)

## 移除帳戶的MSC設定 {#remove-msc-configuration-for-account}

1. 在Salesforce Lightning中，按一下齒輪圖示並選取&#x200B;**設定**。

1. 按一下&#x200B;**物件管理員**。

1. 向下捲動至並選取&#x200B;**帳戶**。

1. 按一下&#x200B;**頁面配置**。

1. 按一下&#x200B;**帳戶配置**。

帳戶檢視只有一個按鈕 — 「傳送MSE電子郵件」和以下欄位：

![](assets/uninstall-salesforce-lightning-customization-package-21.png)

## 移除Marketo銷售寄件匣 {#remove-marketo-sales-outbox}

1. 在Salesforce中，按一下熒幕上方的&#x200B;**+**&#x200B;標籤。

1. 按一下&#x200B;**自訂我的標籤**。

1. 從右側選取「Marketo銷售寄件匣」選項。 按一下[移除]箭頭，然後按一下[儲存]。****。

## 刪除Sales Connect封裝 {#delete-sales-connect-package}

從Salesforce帳戶移除所有物件後，請遵循下列步驟。

1. 在Salesforce Lightning中，按一下齒輪圖示並選取&#x200B;**設定**。

1. 在「快速尋找」方塊中，輸入「Apex類別」。

1. 按一下清單上所有「MarketoSalesConnectionCustomization」或「MarketoSalesEngageCustomization」專案旁的&#x200B;**刪除**。

一切就緒！

以下是需要從Salesforce例項中移除的所有物件清單：

## Sales Connect自訂詳細資料 {#sales-connect-customization-details}

<table>
 <tr>
  <th>自訂活動欄位</th>
  <th>說明</th>
  <th>類型</th>
  <th>資料類型</th>
 </tr>
 <tr>
  <td>MSC呼叫本機目前狀態識別碼</td>
  <td>身為使用者，我可以在透過MSC電話進行呼叫時，選擇「本機顯示狀態」作為選項。 來電會顯示接收者的本機號碼</td>
  <td>活動</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>MSC通話錄製URL</td>
  <td>可以錄製通話，並在這裡記錄錄製的連結 </td>
  <td>活動</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>MSC行銷活動</td>
  <td>記錄連絡人/潛在客戶所在的MSC行銷活動的名稱</td>
  <td>活動</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>MSC促銷活動URL</td>
  <td>將URL記錄到在MSC中建立的行銷活動。 按一下此按鈕，就會在MSC網頁應用程式中開啟促銷活動</td>
  <td>活動</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>MSC促銷活動目前步驟</td>
  <td>如果連絡人/潛在客戶在行銷活動中，此欄位將記錄他們目前所在步驟的名稱</td>
  <td>活動</td>
  <td>核取方塊</td>
 </tr>
 <tr>
  <td>已檢視的MSC電子郵件附件</td>
  <td>在傳送包含收件者檢視之附件的電子郵件時記錄資料</td>
  <td>活動</td>
  <td>核取方塊</td>
 </tr>
 <tr>
  <td>MSC電子郵件已點按</td>
  <td>當收件者按一下電子郵件中的連結時，記錄核取記號</td>
  <td>活動</td>
  <td>核取方塊</td>
 </tr>
 <tr>
  <td>MSC電子郵件已回覆</td>
  <td>在收件者回覆電子郵件時記錄核取記號</td>
  <td>活動</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>MSC電子郵件狀態</td>
  <td>顯示電子郵件是否已傳送/進行中/退回（追蹤退回電子郵件取決於使用的傳遞頻道）</td>
  <td>活動</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>MSC電子郵件範本</td>
  <td>記錄用於傳送給潛在客戶/連絡人的電子郵件中的MSC範本名稱</td>
  <td>活動</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>MSC電子郵件範本URL</td>
  <td>將URL記錄到在MSC中建立的範本。 按一下此選項會在MSC網頁應用程式中開啟範本</td>
  <td>活動</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>MSC電子郵件URL</td>
  <td>按一下此URL將會開啟MSC中的命令中心，並拉出「人員詳細資料檢視歷史記錄」標籤，使用者可以在其中檢視已傳送的電子郵件</td>
  <td>活動</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>已檢視的MSC電子郵件</td>
  <td>在收件者檢視電子郵件時記錄核取記號</td>
  <td>活動</td>
  <td>核取方塊</td>
 </tr>
</table>

<table>
 <tr>
  <th>MSC累計記錄欄位</th>
  <th>說明</th>
  <th>類型</th>
  <th>資料類型</th>
 </tr>
 <tr>
  <td>MSC — 上次行銷參與</td>
  <td>上次來自行銷的傳入參與</td>
  <td>
  <p>帳戶
  <p>連絡人
  <p>銷售機會
  <p>機會</td>
  <td>資料與時間</td>
 </tr>
 <tr>
  <td>MSC — 上次行銷參與日期</td>
  <td>來自行銷的參與時間戳記</td>
  <td>
  <p>帳戶 
  <p>連絡人 
  <p>銷售機會 
  <p>機會</td>
  <td>資料與時間</td>
 </tr>
 <tr>
  <td>MSC — 上次行銷參與摘要</td>
  <td>參與的說明</td>
  <td>
  <p>帳戶 
  <p>連絡人 
  <p>銷售機會 
  <p>機會</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>MSC — 上次行銷參與Source</td>
  <td>行銷參與的Source</td>
  <td>
  <p>帳戶 
  <p>連絡人 
  <p>銷售機會 
  <p>機會</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>MSC — 上次行銷參與型別</td>
  <td>參與型別（例如：網路活動）</td>
  <td>
  <p>帳戶 
  <p>連絡人 
  <p>銷售機會 
  <p>機會</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>MSC — 按銷售列出的最後作業</td>
  <td>銷售團隊執行的最後一個傳出活動</td>
  <td>
  <p>帳戶 
  <p>連絡人 
  <p>銷售機會 
  <p>機會</td>
  <td>資料與時間</td>
 </tr>
 <tr>
  <td>MSC — 上次回覆</td>
  <td>銷售電子郵件的最後一封電子郵件回覆</td>
  <td>
  <p>帳戶 
  <p>連絡人 
  <p>銷售機會 
  <p>機會</td>
  <td>資料與時間</td>
 </tr>
 <tr>
  <td>MSC — 目前的促銷活動</td>
  <td>記錄連絡人/潛在客戶所在的MSC行銷活動的名稱</td>
  <td>
  <p>帳戶 
  <p>連絡人 
  <p>銷售機會 
  <p>機會</td>
  <td>文字</td>
 </tr>
 <tr>
  <td>MSC — 上次銷售業務開發</td>
  <td>上次來自銷售人員的傳入參與</td>
  <td>
  <p>帳戶
  <p>連絡人
  <p>銷售機會
  <p>機會</td>
  <td>資料與時間</td>
 </tr>
 <tr>
  <td>MSC — 選擇退出</td>
  <td>選擇退出欄位</td>
  <td>
  <p>帳戶 
  <p>連絡人 
  <p>銷售機會 
  <p>機會</td>
  <td>核取方塊</td>
 </tr>
</table>

<table>
 <tr>
  <th>MSC按鈕</th>
  <th>說明</th>
  <th>類型</th>
 </tr>
 <tr>
  <td>傳送MSC電子郵件</td>
  <td>從Salesforce傳送銷售電子郵件</td>
  <td>
  <p>帳戶 
  <p>連絡人 
  <p>銷售機會 
  <p>機會</td>
 </tr>
 <tr>
  <td>新增至MSC Campaign</td>
  <td>從Salesforce新增至MSC行銷活動</td>
  <td>
  <p>連絡人
  <p>銷售機會</td>
 </tr>
 <tr>
  <td>推送至MSC</td>
  <td>從Salesforce將連絡人推播至MSC</td>
  <td>
  <p>連絡人
  <p>銷售機會</td>
 </tr>
 <tr>
  <td>使用MSC來電</td>
  <td>從Salesforce進行銷售通話</td>
  <td>
  <p>連絡人
  <p>銷售機會</td>
 </tr>
</table>

<table>
 <tr>
  <th>MSC大量作業按鈕</th>
  <th>說明</th>
  <th>類型</th>
 </tr>
 <tr>
  <td>新增至MSC Campaign</td>
  <td>從Salesforce新增至MSC行銷活動</td>
  <td>
  <p>連絡人
  <p>銷售機會</td>
 </tr>
 <tr>
  <td>推送至MSC</td>
  <td>從Salesforce將連絡人推播至MSC</td>
  <td>
  <p>連絡人
  <p>銷售機會</td>
 </tr>
 <tr>
  <td>使用MSC傳送電子郵件</td>
  <td>使用Salesforce的MSC傳送電子郵件</td>
  <td>
  <p>連絡人
  <p>銷售機會</td>
 </tr>
</table>
