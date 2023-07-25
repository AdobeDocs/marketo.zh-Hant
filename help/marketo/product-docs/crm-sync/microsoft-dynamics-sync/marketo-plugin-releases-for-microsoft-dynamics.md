---
unique-page-id: 10099389
description: 適用於Microsoft Dynamics的Marketo外掛程式版本 — Marketo檔案 — 產品檔案
title: 適用於Microsoft Dynamics的Marketo外掛程式版本
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 7%

---

# 適用於Microsoft Dynamics的Marketo外掛程式版本 {#marketo-plugin-releases-for-microsoft-dynamics}

第一次同步至Microsoft Dynamics時，您會下載Marketo適用的外掛程式最新版本。 Marketo會定期更新這些外掛程式，讓您能夠返回相同位置下載新版本。

[下載最新的外掛程式](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 與您的Dynamics版本相對應。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## 更新您的Dynamics解決方案 {#updating-your-dynamics-solution}

1. 匯入最新版本的解決方案，以取代現有的Dynamics CRM版本(例如：如果您的Dynamics CRM版本為1.4，而最新版本為1.5，您便可以匯入 _超過_ 1.4版)。

1. 您將會看到下列快顯視窗。 選取 **更新** 和 **維護自訂**，然後按一下 **匯入**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## 最新版本 {#latest-versions}

>[!NOTE]
>
>這些版本適用於內部部署和線上版本的Dynamics。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">版本</th> 
   <th colspan="1">發行日期</th> 
   <th>備註</th> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.1.1</td> 
   <td colspan="1">02/04/21</td> 
   <td colspan="1">支援多選選項集欄位同步（此功能僅適用於V9.X及更高版本）。.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">新增對Campaign與MS Dynamics同步的支援。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">新增對立即可用的Microsoft Dynamics 9.x版潛在客戶連絡流程資格支援。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">錯誤修正：嘗試安裝適用於Dynamics 2013的Marketo解決方案時發生業務流程錯誤。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">9/29/17</td> 
   <td colspan="1">錯誤修正：內部修訂。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">錯誤修正：外掛程式未訂閱擷取自訂物件狀態變更的事件。 此修正專屬於Dynamics CRM On Premise 2011。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">錯誤修正：未完全擷取機會聯絡人角色的更新。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1"><p>錯誤修正：建立商機時，在marketo記錄檔中的customeropportunityrole上發現不必要的更新交易。 </p><p>錯誤修正：刪除customeropportunityrole實體時，會記錄額外的刪除交易。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">錯誤修正：非同步更新和刪除自訂物件。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">4/8/16</td> 
   <td colspan="1">錯誤修正：當銷售機會將同步篩選器設為「否」，而商機和聯絡人沒有同步篩選器時，當銷售機會符合資格時，系統不會為聯絡人和商機產生「建立記錄」。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>錯誤修正：關閉同步篩選器時會記錄「指派事件」。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">錯誤修正：客戶無法在CRM中建立銷售機會，因為登入使用者沒有Marketo Config許可權。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">錯誤修正：為一般Dynamics使用者建立存取限制，以解決安全性問題。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>錯誤修正： Dynamics中的更新未同步至Marketo的步驟和影像。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">錯誤修正：當同步篩選器設為false時，銷售機會記錄會同步至Marketo。</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[下載Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)
