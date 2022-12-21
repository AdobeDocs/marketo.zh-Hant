---
unique-page-id: 10099102
description: Microsoft Dynamics MSI的外掛程式發行 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics MSI的外掛程式發行
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
source-git-commit: ff076d66a193664aa6ec05cf940143cebdd2d942
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 6%

---

# Microsoft Dynamics MSI的外掛程式發行 {#plug-in-releases-for-microsoft-dynamics-msi}

當您首次同步到Microsoft Dynamics時，請下載並安裝最新版本的Marketo Sales Insight(MSI)插件。 Marketo會定期更新這些外掛程式，讓您回到相同位置下載新版本。

如果您使用Marketo的原生CRM同步解決方案來同步Dynamics，請 [下載最新外掛程式](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)與您的Dynamics版本對應的{target=&quot;_blank&quot;}。 若是具有自訂同步功能且已購買Marketo Sales Insight的使用者， [包在此](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target=&quot;_blank&quot;}。

>[!NOTE]
>
>這些版本適用於內部部署和線上版本的Dynamics。

## 升級MSI解決方案 {#upgrading-your-msi-solution}

1. 匯入最新版本的解決方案 _在現有版本上_ ，按 **匯入** 按鈕。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>範例：如果您的Dynamics CRM有2.0.0.20版，而最新版本是2.0.0.21，您將匯入 _over_ 版本2.0.0.20。

1. 按一下 **下一個**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. 選擇 **升級階段** 和 **維護自定義**，然後按一下 **匯入**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. 按一下 **下一個**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. 成功導入後，您將看到兩個MSI解決方案：MarketoSalesInsight和MarketoSalesInsight_Upgrade。 選取舊版解決方案，然後按一下「套用解決方案升級」 。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

就這樣！ 升級後，您將只看到一個MSI解決方案。

## 版本更新 {#version-updates}

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
   <th colspan="1">備註</th> 
  </tr> 
  <tr> 
   <td colspan="1">02/03/22</td> 
   <td colspan="1">2.0.0.27</td> 
   <td colspan="1">前瞻分析的帳戶配置：有趣的時刻、分數變更、網路活動、電子郵件活動</td> 
  </tr>
  <tr> 
   <td colspan="1">01/05/22</td> 
   <td colspan="1">2.0.0.26</td> 
   <td colspan="1">傳送電子郵件的方案採用分數</td> 
  </tr>
  <tr> 
   <td colspan="1">10/28/21</td> 
   <td colspan="1">2.0.0.25</td> 
   <td colspan="1">產品採用分數量度，新的全域控制面板（網路活動、電子郵件、最佳賭注）</td> 
  </tr>
  <tr> 
   <td colspan="1">02/10/21</td> 
   <td colspan="1">2.0.0.22</td> 
   <td colspan="1">在MSI解決方案上刪除已啟用自動審核和文檔更改</td> 
  </tr>
  <tr> 
   <td colspan="1">10/01/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">錯誤修正：為具有Sales Insight角色的用戶分配對MSI API配置欄位的訪問</td> 
  </tr> 
  <tr> 
   <td colspan="1">07/20/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">錯誤修正：新增非同步記錄的驗證訊息</td> 
  </tr> 
  <tr> 
   <td colspan="1">06/12/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">錯誤修正：在MSD API配置上隱藏MSI密碼</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/26/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">錯誤修正：要更改顯示MSI按鈕的MSI角色ID驗證，請執行以下操作</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/21/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">錯誤修正：取消隱藏所有者欄位，並將欄位設為非必填欄位</td> 
  </tr> 
  <tr> 
   <td colspan="1">04/28/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">錯誤修正：移除MSD CRM Sitemap設定連結相依性</td> 
  </tr> 
 </tbody> 
</table>
