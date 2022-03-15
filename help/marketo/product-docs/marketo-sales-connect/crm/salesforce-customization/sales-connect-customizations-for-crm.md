---
unique-page-id: 14745793
description: CRM的銷售連接定制 — Marketo文檔 — 產品文檔
title: CRM的銷售連接自定義項
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
source-git-commit: 94f89e64b69d3997effe6736241a68f8314db1e6
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# CRM的銷售連接自定義項 {#sales-connect-customizations-for-crm}

以下欄位和按鈕由Salesforce CRM中的元資料API建立。 建立欄位後，管理員必須在其CRM中配置頁面佈局以公開它們。 可以找到說明 [這裡](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)。

>[!NOTE]
>
>這對ToutApp和Sales Connect客戶都有影響。

## 如何在Salesforce中安裝自定義項 {#how-to-install-customizations-in-salesforce}

1. 在「銷售連接」中，按一下齒輪表徵圖並選擇 **設定**。

   ![](assets/one.png)

1. 在「管理設定」下，選擇 **Salesforce**。

   ![](assets/two.png)

1. 按一下 **Marketo銷售連接自定義**。

   ![](assets/three.png)

1. 按一下 **連接到Salesforce**。

   ![](assets/four.png)

1. 登錄到Salesforce。

   ![](assets/five.png)

## 更新Salesforce自定義 {#update-salesforce-customization}

對Salesforce Customization包的更新將包括增強功能和錯誤修復。 要檢查更新是否可用或是否執行更新，請執行以下步驟。

>[!NOTE]
>
>**需要管理權限。**

1. 在 [Web應用](https://www.toutapp.com)，按一下齒輪表徵圖並選擇 **設定**。

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. 在「Admin Settings（管理設定）」下，按一下 **Salesforce**。

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. Sales Connect Customization卡將顯示是否有可用更新。 按一下 **更新自定義項**。

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. 按一下 **升級**。

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. 等待更新安裝。 根據需要多少個版本號，安裝時間會有所不同。

   ![](assets/sales-connect-customizations-for-crm-10.png)

完成後，您的卡將顯示「您的Sales Connect自定義項是最新的」。

![](assets/sales-connect-customizations-for-crm-11.png)

## 自定義活動欄位 {#custom-activity-fields}

Marketo將檢測到新欄位的建立，然後執行一次性資料回填、重新映射以及值與欄位的持續同步 **新** 僅限。 舊欄位將不會更新。

| **欄位名稱** | **說明** |
|---|---|
| MSE調用本地存在ID | 當您從MSE Phone撥打電話時，作為用戶，可以選擇「本地存在」作為選項。 來電將顯示接收方的本地號碼。 |
| MSE呼叫錄制URL | 可以記錄呼叫，並在此處記錄錄制的連結。 |
| MSE市場活動 | Contact/Lead是其成員的MSE市場活動的日誌名稱。 |
| MSE市場活動URL | 記錄在MSE中建立的市場活動的URL。 按一下此按鈕將開啟MSE Web應用中的市場活動。 |
| MSE市場活動當前步驟 | 如果聯繫人/潛在顧客是市場活動的一部分，此欄位將記錄潛在顧客/潛在顧客當前所在步驟的名稱。 |
| 已查看MSE電子郵件附件 | 當電子郵件與附件一起發送且收件人查看附件時，記錄資料。 |
| 已按一下MSE電子郵件 | 當收件人按一下電子郵件中的連結時，記錄複選標籤。 |
| MSE電子郵件已回復 | 收件人回復電子郵件時記錄複選標籤。 |
| MSE電子郵件狀態 | 顯示是否發送/正在發送/跳轉電子郵件（跟蹤跳轉的電子郵件取決於使用的傳送渠道）。 |
| MSE電子郵件模板 | 在發送到潛在顧客/聯繫人的電子郵件中使用的MSE模板的日誌名稱。 |
| MSE電子郵件模板URL | 將URL記錄到在MSE中建立的模板。 按一下此選項將開啟MSE Web應用中的模板。 |
| MSE電子郵件URL | 按一下此URL將開啟MSE中的Command Center，並拉出「人員詳細資訊視圖」歷史記錄頁籤，在該頁籤中您可以查看已發送的電子郵件。 |
| 已查看MSE電子郵件 | 當收件人查看電子郵件時記錄複選標籤。 |

## 匯總日誌記錄欄位 {#roll-up-logging-fields}

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
   <td>MSE — 上次市場推廣活動</td> 
   <td>上次從市場營銷傳入的項目。 </td> 
  </tr> 
  <tr> 
   <td>MSE — 上次市場營銷訂約日期</td> 
   <td>市場部的參與時間戳。</td> 
  </tr> 
  <tr> 
   <td>MSE — 上次市場推廣項目設計</td> 
   <td>項目描述。</td> 
  </tr> 
  <tr> 
   <td>MSE — 上次市場營銷項目來源</td> 
   <td>市場推廣服務來源。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 上次市場營銷項目類型</td> 
   <td colspan="1">項目類型。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 按銷售列出的上次活動<br></td> 
   <td colspan="1">銷售團隊執行的上次傳出活動。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 上次答復</td> 
   <td colspan="1">上次回復銷售電子郵件。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 當前銷售活動</td> 
   <td colspan="1">潛在客戶/聯繫人是其成員的MSE市場活動的日誌名稱。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 上次銷售項目</td> 
   <td colspan="1">Sales的上次傳入項目。 </td> 
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
| 發送MSE電子郵件 | 從Salesforce發送銷售電子郵件。 |
| 添加到MSE市場活動 | 從Salesforce添加到MSE市場活動。 |
| 推送到MSE | 將聯繫人從Salesforce推送到MSE。 |
| 與MSE通話 | 從Salesforce撥打Sales電話。 |

## 批量操作按鈕 {#bulk-action-buttons}

| **按鈕名稱** | **說明** |
|---|---|
| 添加到MSE市場活動 | 從Salesforce添加到MSE市場活動。 |
| 推送到MSE | 將聯繫人從Salesforce推送到MSE。 |

## 使用手冊 {#user-guides}

[Salesforce中的MSE自定義報表](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[Salesforce的MSE](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[Salesforce閃電的MSE](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
