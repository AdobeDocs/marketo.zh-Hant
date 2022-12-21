---
unique-page-id: 10099389
description: Marketo Dynamics外掛程式發行 — Marketo檔案 — 產品檔案
title: Marketo Dynamics外掛程式版本
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
source-git-commit: 1379fcbdc0a8673b1d6cb17a9d573d3625d5a1b8
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 7%

---

# Marketo Dynamics外掛程式版本 {#marketo-plugin-releases-for-microsoft-dynamics}

第一次同步至Microsoft Dynamics時，請下載最新版的Marketo外掛程式。 Marketo會定期更新這些外掛程式，讓您回到相同位置下載新版本。

[下載最新外掛程式](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 對應至您的Dynamics版本。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## 更新Dynamics解決方案 {#updating-your-dynamics-solution}

1. 將最新版本的解決方案匯入至您的Dynamics CRM的現有版本(例如：如果您的Dynamics CRM有1.4版，而最新版本是1.5版，您將匯入 _over_ 1.4版)。

1. 您會看到下列快顯視窗。 選擇 **更新** 和 **維護自定義**，然後按一下 **匯入**.

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
   <td colspan="1">新增支援MS Dynamics的促銷活動同步。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">新增對符合現成可用資格的支援，進而導致Microsoft Dynamics 9.x版的聯絡程式。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">錯誤修正：嘗試安裝Dynamics 2013適用的Marketo解決方案時發生業務流程錯誤。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">9/29/17</td> 
   <td colspan="1">錯誤修正：內部修訂。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">錯誤修正：外掛程式未訂閱擷取自訂物件之狀態變更的事件。 此修正專供Dynamics CRM On Premise 2011使用。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">錯誤修正：未完全捕獲機會聯繫人角色的更新。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1"><p>錯誤修正：建立商機時，會注意到marketo記錄中customerpocityrole的不必要更新交易。 </p><p>錯誤修正：刪除customerportityrole實體時記錄了額外的刪除事務。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">錯誤修正：將自訂物件的更新和刪除設為非同步。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">4/8/16</td> 
   <td colspan="1">錯誤修正：當銷售機會的同步篩選器設定為NO，並且銷售機會和聯繫人沒有同步篩選器時，銷售機會合格時，系統不會為聯繫人和業務機會生成建立日誌。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>錯誤修正：同步篩選器關閉時，會記錄「指派事件」。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">錯誤修正：由於登入使用者沒有Marketo設定權限，客戶無法在CRM中建立銷售機會。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">錯誤修正：為一般Dynamics使用者建立存取限制，以解決安全性疑慮。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>錯誤修正：Dynamics中的更新未同步至Marketo以取得步驟和影像。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">錯誤修正：同步篩選器設為false時，銷售機會記錄正在同步至Marketo。</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[下載Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)
