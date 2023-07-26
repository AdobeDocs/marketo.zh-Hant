---
unique-page-id: 15695924
description: 帳戶分析排名和調整 — Marketo檔案 — 產品檔案
title: 帳戶設定檔排名與調整
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# 帳戶設定檔排名與調整 {#account-profiling-ranking-and-tuning}

帳戶設定檔會識別您的理想客戶設定檔(ICP)、根據ICP對資料庫中的公司進行排名，並將ICP指標資料新增至升級為具名帳戶的帳戶。

## 模型結果 {#model-results}

結果會顯示您所有依等級劃分的已知科目。 A是最高等級，D是最低等級。

![](assets/results.png)

雖然這是選擇性的，但建議您選取「自動提升」核取方塊，因為這樣可為您節省大量時間。 不過，如果您想逐一瀏覽每個帳戶和 [手動新增](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts)，只要取消勾選此方塊即可。

<table> 
 <tbody> 
  <tr> 
   <td><strong>排名</strong></td> 
   <td> 
    <div>
      根據理想客戶設定檔的帳戶排名。 A代表最適合，D代表最不適合。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>傾向</strong></td> 
   <td> 
    <div>
      與非ICP型帳戶選擇相比，轉換率的預估增加。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>帳戶 (%)</strong></td> 
   <td> 
    <div>
      模型輸入中具有此排名的帳戶百分比。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>模型基準的%</strong></td> 
   <td> 
    <div>
      模型基準中擁有此等級的帳戶百分比。 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## 模型調整 {#model-tuning}

在「模型」標籤中，按一下「調整模型」按鈕。

![](assets/two.png)

有數個標籤可供選擇，允許深入自訂。

![](assets/tuning-page.png)

**指標類別**

<table> 
 <tbody> 
  <tr> 
   <td><strong>合規性</strong></td> 
   <td> 
    <div>
      認證、合規性相關職位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>作業</strong></td> 
   <td> 
    <div>
      與作業相關的職位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>小時</strong></td> 
   <td> 
    <div>
      HR或薪資軟體、與HR相關的職位/聘用。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>工程</strong></td> 
   <td> 
    <div>
      技術、架構、工程相關職位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>銷售</strong></td> 
   <td> 
    <div>
      適用於銷售、銷售相關職位/聘用的解決方案與軟體。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>方法</strong></td> 
   <td> 
    <div>
      意圖指示器。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      硬體與軟體解決方案、技術、IT相關職位/聘用。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>財務</strong></td> 
   <td> 
    <div>
      財務軟體、財務相關職位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>行銷</strong></td> 
   <td> 
    <div>
      行銷技術與軟體、行銷相關職位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>企業</strong></td> 
   <td> 
    <div>
      Forbes或Inc的上市或商業合作關係。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>客戶體驗與關係</strong></td> 
   <td> 
    <div>
      客戶成功與客戶關係職位/聘用。
    </div></td> 
  </tr> 
 </tbody> 
</table>

將滑鼠停留在工具提示上，即可檢視每欄的說明。

![](assets/tool-tip.png)

按一下新增ICP指標下拉式清單，將其他指標插入模型。

![](assets/add-icp.png)

勾選「匯出」方塊可讓您在「具名帳戶詳細資訊」頁面上檢視ICP指示器，以及在中使用選取的ICP指示器作為限制 [具名帳戶篩選器](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>ICP指示器作為限制包含在 **具名帳戶的成員** 篩選器和觸發器。

指標權重是控制每個指標在模型中接收的重要性層級。

![](assets/weightage.png)

按一下「重新整理模型」以使這些變更生效。

![](assets/refresh-button.png)

當您完成模型調整（重新整理模型後），請返回「模型結果」標籤並按一下 **儲存並套用排名**.

![](assets/ranks.png)
