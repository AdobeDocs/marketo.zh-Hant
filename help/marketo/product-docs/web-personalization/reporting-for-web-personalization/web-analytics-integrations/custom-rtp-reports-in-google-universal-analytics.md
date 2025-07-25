---
unique-page-id: 7504218
description: Google Universal Analytics中的自訂RTP報表 — Marketo檔案 — 產品檔案
title: Google Universal Analytics中的自訂RTP報表
exl-id: c8b1e653-03b8-48bc-b80d-3e6cdf3485c3
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 3%

---

# Google Universal Analytics中的自訂RTP報表 {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[整合RTP與Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

本文說明如何設定Google Universal Analytics (GUA)的RTP自訂報表。  從RTP傳送到GUA的資料可以設定為兩個單獨的自訂報告，稱為：

* RTP B2B
* RTP參與

## 設定[!UICONTROL Custom Report] {#setting-up-a-custom-report}

1. 登入Google Analytics。

1. 按一下頂端功能表中的&#x200B;**[!UICONTROL Customization]**。

1. 按一下「**[!UICONTROL New Custom Report]**」。

![](assets/image2015-3-22-16-3a10-3a48.png)

## RTP B2B報表 {#rtp-b-b-report}

1. 命名報告&#x200B;**RTP B2B報告**。

1. 為第一個索引標籤命名&#x200B;**[!UICONTROL Industry]**。

>[!NOTE]
>
>您將&#x200B;**複製此索引標籤**&#x200B;並建立其他類似的索引標籤 — 步驟5)

1. 選取&#x200B;**[!UICONTROL Explorer]**&#x200B;報告型別。

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. 在&#x200B;**[!UICONTROL Metric Groups]**&#x200B;區段中，選取與您的業務相關的量度。

   a.我們建議以下事項：

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. 複製此索引標籤4次並命名它們：

   1. **產業**
   1. **群組**
   1. **類別**
   1. **ABM**
   1. **組織**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. 在&#x200B;**Dimension深入研究**&#x200B;區段中，設定每個標籤的相關維度，如下所示。

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      標簽名稱 
    </div></th> 
   <th> 
    <div>
      Dimension深入研究
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>行業</td> 
   <td><img src="assets/1.png" data-linked-resource-id="7514675" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td><img src="assets/2.png" data-linked-resource-id="7514674" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>類別</td> 
   <td><img src="assets/3.png" data-linked-resource-id="7514673" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>ABM</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>組織</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. 請勿設定任何篩選器，並將此報表設定為可供&#x200B;**[!UICONTROL All Web Site Data]**&#x200B;使用（或在與特定Analytics帳戶相關時變更）。

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## RTP參與報告 {#rtp-engagement-report}

1. 命名報告&#x200B;**RTP參與報告**。

1. 將第一個索引標簽名稱設為&#x200B;**[!UICONTROL All Engagement]**。

>[!NOTE]
>
>您將重複此標籤並建立其他類似的標籤 — 步驟5)

1. 選取&#x200B;**[!UICONTROL Explorer]**&#x200B;報告型別。

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. 在[!UICONTROL Metric Groups]區段中，選取與您的業務相關的量度。 建議如下：

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. 複製此索引標籤4次並命名它們：

   1. **所有參與**
   1. **產業參與度**
   1. **依群組的參與**
   1. 依類別&#x200B;**參與度**
   1. 由ABM進行的&#x200B;**參與**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. 在&#x200B;**Dimension深入研究**&#x200B;區段中，設定每個標籤的相關維度，如下所示：

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      標簽名稱 
    </div></th> 
   <th> 
    <div>
      Dimension深入研究 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>所有參與</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>ABM的參與</td> 
   <td><img width="277" src="assets/4.png" data-linked-resource-id="7514678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>依類別的參與</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>依群組的參與</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>各產業參與度</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. 設定下列篩選器：

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Inc/Exc 
    </div></th> 
   <th> 
    <div>
      欄位 
    </div></th> 
   <th> 
    <div>
      比對型別 
    </div></th> 
   <th> 
    <div>
      值 
    </div></th> 
   <th colspan="1"> 
    <div>
      註解 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><p>包含</p></td> 
   <td><p><span class="uicontrol">事件類別</span></p></td> 
   <td>Regex</td> 
   <td>RTP-Campaigns|RTP-Recommendations|RTP-Segments</td> 
   <td colspan="1">將篩選與RTP無關的所有其他自訂事件</td> 
  </tr> 
  <tr> 
   <td>排除</td> 
   <td><span class="uicontrol">事件標籤</span></td> 
   <td>Regex</td> 
   <td>#</td> 
   <td colspan="1">可讓您使用行銷活動名稱中的#，從報表行銷活動中進行篩選</td> 
  </tr> 
 </tbody> 
</table>

1. 將此報告設定為&#x200B;**[!UICONTROL All Web Site Data]**&#x200B;可用（或視需要變更）。

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. 按一下「**[!UICONTROL Save]**」。

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[整合RTP與Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Google Universal Analytics中的自訂RTP儀表板](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
