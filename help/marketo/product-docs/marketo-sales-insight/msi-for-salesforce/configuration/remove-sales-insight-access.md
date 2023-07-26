---
description: 移除銷售分析存取權 — Marketo檔案 — 產品檔案
title: 移除Sales Insight存取權
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# 移除Sales Insight存取權 {#remove-sales-insight-access}

使用以下步驟，移除對Salesforce中Sales Insight功能的存取權。 適用於Salesforce Classic和Lightning。

## 概觀 {#overview}

存取所有Sales Insight功能需要下列物件、Apex類別和Visualforce頁面的許可權。 移除這些專案將會移除Sales Insight的存取權。

**物件設定**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>最佳化檢視詳細資料</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>最佳化檢視</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>InterestedMentsCache</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>Marketo銷售分析設定</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>評分快取</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>值</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>WebActivityCache</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
 </tbody> 
</table>

* Apex類別存取：以「mkto_si」開頭的159個Apex類別
* Visualforce頁面存取：64個以「mkto_si」開頭的Visualforce頁面
* 自訂設定定義：mkto_si.Marketo設定和mkto_si.User偏好設定

## 移除Sales Insight的存取權 {#removing-access-to-sales-insight}

1. 登入您的Salesforce帳戶。

1. 按一下 **設定**.

   ![](assets/remove-sales-insight-access-1.png)

1. 在「管理員」底下，按一下 **管理使用者**，然後 **設定檔**.

1. 按一下您要更新的設定檔，然後 **編輯**.

1. 向下捲動至「標籤設定」下的「自訂標籤設定」。

1. 從Marketo Sales Insight Config和MSI Marketo Sales Outbox的下拉式清單中選取「Tab Hidden」選項。

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. 向下捲動至「自訂物件許可權」。

1. 移除下列物件的「讀取、建立、編輯、刪除」存取權：

   * BestBetsCache
   * 最佳化檢視詳細資料
   * 最佳化檢視
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestedMentsCache
   * Marketo銷售分析設定
   * 評分快取
   * 值
   * WebActivityCache

1. 向下捲動至「已啟用的Apex類別存取」區段。 按一下 **編輯**.

1. 從「啟用的Apex類別」段落中，選取所有以「mkto_si」開頭的類別。 這最多可新增159個類別。

1. 按一下 **移除**，然後 **儲存**.

   ![](assets/remove-sales-insight-access-4.png)

1. 向下捲動至「已啟用的Visualforce頁面存取」區段。 按一下 **編輯**.

1. 從「已啟用的Visualforce頁面」區段中，選取所有以「mkto_si」開頭的頁面。 最多可新增64頁。

1. 按一下 **移除**，然後 **儲存**.

   ![](assets/remove-sales-insight-access-5.png)

1. 向下捲動至「已啟用自訂設定定義存取」區段。 按一下 **編輯**.

1. 選取「Marketo Sales Insight.mkto_si.Marketo設定」和「Marketo Sales Insight.mkto_si.User偏好設定」。

1. 按一下 **移除**，然後 **儲存**.

   ![](assets/remove-sales-insight-access-6.png)

完成了！ 您已成功移除銷售分析存取權。 對您要移除其存取權的任何其他設定檔重複相同的步驟。
