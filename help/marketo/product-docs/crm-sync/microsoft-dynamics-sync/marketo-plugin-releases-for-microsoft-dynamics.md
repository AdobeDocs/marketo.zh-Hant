---
unique-page-id: 10099389
description: MarketoMicrosoftDynamics插件版本 — Marketo文檔 — 產品文檔
title: MarketoDynamics插件版本
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
source-git-commit: 1379fcbdc0a8673b1d6cb17a9d573d3625d5a1b8
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 7%

---

# MarketoDynamics插件版本 {#marketo-plugin-releases-for-microsoft-dynamics}

首次同步到MicrosoftDynamics時，將下載最新版本的Marketo插件。 Marketo會定期更新這些插件，以便您可以返回到同一位置下載新版本。

[下載最新插件](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 與Dynamics版本對應。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## 更新Dynamics解決方案 {#updating-your-dynamics-solution}

1. 將解決方案的最新版本導入到Dynamics CRM的現有版本(例如：如果您的Dynamics CRM有1.4版，且最新版本為1.5版，您將導入 _超_ 版本1.4)。

1. 您將看到以下彈出窗口。 選擇 **更新** 和 **維護自定義**，然後按一下 **導入**。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## 最新版本 {#latest-versions}

>[!NOTE]
>
>這些版本適用於Dynamics的內部版本和線上版本。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">版本</th> 
   <th colspan="1">發佈日期</th> 
   <th>注釋</th> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.1.1</td> 
   <td colspan="1">02/04/21</td> 
   <td colspan="1">支援多選選項集欄位同步（此功能僅適用於V9.X及更高版本）。。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">已添加對與MS Dynamics進行市場活動同步的支援。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">增加了對開箱即用資格的支援，導致MicrosoftDynamics 9.x版的聯繫流程。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">錯誤修復：嘗試安裝MarketoDynamics 2013解決方案時出現業務流程錯誤。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">9/29/17</td> 
   <td colspan="1">錯誤修復：內部修訂。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">錯誤修復：插件未訂閱捕獲自定義對象狀態更改的事件。 此修復程式特定於Dynamics CRM On Premise 2011。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">錯誤修復：未完全捕獲機會聯繫人角色的更新。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1"><p>錯誤修復：在建立商機時，會注意到marketo日誌中客戶機會角色的不必要更新事務。 </p><p>錯誤修復：刪除客戶機會角色實體時記錄了額外的刪除事務。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">錯誤修復：已使自定義對象的更新和刪除非同步。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">4/8/16</td> 
   <td colspan="1">錯誤修復：當潛在顧客的同步篩選器設定為NO，並且業務機會和聯繫人沒有同步篩選器時，在潛在顧客獲得資格時，不會為聯繫人和業務機會生成建立日誌。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>錯誤修復：關閉同步篩選器時記錄了分配事件。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">錯誤修復：客戶無法在CRM中建立潛在客戶，因為登錄用戶沒有Marketo配置權限。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">錯誤修復：為普通Dynamics用戶建立了訪問限制，以解決安全問題。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>錯誤修復：Dynamics中的更新未同步到Marketo以獲取步驟和映像。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">錯誤修復：當同步篩選器設定為false時，潛在客戶記錄正在同步到Marketo。</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[下載Marketo銷售線索管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)
