---
unique-page-id: 10099389
description: 適用於Marketo Dynamics的Microsoft外掛程式版本 — Marketo檔案 — 產品檔案
title: 適用於Microsoft Dynamics的Marketo外掛程式版本
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: f1fd9564abe4702c3a124442ee26027d4d22f23d
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# 適用於Microsoft Dynamics的Marketo外掛程式版本 {#marketo-plugin-releases-for-microsoft-dynamics}

當您首次同步至Microsoft Dynamics時，需下載最新版的Marketo外掛程式。 Marketo會定期更新這些外掛程式，讓您能夠返回相同位置下載新版本。

[下載與您的Dynamics版本對應的最新外掛程式](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## 正在更新您的Dynamics解決方案 {#updating-your-dynamics-solution}

1. 匯入最新版本的解決方案，以取代現有的Dynamics CRM版本（例如：如果您的Dynamics CRM版本為1.4，而最新版本為1.5，則您會匯入&#x200B;_超過_&#x200B;版本1.4）。

1. 您會看到下列快顯視窗。 選取&#x200B;**更新**&#x200B;和&#x200B;**維護自訂**，然後按一下&#x200B;**匯入**。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## 最新版本 {#latest-versions}

>[!NOTE]
>
>這些版本適用於Dynamics的內部部署和線上版本。

<table> 
 <tbody> 
  <tr> 
   <th style="width:15%">版本</th> 
   <th style="width:20%">發行日期</th> 
   <th style="width:65%">附註</th> 
  </tr>
  <tr> 
   <td>5.0.2.1</td> 
   <td>1/19/24</td> 
   <td>錯誤修正：修正與自訂實體同步相關的錯誤。</td> 
  </tr> 
  <tr> 
   <td>5.0.2.0</td> 
   <td>03/24/23</td> 
   <td>錯誤修正：修正無法在MS Dynamics上合併連絡人的錯誤。</td> 
  </tr> 
  <tr> 
   <td>5.0.1.8</td> 
   <td>03/27/23</td> 
   <td>錯誤修正：防止外掛程式覆寫MS Dynamics中UI元素的其他自訂。
   <p>
   錯誤修正：恢復5.0.1.1中遺失的導覽圖磚。</td> 
  </tr> 
  <tr> 
   <td>5.0.1.1</td> 
   <td>02/04/21</td> 
   <td>支援多選選項集欄位同步（此功能僅適用於V9.X及更高版本）。</td> 
  </tr> 
  <tr> 
   <td>4.2.0.0</td> 
   <td>10/16/20</td> 
   <td>新增與MS Dynamics同步Campaign的支援。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.24</td> 
   <td>8/22/18</td> 
   <td>新增立即可用的支援，讓銷售機會符合Microsoft Dynamics 9.x版的聯絡流程。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.23</td> 
   <td>6/27/18</td> 
   <td>錯誤修正：嘗試安裝適用於Dynamics 2013的Marketo解決方案時發生業務流程錯誤。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.22</td> 
   <td>9/29/17</td> 
   <td>錯誤修正：內部修訂。</td> 
  </tr> 
  <tr> 
   <td><p>4.0.0.21</p></td> 
   <td>11/9/16</td> 
   <td>錯誤修正：外掛程式未訂閱擷取自訂物件狀態變更的事件。 此修正專屬於Dynamics CRM On Premise 2011。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.20</td> 
   <td>7/22/16</td> 
   <td>錯誤修正：未完整擷取機會聯絡人角色的更新。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.19</td> 
   <td>6/28/16</td> 
   <td>錯誤修正：建立商機時，在marketo記錄檔的customeropportunityrole上發現不必要的更新交易。<p>錯誤修正：刪除customeropportunityrole實體時，會記錄額外的刪除交易。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.18</td> 
   <td>5/31/16</td> 
   <td>錯誤修正：非同步更新和刪除自訂物件。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.17</td> 
   <td>4/8/16</td> 
   <td>錯誤修正：當銷售機會將同步篩選器設為「否」，且商機和聯絡人沒有同步篩選器時，當銷售機會符合資格時，將不會為聯絡人和商機產生「建立記錄」。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.16</td> 
   <td>3/29/16</td> 
   <td>錯誤修正：當關閉同步篩選器時，會記錄「指派事件」 。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.15</td> 
   <td>3/3/16</td> 
   <td>錯誤修正：客戶無法在CRM中建立銷售機會，因為登入使用者沒有Marketo設定許可權。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.14</td> 
   <td>1/18/16</td> 
   <td>錯誤修正：為一般Dynamics使用者建立存取限制，以解決安全性問題。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.13</td> 
   <td>12/30/15</td> 
   <td>錯誤修正： Dynamics中的更新未同步至Marketo的步驟和影像。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.12</td> 
   <td>11/12/15</td> 
   <td>錯誤修正：當同步篩選器設為false時，潛在客戶記錄正同步至Marketo。</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[下載Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
