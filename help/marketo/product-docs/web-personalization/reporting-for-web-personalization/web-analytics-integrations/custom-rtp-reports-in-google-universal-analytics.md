---
unique-page-id: 7504218
description: Google Universal Analytics中的自訂RTP報表——行銷檔案——產品檔案
title: Google Universal Analytics中的自訂RTP報表
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---


# Google Universal Analytics中的自訂RTP報表{#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[將RTP與Google Universal Analytics整合](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

本文說明如何為Google Universal Analytics(GUA)設定RTP自訂報表。  從RTP發送到GUA的資料可以設定為兩個單獨的自定義報告，名為：

* RTP B2B
* RTP參與

## 設定自訂報表{#setting-up-a-custom-report}

1. 登入Google Analytics。

1. 按一下頂部菜單中的&#x200B;**Customization**。

1. 按一下「**+新自訂報表**」。

![](assets/image2015-3-22-16-3a10-3a48.png)

## RTP B2B報告{#rtp-b-b-report}

1. 為報告命名&#x200B;**RTP B2B報告**。

1. 為第一個頁籤命名&#x200B;**Industry**。

>[!NOTE]
>
>您將&#x200B;**複製此標籤**&#x200B;並建立其他類似標籤——步驟5)

1. 選擇&#x200B;**Explorer**&#x200B;報表類型。

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. 在&#x200B;**量度群組**&#x200B;區段中，選取與您的業務相關的量度。

   a.我們建議您：

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. 複製此標籤4次，並命名：

   1. **產業**
   1. **群組**
   1. **類別**
   1. **ABM**
   1. **組織**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. 在&#x200B;**維度下鑽**&#x200B;區段中，為每個標籤設定相關維度，如下所示。

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      標籤名稱 
    </div></th> 
   <th> 
    <div>
      維度下鑽
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>產業</td> 
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

1. 請勿設定任何篩選條件，並將此報表設為&#x200B;**所有網站資料**&#x200B;可用(或變更（如果與特定Analytics帳戶相關）。

1. 按一下&#x200B;**保存**。

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## RTP參與報告{#rtp-engagement-report}

1. 為報告命名&#x200B;**RTP參與報告**。

1. 將第1個標籤名稱設定為&#x200B;**所有參與**。

>[!NOTE]
>
>您將複製此標籤並建立其他類似標籤——步驟5)

1. 選擇&#x200B;**Explorer**&#x200B;報表類型。

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. 在「量度群組」區段中，選取與您的業務相關的量度。 以下是建議：

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. 複製此標籤4次，並命名：

   1. **所有參與**
   1. **依產業區分的參與度**
   1. **參與（依群組區分）**
   1. **參與（依類別區分）**
   1. **ABM的參與**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. 在&#x200B;**維度下鑽**&#x200B;區段中，將每個標籤的相關維度設定如下：

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      標籤名稱 
    </div></th> 
   <th> 
    <div>
      維度下鑽 
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
   <td>參與（依類別區分）</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>參與（依群組區分）</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>依產業區分的參與度</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. 設定下列篩選：

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
      符合類型 
    </div></th> 
   <th> 
    <div>
      值 
    </div></th> 
   <th colspan="1"> 
    <div>
      注釋 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><p>包含</p></td> 
   <td><p>事件類別</p></td> 
   <td>Regex</td> 
   <td>RTP-Campaigns|RTP-Recommendations|RTP-Segments</td> 
   <td colspan="1">將過濾與RTP無關的所有其它自定義事件</td> 
  </tr> 
  <tr> 
   <td>排除</td> 
   <td>事件標籤</td> 
   <td>Regex</td> 
   <td>#</td> 
   <td colspan="1">可讓您使用促銷活動名稱中的#，從報表促銷活動中篩選</td> 
  </tr> 
 </tbody> 
</table>

1. 將此報告設為&#x200B;**所有網站資料**（或視需要變更）。

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. 按一下&#x200B;**保存**。

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[將RTP與Google Universal Analytics整合](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Google Universal Analytics中的自訂RTP儀表板](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
