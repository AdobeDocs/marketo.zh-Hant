---
unique-page-id: 14745793
description: CRM的Sales Connect自訂 — Marketo檔案 — 產品檔案
title: CRM的Sales Connect自定義
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
source-git-commit: 2712a21b7457ef51a9112074465c54e8f7954fa9
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# CRM的Sales Connect自定義 {#sales-connect-customizations-for-crm}

以下欄位和按鈕由Salesforce CRM中的中繼資料API建立。 建立欄位後，管理員必須在其CRM中設定頁面配置，以公開這些欄位。 可找到指示 [此處](https://docs.marketo.com/display/docs/assets/marketo-sales-engage-for-salesforce-installation-and-success-guide.pdf).

>[!NOTE]
>
>這會影響ToutApp和Sales Connect客戶。

## 如何在Salesforce中安裝自訂 {#how-to-install-customizations-in-salesforce}

1. 在Sales Connect中，按一下齒輪表徵圖並選擇 **設定**.

   ![](assets/one.png)

1. 在「管理設定」下，選取 **Salesforce**.

   ![](assets/two.png)

1. 按一下 **Marketo Sales Connect自定義**.

   ![](assets/three.png)

1. 按一下 **連接到Salesforce**.

   ![](assets/four.png)

1. 登入Salesforce。

   ![](assets/five.png)

## 更新Salesforce自訂 {#update-salesforce-customization}

Salesforce自訂套件的更新將包含增強功能和錯誤修正。 要檢查更新是否可用或執行更新，請執行以下步驟。

>[!NOTE]
>
>**需要管理員權限。**

1. 在 [網頁應用程式](https://www.toutapp.com)，按一下齒輪圖示並選取 **設定**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. 在「管理設定」下，按一下 **Salesforce**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. 如果有更新，將顯示Sales Connect自定義卡。 按一下 **更新自訂**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. 按一下 **升級**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. 等待更新以安裝。 安裝時間會因您所需的版本號碼而異。

   ![](assets/sales-connect-customizations-for-crm-10.png)

完成後，您的卡片將顯示「您的Sales Connect自定義項為最新」。

![](assets/sales-connect-customizations-for-crm-11.png)

## 自訂活動欄位 {#custom-activity-fields}

Marketo會偵測新欄位的建立，然後執行一次性回填資料、重新對應，以及將值持續同步至 **new** 欄位。 不會更新舊欄位。

| **欄位名稱** | **說明** |
|---|---|
| MSE呼叫本機存在ID | 從MSE Phone進行呼叫時，您可以選擇「本機狀態」作為選項。 傳入的呼叫將顯示接收器的本地號碼。 |
| MSE呼叫記錄URL | 您可以記錄呼叫，並在此處記錄錄制的連結。 |
| MSE促銷活動 | 記錄Contact/Lead所屬MSE促銷活動的名稱。 |
| MSE促銷活動URL | 將URL記錄到以MSE建立的促銷活動。 按一下，便會開啟MSE網頁應用程式中的促銷活動。 |
| MSE促銷活動目前步驟 | 如果聯絡人/銷售機會是促銷活動的一部分，此欄位將記錄銷售機會/聯繫人目前所在步驟的名稱。 |
| 已查看MSE電子郵件附件 | 當電子郵件隨附件傳送且收件者檢視附件時，記錄資料。 |
| 已點按MSE電子郵件 | 當收件者按一下電子郵件中的連結時，記錄核取記號。 |
| MSE電子郵件已回覆 | 當收件者回覆電子郵件時，記錄核取記號。 |
| MSE電子郵件狀態 | 顯示電子郵件是否已傳送/進行中/已退信（追蹤已退信電子郵件取決於使用的傳送管道）。 |
| MSE電子郵件範本 | 記錄傳送至銷售機會/連絡人之電子郵件中所使用之MSE範本的名稱。 |
| MSE電子郵件範本URL | 將URL記錄到以MSE建立的範本。 按一下，便會開啟MSE Web應用程式中的範本。 |
| MSE電子郵件URL | 按一下此URL將開啟MSE中的Command Center，並拉出「人員詳細資訊視圖」歷史記錄頁簽，您可以在其中查看已發送的電子郵件。 |
| 已檢視MSE電子郵件 | 當收件者檢視電子郵件時，記錄核取記號。 |

## 匯總記錄欄位 {#roll-up-logging-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>欄位名稱</strong></td> 
   <td><strong>說明</strong></td> 
  </tr> 
  <tr> 
   <td>MSE — 上次行銷參與</td> 
   <td>上次從行銷傳入的參與。 </td> 
  </tr> 
  <tr> 
   <td>MSE — 上次行銷參與日期</td> 
   <td>來自行銷的參與時間戳記。</td> 
  </tr> 
  <tr> 
   <td>MSE — 上次行銷參與次數</td> 
   <td>參與的說明。</td> 
  </tr> 
  <tr> 
   <td>MSE — 上次行銷參與來源</td> 
   <td>行銷參與的來源。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 上次行銷參與類型</td> 
   <td colspan="1">參與類型。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 按銷售列出的上次活動<br></td> 
   <td colspan="1">銷售團隊執行的上次傳出活動。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 上次答復</td> 
   <td colspan="1">上次回覆銷售電子郵件的電子郵件。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 當前銷售活動</td> 
   <td colspan="1">記錄銷售機會/連絡人所屬MSE促銷活動的名稱。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 上次銷售參與</td> 
   <td colspan="1">來自Sales的上次傳入參與。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 選擇退出</td> 
   <td colspan="1">退出欄位。</td> 
  </tr> 
 </tbody> 
</table>

## 按鈕 {#buttons}

| **按鈕名稱** | **說明** |
|---|---|
| 傳送MSE電子郵件 | 從Salesforce傳送銷售電子郵件。 |
| 新增至MSE促銷活動 | 從Salesforce新增至MSE促銷活動。 |
| 推送至MSE | 從Salesforce推送連絡人至MSE。 |
| 使用MSE呼叫 | 從Salesforce進行銷售呼叫。 |

## 批量操作按鈕 {#bulk-action-buttons}

| **按鈕名稱** | **說明** |
|---|---|
| 新增至MSE促銷活動 | 從Salesforce新增至MSE促銷活動。 |
| 推送至MSE | 從Salesforce推送連絡人至MSE。 |

## 使用手冊 {#user-guides}

[Salesforce中的MSE自訂報表](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[Salesforce的MSE](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[Salesforce閃電的MSE](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
