---
unique-page-id: 10099102
description: Microsoft Dynamics MSI的增效模組版本——行銷檔案——產品檔案
title: Microsoft Dynamics MSI的增效模組版本
translation-type: tm+mt
source-git-commit: d1d74e24c07578b1b0c2696c08fe5a5be543cce8
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 4%

---


# Microsoft Dynamics MSI的增效模組版本{#plug-in-releases-for-microsoft-dynamics-msi}

當您第一次同步至Microsoft Dynamics時，請下載並安裝Marketo Sales Insight(MSI)的最新版本外掛程式。 Marketo會定期更新這些外掛程式，讓您回到相同位置下載新版本。

請[下載與Dynamics版本對應的最新外掛程式](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)。

>[!NOTE]
>
>這些版本適用於內部部署版本和線上版本的Dynamics。

## 升級您的MSI解決方案{#upgrading-your-msi-solution}

1. 按Dynamics中的&#x200B;**匯入**&#x200B;按鈕，將解決方案的最新版本匯入至Dynamics CRM的現有版本&#x200B;_。_

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>範例：如果您的Dynamics CRM有2.0.0.20版，而最新版本為2.0.0.21，您將匯入&#x200B;_over_ 2.0.0.20版。

1. 按一下&#x200B;**Next**。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. 選擇&#x200B;**升級階段**&#x200B;和&#x200B;**維護自定義**，然後按一下&#x200B;**導入**。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. 按一下&#x200B;**Next**。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. 成功匯入後，您會看到兩個MSI解決方案：MarketoSalesInsight和MarketoSalesInsight_Upgrade。 選取舊版解決方案，然後按一下「套用解決方案升級」。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

就這樣！ 升級後，您只會看到一個MSI解決方案。

## 版本更新{#version-updates}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">發行日期</th> 
   <th colspan="1">版本</th> 
   <th colspan="1">附註</th> 
  </tr> 
  <tr> 
   <td colspan="1">10/1/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">錯誤修正：為具有Sales Insight角色的使用者指派對MSI API設定欄位的存取權</td> 
  </tr> 
  <tr> 
   <td colspan="1">07/20/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">錯誤修正：新增非同步記錄的驗證訊息</td> 
  </tr> 
  <tr> 
   <td colspan="1">06/12/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">錯誤修正：在MSD API配置中隱藏MSI密碼</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/26/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">錯誤修正：若要變更顯示MSI按鈕的MSI角色ID驗證</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/21/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">錯誤修正：取消隱藏擁有者欄位，並讓欄位非必填</td> 
  </tr> 
  <tr> 
   <td colspan="1">04/28/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">錯誤修正：刪除MSD CRM站點地圖設定連結相關性</td> 
  </tr> 
 </tbody> 
</table>
