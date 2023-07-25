---
unique-page-id: 14745793
description: CRM的Sales Connect自訂 — Marketo檔案 — 產品檔案
title: CRM的Sales Connect自訂
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 1%

---

# CRM的Sales Connect自訂 {#sales-connect-customizations-for-crm}

以下欄位和按鈕是由Salesforce CRM中的中繼資料API所建立。 建立欄位後，管理員必須在其CRM中設定頁面配置，才能公開這些欄位。 您可以找到指示 [此處](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>這會影響ToutApp和Sales Connect客戶。

## 如何在Salesforce中安裝自訂 {#how-to-install-customizations-in-salesforce}

1. 在Sales Connect中，按一下齒輪圖示並選取 **設定**.

   ![](assets/one.png)

1. 在「管理設定」下，選取 **Salesforce**.

   ![](assets/two.png)

1. 按一下 **Marketo Sales Connect自訂**.

   ![](assets/three.png)

1. 按一下 **連線到Salesforce**.

   ![](assets/four.png)

1. 登入Salesforce。

   ![](assets/five.png)

## 更新Salesforce自訂 {#update-salesforce-customization}

Salesforce自訂套件的更新將包括增強功能和錯誤修正。 若要檢查是否有可用更新或執行更新，請遵循以下步驟。

>[!NOTE]
>
>**需要管理員許可權。**

1. 在 [網頁應用程式](https://www.toutapp.com)，按一下齒輪圖示並選取 **設定**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. 在「管理設定」底下，按一下 **Salesforce**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. Sales Connect Customization卡片將顯示是否有更新。 按一下 **更新自訂**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. 按一下 **升級**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. 等候更新安裝。 視您需要的版本編號數目而定，安裝時間會有所不同。

   ![](assets/sales-connect-customizations-for-crm-10.png)

完成後，您的卡片將顯示「您的Sales Connect自訂為最新」。

![](assets/sales-connect-customizations-for-crm-11.png)

## 自訂活動欄位 {#custom-activity-fields}

Marketo會偵測新欄位的建立，然後執行一次性資料回填、重新對應，並將值持續同步到 **新** 僅限欄位。 不會更新舊欄位。

| **欄位名稱** | **說明** |
|---|---|
| MSE呼叫本機是否存在ID | 身為使用者，當您從MSE電話進行呼叫時，可以選擇「本機狀態」作為選項。 來電會顯示接收者的本機號碼。 |
| MSE通話錄製URL | 可以錄製通話，並在這裡記錄錄製的連結。 |
| MSE行銷活動 | 記錄連絡人/潛在客戶所屬的MSE促銷活動的名稱。 |
| MSE促銷活動URL | 將URL記錄到在MSE中建立的行銷活動。 按一下此專案即會在MSE網頁應用程式中開啟促銷活動。 |
| MSE行銷活動目前步驟 | 如果連絡人/潛在客戶屬於行銷活動，此欄位將記錄潛在客戶/連絡人目前所在步驟的名稱。 |
| 已檢視MSE電子郵件附件 | 在傳送包含附件的電子郵件且收件者檢視附件時記錄資料。 |
| MSE電子郵件已點按 | 當收件者按一下電子郵件中的連結時，記錄核取記號。 |
| mse電子郵件已回覆 | 當收件者回覆電子郵件時記錄核取記號。 |
| MSE電子郵件狀態 | 顯示電子郵件是否已傳送/進行中/彈回（追蹤彈回電子郵件取決於使用的傳送頻道）。 |
| mse電子郵件範本 | 記錄用於傳送給潛在客戶/連絡人之電子郵件的MSE範本名稱。 |
| MSE電子郵件範本URL | 將URL記錄到在MSE中建立的範本。 按一下此專案即會在MSE網頁應用程式中開啟範本。 |
| MSE電子郵件URL | 按一下此URL將會在MSE中開啟Command Center，並拉出「人員詳細資料檢視歷史記錄」標籤，您可以在其中檢視傳送的電子郵件。 |
| 已檢視的MSE電子郵件 | 當收件者檢視電子郵件時記錄核取記號。 |

## 統計記錄欄位 {#roll-up-logging-fields}

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
   <td>上次來自行銷的傳入參與。 </td> 
  </tr> 
  <tr> 
   <td>MSE — 上次行銷參與日期</td> 
   <td>來自行銷的參與時間戳記。</td> 
  </tr> 
  <tr> 
   <td>MSE — 上次行銷參與說明</td> 
   <td>參與的說明。</td> 
  </tr> 
  <tr> 
   <td>MSE — 上次行銷參與來源</td> 
   <td>行銷參與來源。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 上次行銷參與型別</td> 
   <td colspan="1">參與型別。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 依據銷售列出的最後一個活動<br></td> 
   <td colspan="1">銷售團隊執行的最後一個傳出活動。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 上次回覆</td> 
   <td colspan="1">銷售電子郵件的最後一封電子郵件回覆。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 目前的促銷活動</td> 
   <td colspan="1">記錄潛在客戶/聯絡人所屬的MSE促銷活動的名稱。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 上次銷售參與</td> 
   <td colspan="1">上次來自銷售人員的傳入參與。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 選擇退出</td> 
   <td colspan="1">選擇退出欄位。</td> 
  </tr> 
 </tbody> 
</table>

## 按鈕 {#buttons}

| **按鈕名稱** | **說明** |
|---|---|
| 傳送MSE電子郵件 | 從Salesforce傳送銷售電子郵件。 |
| 新增至MSE行銷活動 | 從Salesforce新增至MSE行銷活動。 |
| 推送至MSE | 將連絡人從Salesforce推播至MSE。 |
| 使用MSE呼叫 | 從Salesforce進行銷售通話。 |

## 大量動作按鈕 {#bulk-action-buttons}

| **按鈕名稱** | **說明** |
|---|---|
| 新增至MSE行銷活動 | 從Salesforce新增至MSE行銷活動。 |
| 推送至MSE | 將連絡人從Salesforce推播至MSE。 |

## 使用手冊 {#user-guides}

[Salesforce中的MSE自訂報表](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[Salesforce的MSE](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[Salesforce Lightning的MSE](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
