---
unique-page-id: 14745793
description: CRM的[!DNL Sales Connect]個自訂 — Marketo檔案 — 產品檔案
title: CRM的[!DNL Sales Connect]個自訂
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 2%

---

# CRM的[!DNL Sales Connect]個自訂 {#sales-connect-customizations-for-crm}

下列欄位和按鈕是由Salesforce CRM中的中繼資料API所建立。 建立欄位後，管理員必須在其CRM中設定頁面配置以公開。 指示[可在此找到](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf)。

## 如何在[!DNL Salesforce]中安裝自訂 {#how-to-install-customizations-in-salesforce}

1. 在[!DNL Sales Connect]中，按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/one.png)

1. 在[!UICONTROL Admin Settings]下，選取&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/two.png)

1. 按一下「**[!UICONTROL Marketo Sales Engage Customizations]**」。

   ![](assets/three.png)

1. 按一下「**[!UICONTROL Connect to Salesforce]**」。

   ![](assets/four.png)

1. 登入[!DNL Salesforce]。

   ![](assets/five.png)

## 更新[!DNL Salesforce]自訂 {#update-salesforce-customization}

[!DNL Salesforce]自訂套件的更新將包括增強功能和錯誤修正。 若要檢查是否有可用的更新或要執行更新，請遵循以下步驟。

>[!NOTE]
>
>**需要系統管理員許可權。**

1. 在[網頁應用程式](https://www.toutapp.com)中，按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. 在[!UICONTROL Admin Settings]底下，按一下&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. 如果有可用的更新，則會顯示[!DNL Sales Connect]自訂卡。 按一下「**[!UICONTROL Update Customizations]**」。

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. 按一下「**[!UICONTROL Upgrade]**」。

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. 等候更新安裝。 視您需要的版本編號而定，安裝時間會有所不同。

   ![](assets/sales-connect-customizations-for-crm-10.png)

完成後，您的卡片會顯示「您的Sales Connect自訂內容為最新狀態」。

![](assets/sales-connect-customizations-for-crm-11.png)

## 自訂活動欄位 {#custom-activity-fields}

Marketo將偵測新欄位的建立，然後僅執行資料的一次性回填、重新對應，以及值的持續同步到&#x200B;**新**&#x200B;欄位。 不會更新舊欄位。

<table><thead>
  <tr>
    <th>欄位名稱</th>
    <th>說明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE呼叫本機是否存在ID</td>
    <td>身為使用者，當您從MSE電話撥打電話時，可以選擇「本機顯示狀態」作為選項。 來電會顯示接收者的本機號碼。</td>
  </tr>
  <tr>
    <td>MSE通話錄製URL</td>
    <td>可以錄製通話，並在這裡記錄錄製的連結。</td>
  </tr>
  <tr>
    <td>MSE行銷活動</td>
    <td>記錄連絡人/潛在客戶所屬的MSE促銷活動的名稱。</td>
  </tr>
  <tr>
    <td>MSE促銷活動URL</td>
    <td>將URL記錄到在MSE中建立的行銷活動。 按一下此按鈕，MSE網頁應用程式中便會開啟促銷活動。</td>
  </tr>
  <tr>
    <td>MSE行銷活動目前步驟</td>
    <td>如果聯絡人/潛在客戶屬於行銷活動，此欄位將記錄該聯絡人/聯絡人目前所在步驟的名稱。</td>
  </tr>
  <tr>
    <td>已檢視MSE電子郵件附件</td>
    <td>當電子郵件連同附件傳送且收件者檢視附件時，會記錄資料。</td>
  </tr>
  <tr>
    <td>MSE電子郵件已點按</td>
    <td>當收件者按一下電子郵件中的連結時，記錄核取記號。</td>
  </tr>
  <tr>
    <td>MSE電子郵件已回覆</td>
    <td>當收件者回覆電子郵件時記錄核取記號。</td>
  </tr>
  <tr>
    <td>MSE電子郵件狀態</td>
    <td>顯示電子郵件是否已傳送/進行中/退回（追蹤退回電子郵件取決於使用的傳遞頻道）。</td>
  </tr>
  <tr>
    <td>mse電子郵件範本</td>
    <td>記錄用於傳送給潛在客戶/聯絡人的電子郵件中的MSE範本名稱。</td>
  </tr>
  <tr>
    <td>MSE電子郵件範本URL</td>
    <td>將URL記錄到在MSE中建立的範本。 按一下此圖示即會在MSE網頁應用程式中開啟範本。</td>
  </tr>
  <tr>
    <td>MSE電子郵件URL</td>
    <td>按一下此URL將會在MSE中開啟Command Center，並拉出「人員詳細資料檢視歷史記錄」標籤，您可在其中檢視已傳送的電子郵件。</td>
  </tr>
  <tr>
    <td>已檢視的MSE電子郵件</td>
    <td>當收件者檢視電子郵件時，記錄核取記號。</td>
  </tr>
</tbody></table>

## 統計記錄欄位 {#roll-up-logging-fields}

<table><thead>
  <tr>
    <th>欄位名稱</th>
    <th>說明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE — 上次行銷參與</td>
    <td>上次來自行銷的傳入參與。</td>
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
    <td>MSE — 上次行銷參與Source</td>
    <td>行銷參與的Source。</td>
  </tr>
  <tr>
    <td>MSE — 上次行銷參與型別</td>
    <td>參與型別。</td>
  </tr>
  <tr>
    <td>MSE — 依銷售顯示的最後一個活動</td>
    <td>銷售團隊執行的最後一個傳出活動。</td>
  </tr>
  <tr>
    <td>MSE — 上次回覆</td>
    <td>銷售電子郵件的最後一封電子郵件回覆。</td>
  </tr>
  <tr>
    <td>MSE — 目前的促銷活動</td>
    <td>記錄潛在客戶/聯絡人所屬的MSE促銷活動的名稱。</td>
  </tr>
  <tr>
    <td>MSE — 上次銷售參與</td>
    <td>上次來自銷售人員的傳入參與。</td>
  </tr>
  <tr>
    <td>MSE — 選擇退出</td>
    <td>選擇退出欄位。</td>
  </tr>
</tbody></table>

## 按鈕 {#buttons}

<table><thead>
  <tr>
    <th>按鈕名稱</th>
    <th>說明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>傳送MSE電子郵件</td>
    <td>從Salesforce傳送銷售電子郵件。</td>
  </tr>
  <tr>
    <td>新增至MSE行銷活動</td>
    <td>從Salesforce新增至MSE行銷活動。</td>
  </tr>
  <tr>
    <td>推送至MSE</td>
    <td>將連絡人從Salesforce推播至MSE。</td>
  </tr>
  <tr>
    <td>使用MSE呼叫</td>
    <td>從Salesforce撥打銷售電話。</td>
  </tr>
</tbody>
</table>

## 大量動作按鈕 {#bulk-action-buttons}

<table><thead>
  <tr>
    <th>按鈕名稱</th>
    <th>說明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>新增至MSE行銷活動</td>
    <td>從Salesforce新增至MSE行銷活動。</td>
  </tr>
  <tr>
    <td>推送至MSE</td>
    <td>將連絡人從Salesforce推播至MSE。</td>
  </tr>
</tbody>
</table>

## 使用手冊 {#user-guides}

[Salesforce中的MSE自訂報表](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/reports-and-dashboards.pdf)

[適用於Salesforce Classic的MSE](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf)

[Salesforce Lightning的MSE](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/sfdc-guide-lightning.pdf)
