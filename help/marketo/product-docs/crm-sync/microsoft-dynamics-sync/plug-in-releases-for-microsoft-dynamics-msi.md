---
unique-page-id: 10099102
description: Microsoft Dynamics MSI的外掛程式版本 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics MSI的外掛程式版本
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 6dcda9b86555c17b3492a02f3985db7d2acd8a32
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---

# Microsoft Dynamics MSI的外掛程式版本 {#plug-in-releases-for-microsoft-dynamics-msi}

當您首次同步至Microsoft Dynamics時，需下載並安裝Marketo Sales Insight (MSI)適用的最新版外掛程式。 請定期Marketo Engage更新這些外掛程式，以便您可以返回相同位置下載新版本。

如果您使用Marketo原生CRM同步解決方案至Dynamics，請 [下載最新的外掛程式](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"} corresponding to your Dynamics release. For those who have a custom sync and have purchased Marketo Sales Insight, the [package is here](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.

>[!NOTE]
>
>這些版本適用於Dynamics的內部部署和線上版本。

## 升級MSI解決方案 {#upgrading-your-msi-solution}

1. 匯入最新版本的解決方案 _超過現有版本_ 的CRM，方法是按下 **[!UICONTROL 匯入]** Dynamics中的按鈕。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>範例：如果您的Dynamics CRM版本為2.0.0.20，而最新版本為2.0.0.21，則需匯入 _超過_ 版本2.0.0.20。

1. 按一下 **[!UICONTROL 下一個]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. 選取 **[!UICONTROL 暫存升級]** 和 **[!UICONTROL 維護自訂]**，然後按一下 **[!UICONTROL 匯入]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. 按一下 **[!UICONTROL 下一個]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. 成功匯入後，您將會看到兩個MSI解決方案：MarketoSalesInsight和MarketoSalesInsight_Upgrade。 選取較舊的解決方案，然後按一下Apply Solution Upgrade。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

就是這樣！ 升級之後，您只會看到一個MSI解決方案。

## 版本更新 {#version-updates}

<table> 
 <tbody> 
  <tr> 
   <th>發行日期</th> 
   <th>版本</th> 
   <th>附註</th> 
  </tr>
  <tr> 
   <td>02/14/24</td> 
   <td>2.00.31</td> 
   <td>變更匿名網路活動的分頁。
   <p>
   從使用者檢視中加密機密金鑰資訊。 匯入新封裝後需要變更密碼才能進行加密。</td> 
  </tr>
  <tr> 
   <td>10/18/23</td> 
   <td>2.00.30</td> 
   <td>合併MSI錯誤記錄檔並移除資訊通知，使其不顯示在Marketo錯誤實體上。</td> 
  </tr>
  <tr> 
   <td>05/19/23</td> 
   <td>2.00.29</td> 
   <td>修正全域控制面板的網頁活動和興趣時刻分頁問題。</td> 
  </tr>
  <tr> 
   <td>03/23/23</td> 
   <td>2.00.28</td> 
   <td>已建立 <a href="https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip">新封裝</a> 用於MSI，以連線到CRM。</td> 
  </tr>
  <tr> 
   <td>02/03/22</td> 
   <td>2.0.0.27</td> 
   <td>前瞻分析的帳戶配置：有趣的時刻、分數變更、網頁活動、電子郵件活動。</td> 
  </tr>
  <tr> 
   <td>01/05/22</td> 
   <td>2.0.0.26</td> 
   <td>傳送電子郵件的方案採用分數。</td> 
  </tr>
  <tr> 
   <td>10/28/21</td> 
   <td>2.0.0.25</td> 
   <td>產品採用分數量度、新的全域控制面板（網頁活動、電子郵件、首選）。</td> 
  </tr>
  <tr> 
   <td>02/10/21</td> 
   <td>2.0.0.22</td> 
   <td>移除MSI解決方案上已啟用自動稽核和檔案變更。</td> 
  </tr>
  <tr> 
   <td>10/01/20</td> 
   <td>2.0.0.21</td> 
   <td>錯誤修正：為具有Sales Insight角色的使用者指派對MSI API設定欄位的存取權。</td> 
  </tr> 
  <tr> 
   <td>07/20/20</td> 
   <td>2.0.0.20</td> 
   <td>錯誤修正：新增非同步記錄的驗證訊息。</td> 
  </tr> 
  <tr> 
   <td>06/12/20</td> 
   <td>2.0.0.19</td> 
   <td>錯誤修正：在MSD API設定上隱藏MSI秘密密碼。</td> 
  </tr> 
  <tr> 
   <td>05/26/20</td> 
   <td>2.0.0.18</td> 
   <td>錯誤修正：變更顯示MSI按鈕的MSI角色ID驗證。</td> 
  </tr> 
  <tr> 
   <td>05/21/20</td> 
   <td>2.0.0.17</td> 
   <td>錯誤修正：取消隱藏擁有者欄位，並將欄位設為非必填。</td> 
  </tr> 
  <tr> 
   <td>04/28/20</td> 
   <td>2.0.0.16</td> 
   <td>錯誤修正：正在移除MSD CRM Sitemap設定連結相依性。</td> 
  </tr> 
 </tbody> 
</table>
