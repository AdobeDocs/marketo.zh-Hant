---
unique-page-id: 15695924
description: 帳戶分析排名和調整 — Marketo檔案 — 產品檔案
title: 帳戶分析排名和調整
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# 帳戶分析排名和調整 {#account-profiling-ranking-and-tuning}

「帳戶配置檔案」可確定您的理想客戶配置檔案(ICP)，根據ICP對資料庫中的公司進行排名，並將ICP指標資料添加到以「指定帳戶」促銷的帳戶。

## 模型結果 {#model-results}

結果會顯示依等級劃分的所有已知帳戶。 A是最高等級，D是最低。

![](assets/results.png)

若為選用項目，建議您選取「自動促銷」核取方塊，因為這可為您節省大量時間。 不過，如果您想要瀏覽每個帳戶和 [手動新增](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts)，只要取消勾選方塊即可。

<table> 
 <tbody> 
  <tr> 
   <td><strong>排名</strong></td> 
   <td> 
    <div>
      根據理想客戶設定檔的帳戶排名。 A最合適，D最不合適。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>傾向</strong></td> 
   <td> 
    <div>
      與非基於比較方案的賬戶選擇相比，轉換率的估計增加。 
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
   <td><strong>模型基準百分比</strong></td> 
   <td> 
    <div>
      模型基礎中具有此排名的帳戶百分比。 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## 模型調整 {#model-tuning}

在「模型」(Model)頁簽中，按一下「調整模型」(Tune Model)按鈕。

![](assets/two.png)

有數個索引標籤可供選擇，以進行深入自訂。

![](assets/tuning-page.png)

**指標類別**

<table> 
 <tbody> 
  <tr> 
   <td><strong>合規性</strong></td> 
   <td> 
    <div>
      認證、與法規遵從性相關的職位/招聘。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>操作</strong></td> 
   <td> 
    <div>
      與業務有關的職位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>HR</strong></td> 
   <td> 
    <div>
      HR或工資單軟體，與HR相關的職位/聘用。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>工程</strong></td> 
   <td> 
    <div>
      技術、框架、與工程有關的職位/雇用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>銷售</strong></td> 
   <td> 
    <div>
      用於銷售、銷售相關職位/招聘的解決方案和軟體。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>目的</strong></td> 
   <td> 
    <div>
      意圖指標。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      硬體和軟體解決方案、技術、與IT相關的職位/招聘。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>金融</strong></td> 
   <td> 
    <div>
      財務軟體、財務相關職位/雇用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>行銷</strong></td> 
   <td> 
    <div>
      市場營銷技術和軟體、與市場營銷相關的職位/招聘。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>企業</strong></td> 
   <td> 
    <div>
      《福布斯》或《公司》的上市或商業合作。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>客戶體驗與關係</strong></td> 
   <td> 
    <div>
      客戶成功和客戶關係職位/雇用。
    </div></td> 
  </tr> 
 </tbody> 
</table>

將滑鼠指標暫留在工具提示上，即可取得每欄的說明。

![](assets/tool-tip.png)

按一下「添加ICP指示器」(Add ICP Indicator)下拉清單，將其他指示器插入模型中。

![](assets/add-icp.png)

勾選「匯出」方塊，即可在「指定帳戶」詳細資訊頁面上查看ICP指標，並將選取的ICP指標用作 [名稱帳戶篩選器](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>比較方案指標列為 **指定帳戶的成員** 篩選器和觸發器。

指標權重是控制每個指標在模型中所接收重要性的級別。

![](assets/weightage.png)

按一下「刷新模型」(Refresh Model)，使這些更改生效。

![](assets/refresh-button.png)

完成模型調整後（刷新模型後），返回「模型結果」(Model Results)頁簽，然後按一下 **儲存並套用排名**.

![](assets/ranks.png)
