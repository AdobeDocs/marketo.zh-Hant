---
unique-page-id: 7504238
description: Google Universal Analytics中的自訂RTP儀表板——行銷檔案——產品檔案
title: Google Universal Analytics中的自訂RTP儀表板
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---


# Google Universal Analytics中的自訂RTP儀表板{#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[將RTP與Google Universal Analytics整合](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

此貼文說明如何在Google Universal Analytics(GUA)中設定RTP儀表板。 從RTP傳送至GUA的資料可以設定為兩個獨立的自訂控制面板，稱為：

* RTP B2B
* RTP參與

## 設定自訂控制面板{#setting-up-a-custom-dashboard}

1. 登入Google Analytics。 按一下頂部菜單中的&#x200B;**報告**。 按一下「**控制面板**&#x200B;和&#x200B;**+新自訂控制面板**」。

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. 選擇&#x200B;**空白畫布**，新增&#x200B;**控制面板名稱**，然後按一下「建立控制面板&#x200B;**」。**

1. 按一下「新增介面工具集」，以建立新介面工具集。****

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## RTP B2B儀表板{#rtp-b-b-dashboard}

此儀表板可讓使用者從B2B的角度分析其網站效能。

它可依產業、收入、規模、帳戶型清單和目標區段提供造訪來源和站上行為等資訊。

控制面板由3欄組成

* 流量來源
* 區段
* Firmographic向下切入

1. 建立名為&#x200B;**RTP B2B儀表板**&#x200B;的新儀表板，並定義以下Widget:

![](assets/image2015-3-22-16-3a50-3a3.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      欄1 —— 流量來源
    </div></th> 
   <th> 
    <div> <strong>欄2 —— 區段</strong> 
    </div></th> 
   <th> 
    <div> <strong>Column 3 - Firmographic向下鑽取</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>名稱：依區段和頻道的作業</li> 
     <li>介面工具集類型：列<br></li> 
     <li>建立長條圖，其中顯示：會話</li> 
     <li>分組依據：事件標籤</li> 
     <li>透視方式：預設渠道群組</li> 
     <li>篩選：<br>僅顯示 |事件類別（包含）RTP-區段</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名稱：RTP分段用戶數</li> 
     <li>類型：2.1量度</li> 
     <li>顯示下列量度：使用者<br></li> 
     <li>篩選：<br>僅顯示 |事件類別（包含）RTP-區段</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名稱：各產業研討會</li> 
     <li>類型：派<br></li> 
     <li>建立圓形圖，其中顯示：會話</li> 
     <li>分組依據：RTP-Industry</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>名稱：依產業和通道的研討會</strong></li> 
     <li><strong>介面工具集類型：列</strong></li> 
     <li><strong>建立長條圖，其中顯示：會話</strong></li> 
     <li><strong>分組依據：RTP-Industry</strong></li> 
     <li><strong>透視方式：預設渠道群組</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>名稱：依國家區分的會議</strong></li> 
     <li><strong>類型：Geomap</strong></li> 
     <li><strong>繪製選取的量度：國家／地區 |工作階段</strong></li> 
     <li><strong>選擇地區：世界</strong></li> 
     <li><strong>篩選：僅顯示 |事件類別（包含）RTP-區段</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>名稱：按RTP類別的會話</strong></li> 
     <li><strong>類型：派</strong></li> 
     <li><strong>建立圓形圖，其中顯示：會話</strong></li> 
     <li><strong>分組依據：RTP類別</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>名稱：頂層目標區段</li> 
     <li>類型：列</li> 
     <li>建立長條圖，其中顯示：使用者</li> 
     <li>分組依據：事件動作</li> 
     <li>篩選：僅顯示 |事件類別（包含）RTP-區段</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>名稱：按RTP組的會話</li> 
     <li>類型：列<br></li> 
     <li>建立長條圖，其中顯示：會話</li> 
     <li>分組依據：RTP組</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>名稱：依熱門細分的工作階段和目標</li> 
     <li>類型：表格<br></li> 
     <li>顯示下列欄：<br>事件標籤 |工作階段 |目標轉換率</li> 
     <li>篩選：<br>僅顯示 |事件類別（包含）RTP-區段</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## RTP參與儀表板{#rtp-engagement-dashboard}

此控制面板可讓使用者分析其RTP促銷活動效能和建議引擎參與。 它提供平均值的比較 會話持續時間和每個會話的頁數介於：

* 未參與
* 參與（個人化促銷活動的曝光和點按）
* 點按建議引擎和主要建議內容

建立名為&#x200B;**RTP參與儀表板**&#x200B;的新儀表板，並定義下列Widget:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>第1欄促銷活動曝光度</strong> 
    </div></th> 
   <th> 
    <div> <strong>欄2促銷活動點進</strong> 
    </div></th> 
   <th> 
    <div> <strong>第3欄建議引擎</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>名稱：<strong>CTA（參與）總計</strong></li> 
     <li>類型：<strong>2.1量度</strong></li> 
     <li>顯示下列量度：<strong>事件總數</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（包含）:RTP-Campaigns</strong><br><strong>[僅顯示]事件操作（完全匹配）:曝光</strong><strong>[不顯示]事件標籤（包含）:#</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>名稱：<strong>總CTA（點進）</strong></li> 
     <li>類型：<strong>2.1量度</strong></li> 
     <li>顯示下列量度：<strong>事件總數</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（包含）:RTP-Campaigns</strong><br><strong>[僅顯示]事件操作（完全匹配）:點按</strong><strong>[不顯示]事件標籤（包含）:#</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>名稱：<strong>CRE —— 點按總次數</strong></li> 
     <li>類型：<strong>2.1量度</strong><br></li> 
     <li>顯示下列量度：<strong>Pageviews</strong></li> 
     <li>篩選：<strong>[only show]頁（包含）:rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>名稱：<strong>平均 會話持續時間（參與）</strong></li> 
     <li>類型：<strong>2.1量度</strong></li> 
     <li>顯示下列量度：<strong>平均 會話持續時間</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（完全符合）:RTP-Campaigns</strong><br><strong>[僅顯示]事件操作（完全匹配）:印象</strong><strong>[不顯示]事件標籤（包含）:#</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>名稱：<strong>平均 會話持續時間（點進）</strong></li> 
     <li>類型：<strong>2.1量度</strong></li> 
     <li>顯示下列量度：<strong>平均 會話持續時間</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（完全符合）:RTP-Campaigns</strong><br><strong>[僅顯示]事件操作（完全匹配）:clicks</strong><strong>[不顯示]事件標籤（包含）:#</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>名稱：<strong>CRE —— 主要建議內容</strong></li> 
     <li>類型：<strong>表</strong><br></li> 
     <li>顯示下列欄：<br><strong>頁面標題 | Pageviews</strong><br></li> 
     <li>篩選器：<br>篩選器：<strong>[only show]頁（包含）:rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>名稱：<strong>頁面／工作階段（參與）</strong></li> 
     <li>類型：<strong>2.1量度</strong></li> 
     <li>顯示下列量度：<strong>頁／會話</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（完全符合）:RTP-Campaigns</strong></li> 
     <li><strong>[僅顯示]事件操作（完全匹配）:印象</strong></li> 
     <li><strong>[不顯示]事件標籤（包含）:#</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名稱：<strong>頁面／工作階段（點進）</strong></li> 
     <li>類型：<strong>2.1量度</strong></li> 
     <li>顯示下列量度：<strong>頁／會話</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（完全符合）:RTP-Campaigns</strong></li> 
     <li><strong>[僅顯示]事件操作（完全匹配）:點擊</strong></li> 
     <li><strong>[不顯示]事件標籤（包含）:#</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>名稱：<strong>CTA</strong>曝光次數</li> 
     <li>類型：<strong>表</strong></li> 
     <li>顯示下列欄：<strong>事件標籤 |事件總數 |用戶</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（完全符合）:RTP-Campaigns</strong><br><strong>[僅顯示]事件操作（完全匹配）:印象</strong><strong>[不顯示]事件標籤（包含）:#</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名稱：<strong>點進，由CTA</strong></li> 
     <li>類型：<strong>表</strong></li> 
     <li>顯示下列欄：<strong>事件標籤 |事件總數 |用戶</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（完全符合）:RTP-Campaigns</strong><br><strong>[僅顯示]事件操作（完全匹配）:clicks&lt;a3/</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[將RTP與Google Universal Analytics整合](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Google Universal Analytics中的自訂RTP報表](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
