---
unique-page-id: 7504238
description: Google Universal Analytics中的自訂RTP儀表板 — Marketo檔案 — 產品檔案
title: Google Universal Analytics中的自訂RTP儀表板
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Google Universal Analytics中的自訂RTP儀表板 {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[整合RTP與Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

本文說明如何在Google Universal Analytics (GUA)中設定RTP儀表板。 從RTP傳送到GUA的資料可以設定為兩個單獨的自訂儀表板，稱為：

* RTP B2B
* RTP參與

## 設定自訂儀表板 {#setting-up-a-custom-dashboard}

1. 登入Google Analytics。 按一下頂端功能表中的&#x200B;**[!UICONTROL Reporting]**。 按一下&#x200B;**[!UICONTROL Dashboards]**&#x200B;和&#x200B;**[!UICONTROL New Dashboard]**。

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. 選取&#x200B;**空白畫布**，新增&#x200B;**儀表板名稱**，然後按一下&#x200B;**[!UICONTROL Create Dashboard]**。

1. 按一下&#x200B;**[!UICONTROL Add Widget]**&#x200B;以建立新的Widget。

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## RTP B2B控制面板 {#rtp-b-b-dashboard}

此儀表板可讓使用者從B2B角度分析其網站效能。

它提供各種資訊，例如依產業、收入、規模、以帳戶為基礎的清單和目標區段的造訪來源和現場行為。

儀表板包含3欄

* 流量來源
* 分段
* 第一層向下切入

1. 建立名為&#x200B;**RTP B2B儀表板**&#x200B;的新儀表板，並定義下列Widget：

![](assets/image2015-3-22-16-3a50-3a3.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      欄1 — 流量來源
    </div></th> 
   <th> 
    <div> <strong>欄2 — 分段</strong> 
    </div></th> 
   <th> 
    <div> <strong>第3欄 — 第一層向下鑽研</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>名稱：依區段和管道區分的工作階段</li> 
     <li>Widget型別： <span class="uicontrol">列</span><br></li> 
     <li><span class="uicontrol">建立顯示</span>： <span class="uicontrol">工作階段</span>的橫條圖</li> 
     <li><span class="uicontrol">依</span>分組： <span class="uicontrol">事件標籤</span></li> 
     <li><span class="uicontrol">樞紐分析依據</span>： <span class="uicontrol">預設通道群組</span></li> 
     <li>篩選器： <br><span class="uicontrol">僅顯示</span> | <span class="uicontrol">事件類別</span> （<span class="uicontrol">包含</span>） RTP區段</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名稱： RTP分段使用者數</li> 
     <li>型別： <span class="uicontrol">2.1量度</span></li> 
     <li><span class="uicontrol">顯示下列量度</span>： <span class="uicontrol">使用者</span><br></li> 
     <li>篩選器： <br><span class="uicontrol">僅顯示</span> | <span class="uicontrol">事件類別</span> （包含） RTP區段</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名稱：依產業區分的工作階段</li> 
     <li>型別： <span class="uicontrol">圓形圖</span><br></li> 
     <li><span class="uicontrol">建立圓形圖，顯示</span>： <span class="uicontrol">工作階段</span></li> 
     <li><span class="uicontrol">依</span>分組： <span class="uicontrol">RTP — 產業</span></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>名稱：依產業和管道區分的工作階段</strong></li> 
     <li><strong>Widget型別： <span class="uicontrol">列</span></strong></li> 
     <li><strong><span class="uicontrol">建立顯示</span>： <span class="uicontrol">工作階段</span>的橫條圖</strong></li> 
     <li><strong><span class="uicontrol">分組依據</span>： <span class="uicontrol">RTP — 產業</span></strong></li> 
     <li><strong><span class="uicontrol">樞紐分析依據</span>： <span class="uicontrol">預設通道群組</span></strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>名稱：依國家/地區劃分的工作階段</strong></li> 
     <li><strong>型別： <span class="uicontrol">Geomap</span></strong></li> 
     <li><strong><span class="uicontrol">繪製選取的量度</span>： <span class="uicontrol">國家/地區</span> | <span class="uicontrol">個工作階段</span></strong></li> 
     <li><strong><span class="uicontrol">選取地區</span>： <span class="uicontrol">世界</span></strong></li> 
     <li><strong>篩選器： <span class="uicontrol">僅顯示</span> | <span class="uicontrol">事件類別</span> （包含） RTP區段</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>名稱：按RTP類別排列的階段作業</strong></li> 
     <li><strong>型別： <span class="uicontrol">圓形圖</span></strong></li> 
     <li><strong><span class="uicontrol">建立圓形圖，顯示</span>： <span class="uicontrol">工作階段</span></strong></li> 
     <li><strong><span class="uicontrol">分組依據</span>： <span class="uicontrol">RTP類別</span></strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>名稱：排名在前的目標區段</li> 
     <li>型別： <span class="uicontrol">列</span></li> 
     <li><span class="uicontrol">建立顯示</span>： <span class="uicontrol">使用者</span>的橫條圖</li> 
     <li><span class="uicontrol">依</span>分組： <span class="uicontrol">事件動作</span></li> 
     <li>篩選器： <span class="uicontrol">僅顯示</span> | <span class="uicontrol">事件類別</span> （包含） RTP區段</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>名稱：按RTP群組排列的階段作業</li> 
     <li>型別：長條圖<br></li> 
     <li>建立長條圖，顯示：階段作業</li> 
     <li>分組依據： RTP-Group</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>名稱：依排名在前的區段區分的工作階段與目標</li> 
     <li>型別：表格<br></li> 
     <li>顯示下列資料行： <br>事件標籤 | 工作階段 | 目標轉換率</li> 
     <li>篩選器：<br>僅顯示 | 事件類別（包含） RTP區段</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## RTP參與儀表板 {#rtp-engagement-dashboard}

此儀表板可讓使用者分析其RTP行銷活動績效和建議引擎參與度。 它提供平均值的比較。 工作階段持續時間與每個工作階段頁面介於：

* 未參與
* 參與（個人化行銷活動的曝光數和點按數）
* 按一下推薦引擎和最常推薦的內容

建立名為&#x200B;**RTP參與儀表板**&#x200B;的新儀表板，並定義下列Widget：

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>欄1行銷活動曝光度</strong> 
    </div></th> 
   <th> 
    <div> <strong>欄2行銷活動點進</strong> 
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
     <li>名稱： <strong>總CTA （參與度）</strong></li> 
     <li>型別： <strong>2.1量度</strong></li> 
     <li>顯示下列量度： <strong>總事件</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（包含）： RTP-Campaigns</strong><br><strong>[僅顯示]事件動作（完全符合）： Impression</strong>[不顯示]事件標籤（包含）： #</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名稱： <strong>CTA總數（點進）</strong></li> 
     <li>型別： <strong>2.1量度</strong></li> 
     <li>顯示下列量度： <strong>總事件</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（包含）： RTP-Campaigns</strong><br><strong>[僅顯示]事件動作（完全相符）：點按次數</strong><strong>[不顯示]事件標籤（包含）： #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名稱： <strong>CRE — 總點按</strong></li> 
     <li>型別： <strong><span class="uicontrol">2.1量度</span></strong><br></li> 
     <li><span class="uicontrol">顯示下列量度</span>： <strong><span class="uicontrol">頁面檢視</span></strong></li> 
     <li>篩選器： <strong>[<span class="uicontrol">僅顯示</span>] <span class="uicontrol">頁面</span> （<span class="uicontrol">包含</span>）： rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>名稱： <strong>平均 工作階段持續時間（參與度）</strong></li> 
     <li>型別： <strong>2.1量度</strong></li> 
     <li>顯示下列量度： <strong>平均 工作階段持續時間</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（完全符合）： RTP-Campaigns</strong><br><strong>[僅顯示]事件動作（完全符合）： impression</strong><strong>[不顯示]事件標籤（包含）： #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>名稱： <strong>平均 工作階段持續時間（點進）</strong></li> 
     <li>型別： <strong>2.1量度</strong></li> 
     <li>顯示下列量度： <strong>平均 工作階段持續時間</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（完全符合）： RTP-Campaigns</strong><br><strong>[僅顯示]事件動作（完全符合）：點按次數</strong><strong>[不顯示]事件標籤（包含）： #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>名稱： <strong>CRE — 最常建議的內容</strong></li> 
     <li>型別： <strong><span class="uicontrol">資料表</span></strong><br></li> 
     <li><span class="uicontrol">顯示下列資料行</span>： <br><strong><span class="uicontrol">頁面標題</span> | <span class="uicontrol">頁面檢視</span></strong><br></li> 
     <li>篩選器：<br>篩選器： <strong>[<span class="uicontrol">僅顯示</span>] <span class="uicontrol">頁面</span> （<span class="uicontrol">包含</span>）： rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>名稱： <strong>頁面/工作階段（參與）</strong></li> 
     <li>型別： <strong><span class="uicontrol">2.1量度</span> </strong></li> 
     <li><span class="uicontrol">顯示下列量度</span>： <strong><span class="uicontrol">頁面/工作階段</span></strong></li> 
     <li>篩選器：<br><strong>[<span class="uicontrol">僅顯示</span>] <span class="uicontrol">事件類別</span> （<span class="uicontrol">完全符合</span>）： RTP-Campaigns</strong></li> 
     <li><strong>[<span class="uicontrol">只顯示</span>] <span class="uicontrol">事件動作</span> （<span class="uicontrol">完全符合</span>）： impression</strong></li> 
     <li><strong>[<span class="uicontrol">不顯示</span>] <span class="uicontrol">事件標籤</span> （<span class="uicontrol">包含</span>）： #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名稱： <strong>頁面/工作階段（點進）</strong></li> 
     <li>型別： <strong>2.1量度</strong></li> 
     <li>顯示下列量度： <strong>頁面/工作階段</strong></li> 
     <li>篩選器：<br><strong>[僅顯示]事件類別（完全相符）： RTP — 促銷活動</strong></li> 
     <li><strong>[僅顯示]事件動作（完全相符）：點按</strong></li> 
     <li><strong>[不要顯示]事件標籤（包含）： #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>名稱： <strong>CTA的曝光數</strong></li> 
     <li>型別： <strong><span class="uicontrol">資料表</span></strong></li> 
     <li><span class="uicontrol">顯示下列資料行</span>： <strong><span class="uicontrol">事件標籤</span> | <span class="uicontrol">事件總數</span> | <span class="uicontrol">位使用者</span></strong></li> 
     <li>篩選器：<br><strong>[<span class="uicontrol">僅顯示</span>] <span class="uicontrol">事件類別</span> （<span class="uicontrol">完全符合</span>）： RTP — 行銷活動</strong><br><strong>[<span class="uicontrol">僅顯示</span>] <span class="uicontrol">事件動作</span> （<span class="uicontrol">完全符合</span>）： impression</strong><strong>[<span class="uicontrol">不顯示</span>] <span class="uicontrol">事件標籤</span> （<span class="uicontrol">包含</span>）： #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>名稱： <strong>CTA的點進</strong></li> 
     <li>型別： <strong><span class="uicontrol">資料表</span></strong></li> 
     <li><span class="uicontrol">顯示下列資料行</span>： <strong><span class="uicontrol">事件標籤</span> | <span class="uicontrol">事件總數</span> | <span class="uicontrol">位使用者</span></strong></li> 
     <li>篩選器：<br><strong>[<span class="uicontrol">僅顯示</span>] <span class="uicontrol">事件類別</span> （<span class="uicontrol">完全符合</span>）： RTP — 行銷活動</strong><br><strong>[<span class="uicontrol">僅顯示</span>] <span class="uicontrol">事件動作</span> （<span class="uicontrol">完全符合</span>）：點按</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[整合RTP與Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Google Universal Analytics中的自訂RTP報告](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
