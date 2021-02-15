---
unique-page-id: 2949160
description: 與Adobe Analytics整合——行銷檔案——產品檔案
title: 與Adobe Analytics整合
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---


# 與Adobe Analytics {#integrate-with-adobe-analytics}整合

## 介紹{#intro}

從B2B的角度分析您的網頁分析，在Adobe Analytics帳戶中檢視組織、產業和行銷人員即時個人化(RTP)宣傳資料。

本檔案可讓Marketo Real-Time Personalization(RTP)與Adobe Adobe Analytics整合。 來自RTP的資料可讓您偵測和分析造訪您網站的所有產業區段和組織的趨勢，並評估RTP宣傳的成效，提供深入資訊和分析以取得最佳結果。

您可以透過查看每個區段中新訪客與舊訪客的數量等度量、分析促銷活動的點按率，以及發現哪些產業和自訂區段及即時促銷活動產生最佳轉化銷售機會，來達成此目標。 利用此功能，從您的RTP帳戶中獲得最大的好處。

## RTP觀眾分析{#rtp-audience-analytics}

透過RTP - AA整合，您的網頁分析介面中有了新的維度。 RTP可自動增強您的網頁分析資料板，包括：

1. 組織與產業資料
1. 自訂的RTP區段
1. 指名帳戶清單（以帳戶為基礎的行銷）

這可增強您的B2B資料，並讓您透過最佳化：

1. 出站渠道
1. 內容
1. 重新定位

## 渠道報表{#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

RTP儀表板可協助您瞭解依垂直產業和RTP區段劃分的訪客。 您可以根據產業及與該產業相關的不同行銷活動（付費、自然、社交）來查看訪客績效。 控制面板也提供訪客依其產業類型檢視哪些網站區域的高階概述。

## 行為報告{#behavioral-report}

Adobe Analytics可以根據組織、產業和RTP區段資料建立不同的行為報表。 這些流量報表可視覺化訪客從一個頁面或事件到下一個頁面或事件的路徑。 此報告可協助您發現哪些內容可讓訪客參與您的網站。

## RTP效能{#rtp-performance}

在Adobe Analytics的「自訂連結」下檢視RTP促銷活動曝光和轉換。

此「自訂連結」報表將以下命名格式顯示促銷活動的印象和轉換：

* 印象區段：[RTP段名稱],ICampaign:[RTP促銷活動名稱]
* 轉換區段：[RTP段名稱],ICampaign:[RTP促銷活動名稱]

![](assets/custom-links-report.png)

## 在Adobe Analytics中設定{#set-up-in-adobe-analytics}

整合使用Adobe Analytics提供的JavaScript API。 自訂轉換變數(eVar)、自訂事件（事件）和流量變數會用於整合中。 必須在AA管理員中啟用所有功能。 您必須在AA中設定轉換變數、自訂事件和流量變數，否則即使您在RTP中啟用資料，也無法在套裝中看到資料。

完成下列步驟，在AA中設定這些變數：

1. 前往您AA帳戶中的&#x200B;**管理工具**。
1. 選擇要與整合一起使用的&#x200B;**報表套裝**。
1. 在&#x200B;**編輯設定下，**&#x200B;移至&#x200B;**轉換**&#x200B;並選取** [轉換變數](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**。\
   選擇[轉換變數](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar)數字（我們建議）:

   1. 

      1. 業界自訂轉換的Evar # 20
      1. 組織自訂轉換的Evar # 21

         >[!NOTE]
         >
         >如果取得這些#，請選取其他可用編號。 將此編號與「RTP帳戶設定」中的插槽編號對齊。

      1. 將狀態變更為*啟用*

         1. 將「名稱」更改為&#x200B;**Industry**&#x200B;和&#x200B;**Organization**。 （這是報表套裝中的顯示方式。）

         1. 將「過期時間」欄位變更為「瀏覽」。****

1. 在「**編輯設定&#x200B;**」下，移至「轉換** a2/>」，並選取「** [成功事件](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**」。**

1. 選取自訂成功事件事件編號（我們建議）:

   1. event20 for RTP Campaigns
   1. RTP段的event21

      >[!NOTE]
      >
      >如果取得這些#，請選取其他可用編號。 將此編號與「RTP帳戶設定」中的插槽編號對齊。

   1. 將兩個事件名稱更改為&#x200B;**RTP促銷活動**&#x200B;和&#x200B;**RTP段**。 此名稱將會出現在報表套裝中。

1. 選擇類型* *欄位為&#x200B;**計數器（無子關聯）**

1. 在&#x200B;**編輯設定**&#x200B;下，轉至** [流量](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable) **並選擇** [流量變數](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**。

   1. 選取流量變數屬性#（我們建議）:

      1. 屬性編號20 —— 名稱：RTP段組織
      1. 屬性編號21 —— 名稱：RTP Segment Industry
      1. 屬性編號25 —— 名稱：促銷活動組織
      1. 屬性編號26 —— 名稱：RTP Campaign產業

         >[!NOTE]
         >
         >如果取得這些#，請選取其他可用編號。 將此編號與RTP帳戶設定中的插槽編號對齊)

      1. 變更4個屬性名稱。 此名稱將會出現在報表套裝中。
   1. 選擇「啟用」欄位至&#x200B;**Enabled**
   1. 選擇路徑報表欄位至&#x200B;**啟用**


## 在Marketo Real-Time Personalization(RTP)中設定{#set-up-in-marketo-real-time-personalization-rtp}

1. 在RTP平台中，轉到&#x200B;**帳戶設定**。

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 在「**帳戶設定**」下，按一下「**網域**」。
1. 在「**Analytics」下方，按一下「** **Adobe Analytics**」。
1. 開啟**On **轉換、自訂和流量變數切換。
1. 指派轉換、事件和流量變數&#x200B;**槽號**，以符合AA中建立的槽號
1. 按一下&#x200B;**SAVE**。

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>我們建議的插槽設定是
>
>**轉換變數**
>
>* 產業自訂轉換——插槽20
>* 組織自訂轉換——插槽21

>
>
**自訂事件**
>
>* 促銷活動自訂事件——插槽20
>* 區段自訂事件——插槽21

>
>
**流量變數**
>
>* 區段組織流量變數——插槽20
>* 區段產業流量變數——插槽21
>* 促銷活動組織流量變數——插槽22
>* 促銷活動產業流量變數——插槽23

>
>
**請確定這些插槽編號與在AA中建立的變數和事件編號對齊。**

## 報告{#reports}

根據組織名稱、產業和RTP區段以及即時宣傳資料，建立增強的SiteAdobe Analytics報表。

AA中自訂報表和控制面板的範例包括：

* 依產業或定義區段的績效（以帳戶為基礎的命名清單）
* 依KPI績效劃分的產業
* 依組織檢視的頁面
* 依組織、產業、區段的行銷渠道績效

**報表範例**

**熱門產業報告**

** ![](assets/top-industries-report.png)

**

**組織報表**

![](assets/image2014-11-29-12-3a29-3a42.png)

**建立RTP儀表板**

建立名為&#x200B;**RTP儀表板**&#x200B;的新儀表板[。 ](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html)此控制面板將協助您瞭解依垂直產業和RTP區段劃分的訪客。

1. 按一下「**控制面板」,**&#x200B;按一下**「新增控制面板」**

1. 命名儀表板&#x200B;**RTP儀表板**
1. 選擇&#x200B;**控制面板大小** 3 x 2、2 x 2
1. 建立[reportlet](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3)並新增[內容至控制面板](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard)

新增產業報表至控制面板

1. 前往「自訂轉換&#x200B;****」，按一下「**產業**」

1. 將圖形配置為&#x200B;**圓形圖**
1. 按一下&#x200B;**儀表板**，新增&#x200B;**小報告**

1. 將報表命名為&#x200B;**熱門產業**
1. 位於儀表板&#x200B;**RTP儀表板**
1. 建立&#x200B;**新建**。

新增區段小報表至控制面板

1. 前往**網站量度， **按一下&#x200B;**自訂事件，區段**

1. 將圖形配置為&#x200B;**垂直條**
1. 按一下&#x200B;**儀表板**，新增&#x200B;**小報告**

1. 為報表命名&#x200B;**排名最前的區段**
1. 位於儀表板&#x200B;**RTP儀表板**
1. 建立&#x200B;**新建。**

您的小報表會顯示在控制面板中。

## 在Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}中檢視印象和點按（轉換）

1. 按一下「自訂連結」。

   ![](assets/sitecatalyst1-1.png)

1. 搜尋印象以檢視代表促銷活動印象數的區段和促銷活動名稱。\
   ![](assets/sitecatalyst1.png)

1. 搜尋轉換以檢視代表促銷活動點按次數的區段和促銷活動名稱。

   ![](assets/sitecatalyst2.png)

