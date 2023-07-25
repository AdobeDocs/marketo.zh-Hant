---
description: Salesforce同步狀態 — Marketo檔案 — 產品檔案
title: Salesforce同步狀態
exl-id: 61197808-7812-4e0a-8ac6-4a60af0f7979
feature: Salesforce Integration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 3%

---

# Salesforce同步狀態 {#salesforce-sync-status}

使用同步狀態儀表板來檢視同步步驟中的同步狀態及其成功狀態。

同步步驟反映物件結構描述和資料本身的每個物件型別對推送或拉出的操作。 統計資料涵蓋同步處理期間的新記錄、更新、刪除和失敗計數。 使用者可依日期、作業型別或物件型別進行篩選。 同步狀態儀表板顯示過去五天的同步週期狀態。

>[!NOTE]
>
>需要管理員許可權

## 檢視同步狀態 {#view-sync-status}

1. 按一下 **管理員**.

   ![](assets/salesforce-sync-status-1.png)

1. 在「整合」下，按一下Salesforce，然後按一下「同步狀態」標籤。

   ![](assets/salesforce-sync-status-2.png)

依預設，統計資料會依最近啟動的專案排序。 您可以按一下排序圖示，依「開始時間」或「結束時間」排序（從最近到最舊）。

![](assets/salesforce-sync-status-3.png)

## 篩選器同步狀態 {#filter-sync-status}

1. 若要篩選資料，請按一下頁面最右側的篩選圖示。

   ![](assets/salesforce-sync-status-4.png)

1. 選取您的日期和時間範圍，然後按一下下拉式清單，依「物件型別」、「作業型別」和/或「狀態型別」篩選。

   ![](assets/salesforce-sync-status-5.png)

1. 按一下 **套用**.

   ![](assets/salesforce-sync-status-6.png)

**選擇性步驟**：若要匯出同步錯誤，請按一下 **匯出**. 資料將會匯出為CSV。

![](assets/salesforce-sync-status-7.png)

## 同步狀態列位 {#sync-status-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>欄位</th> 
   <th>說明</th> 
   <th>列舉值</th> 
  </tr> 
  <tr> 
   <td colspan="1">開始時間</td> 
   <td colspan="1">同步週期開始日期/時間（使用者的時區）</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">結束時間</td> 
   <td colspan="1">同步週期結束日期/時間（使用者的時區）</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">物件</td> 
   <td colspan="1">物件類型</td> 
   <td colspan="1">聯絡人、人員、任務、商機、銷售機會、其他，如下所示</td> 
  </tr>  
  <tr> 
   <td colspan="1">作業</td> 
   <td colspan="1">作業型別</td> 
   <td colspan="1">作業型別，如下所示</td> 
  </tr>  
  <tr> 
   <td colspan="1">狀態</td> 
   <td colspan="1">批次的狀態</td> 
   <td colspan="1">成功、失敗、不完整、處理中、已清除*</td> 
  </tr>
  <tr> 
   <td colspan="1">最新</td> 
   <td colspan="1">新記錄計數</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">更新時間</td> 
   <td colspan="1">已更新記錄計數</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">已刪除</td> 
   <td colspan="1">刪除的記錄數</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">失敗的專案</td> 
   <td colspan="1">同步失敗的記錄數</td> 
   <td colspan="1"><br></td> 
  </tr>  
  <tr> 
   <td colspan="1">已略過</td> 
   <td colspan="1">因為Sync的感興趣欄位沒有變更而略過的記錄數</td> 
   <td colspan="1"></td> 
  </tr>  
 </tbody> 
</table>

&#42;同步步驟失敗後，資料恢復為先前的完整性狀態。

## 物件類型 {#object-type}

<table> 
 <colgroup> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td colspan="1">帳戶</td> 
  </tr>  
  <tr> 
   <td colspan="1">帳戶型別</td> 
  </tr> 
  <tr> 
   <td colspan="1">自訂物件</td> 
  </tr>  
  <tr> 
   <td colspan="1">Campaign</td> 
  </tr>  
  <tr> 
   <td colspan="1">行銷活動會員狀態</td> 
  </tr>
  <tr> 
   <td colspan="1">連絡人</td> 
  </tr>  
  <tr> 
   <td colspan="1">電子郵件範本</td> 
  </tr>  
  <tr> 
   <td colspan="1">Event</td> 
  </tr> 
  <tr> 
   <td colspan="1">人員（銷售機會）</td> 
  </tr>  
  <tr> 
   <td colspan="1">機會</td> 
  </tr>  
  <tr> 
   <td colspan="1">機會聯絡人角色</td> 
  </tr>  
  <tr> 
   <td colspan="1">任務</td> 
  </tr>  
  <tr> 
   <td colspan="1">使用者</td> 
  </tr>  
 </tbody> 
</table>

## 作業型別 {#operation-type}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>作業型別</th> 
   <th>對這些物件找到</th> 
   <th>備註</th> 
   <th>作業型別</th>
  </tr> 
  <tr> 
   <td colspan="1">與計畫的初始連結</td> 
   <td colspan="1">Campaign</td> 
   <td colspan="1">將行銷活動連結至方案</td> 
   <td colspan="1">更新</td>
  </tr>  
  <tr> 
   <td colspan="1">提取轉換</td> 
   <td colspan="1">人員（銷售機會）*</td> 
   <td colspan="1">提取從SFDC轉換至Marketo的動作。 單位（編號）是轉換為聯絡人的潛在客戶</td> 
   <td colspan="1">更新，失敗專案或略過</td>
  </tr> 
  <tr> 
   <td colspan="1">提取刪除</td> 
   <td colspan="1">聯絡人，人員（銷售機會），機會，行銷活動，行銷活動成員，機會聯絡人，自訂物件，行銷活動，行銷活動成員狀態，機會聯絡人角色</td> 
   <td colspan="1">正在同步至Marketo的已刪除SFDC記錄</td> 
   <td colspan="1">已刪除、失敗專案或已略過</td>
  </tr>  
  <tr> 
   <td colspan="1">提取更新</td> 
   <td colspan="1">任務，人員（銷售機會），人員（銷售機會）佇列，聯絡人，事件，機會，帳戶，帳戶型別，促銷活動成員，自訂物件，促銷活動，促銷活動成員狀態，事件，人員狀態，機會，機會聯絡人角色</td> 
   <td colspan="1">SFDC中的更新或新記錄同步至Marketo，提取事件作為活動</td> 
   <td colspan="1">新增、更新、失敗的專案或已略過</td>
  </tr>  
  <tr> 
   <td colspan="1">推送新內容</td> 
   <td colspan="1">任務，電子郵件範本</td> 
   <td colspan="1">推送任務（活動）</td> 
   <td colspan="1"></td>
  </tr>
  <tr> 
   <td colspan="1">推送更新</td> 
   <td colspan="1">任務，電子郵件範本，人員，連絡人，行銷活動</td> 
   <td colspan="1">將更新推送到SFDC並刪除</td> 
   <td colspan="1">更新，失敗專案或略過</td>
  </tr>  
  <tr> 
   <td colspan="1">同步結構描述</td> 
   <td colspan="1">行銷活動成員，自訂物件，行銷活動，行銷活動成員狀態，任務，人員，機會，機會聯絡人角色，使用者</td> 
   <td colspan="1">同步不同物件的中繼資料，以決定要在下一個週期同步哪些新欄位</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">與程式同步</td> 
   <td colspan="1">行銷活動</td> 
   <td colspan="1">將Marketo方案與SFDC行銷活動同步</td> 
   <td colspan="1">新增、更新、失敗或略過</td>
  </tr> 
  <tr> 
   <td colspan="1">更新活動</td> 
   <td colspan="1">任務</td> 
   <td colspan="1">從Salesforce提取活動</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">更新FKS</td> 
   <td colspan="1">全部</td> 
   <td colspan="1">更新所有物件的外部索引鍵</td> 
   <td colspan="1">不適用</td>
  </tr>  
 </tbody> 
</table>

&#42;訂閱層級的品牌設定會決定標籤 — 報表中的「銷售機會」或「人員」。
