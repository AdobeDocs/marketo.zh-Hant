---
unique-page-id: 2949160
description: 與Adobe Analytics整合 — Marketo檔案 — 產品檔案
title: 整合Adobe Analytics
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---

# 整合Adobe Analytics {#integrate-with-adobe-analytics}

## 簡介 {#intro}

在您的Adobe Analytics帳戶中檢視組織、產業和Marketo即時個人化(RTP)促銷活動資料，從B2B觀點分析您的網頁分析。

本檔案可啟用Marketo即時個人化(RTP)與AdobeAdobe Analytics之間的整合。 來自RTP的資料可讓您偵測和分析造訪您網站的所有產業區段和組織的趨勢，並評估RTP促銷活動的成效，提供深入分析和分析以取得最佳結果。

您可以透過查看每個區段中新訪客與再度訪問的訪客的數量等量度、分析促銷活動的點按率，以及探索哪些產業和自訂區段及即時促銷活動產生最佳轉換銷售機會，來達成此目標。 運用此功能，即可從您的RTP帳戶中獲得最大效益。

## RTPAudience Analytics {#rtp-audience-analytics}

透過RTP - AA整合，您的網頁分析介面中有新的維度。 RTP會透過下列功能自動增強您的網頁分析控制面板：

1. 組織與產業資料
1. 自訂的RTP區段
1. 指定帳戶清單(Account-Based Marketing)

這可增強您的B2B資料，並可讓您透過最佳化以專注於相關訪客：

1. 傳出頻道
1. 內容
1. 重新定位

## 管道報表 {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

RTP控制面板可協助您了解根據垂直和RTP區段的訪客劃分。 您可以根據產業查看訪客績效，以及與該產業相關的不同行銷活動（付費、自然、社交）。 控制面板也提供訪客根據其產業類型所檢視之網站區域的概觀。

## 行為報告 {#behavioral-report}

根據組織、產業和RTP區段資料，可在Adobe Analytics中建立不同的行為報表。 這些「流量」報表可視化訪客從一個頁面或事件到下一個頁面所採取的路徑。 此報告可協助您探索讓訪客持續參與您網站的內容。

## RTP效能 {#rtp-performance}

在Adobe Analytics的自訂連結下檢視RTP促銷活動曝光次數和轉換。

此自訂連結報表將以下列命名格式顯示促銷活動的曝光次數和轉換次數：

* 曝光ISgment: [RTP段名稱],Campaign: [RTP促銷活動名稱]
* 轉換區段： [RTP段名稱],Campaign: [RTP促銷活動名稱]

![](assets/custom-links-report.png)

## 在Adobe Analytics中設定 {#set-up-in-adobe-analytics}

整合使用Adobe Analytics提供的JavaScript API。 整合中使用自訂轉換變數(eVar)、自訂事件（事件）和流量變數。 必須從AA管理員內啟用所有項目。 您必須在Aa中設定轉換變數、自訂事件和流量變數，否則即使您在RTP中啟用了資料，也無法在套裝中查看資料。

完成下列步驟，在AA中設定這些變數：

1. 前往 **管理工具** 在您的AA帳戶中。
1. 選取 **報表套裝** 與整合搭配使用。
1. 在 **編輯設定**，前往 **轉換** 選取 **[轉換變數](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   選取 [轉換變數](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) 數字（我們建議）:

   1. 產業自訂轉換的Evar # 20
   1. 組織自訂轉換的Evar # 21

   >[!NOTE]
   >
   >如果取得這些#，請選取其他可用號碼。 將此號碼與RTP帳戶設定中的插槽號碼對齊。

   1. 將狀態變更為 _已啟用_.

      1. 將名稱變更為 **產業** 和 **組織**. （這是報表套裝中的顯示方式。）

      1. 將「過期時間」欄位變更為 **瀏覽**.


1. 在 **編輯設定** 轉到 **轉換** 選取 **[成功事件](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

   1. 選取自訂成功事件事件編號（我們建議）:

      1. event20 for RTP促銷活動
      1. event21 for RTP區段

      >[!NOTE]
      >
      >如果取得這些#，請選取其他可用號碼。 將此號碼與RTP帳戶設定中的插槽號碼對齊。

      1. 將兩個事件名稱變更為 **RTP促銷活動** 和 **RTP區段**. 這是報表套裝中會顯示的名稱。
   1. 選取要 **計數器（無子關聯）**



1. 在 **編輯設定** 轉到 **[流量](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)** 選取 **[流量變數](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. 選取流量變數屬性#（建議使用）:

      1. 屬性# 20 — 名稱：RTP區段組織
      1. 屬性# 21 — 名稱：RTP區段產業
      1. 屬性# 25 — 名稱：促銷活動組織
      1. 屬性# 26 — 名稱：RTP促銷活動產業

      >[!NOTE]
      >
      >如果取得這些#，請選取其他可用號碼。 將此編號與RTP帳戶設定中的插槽編號對齊)

      1. 變更4個屬性名稱。 這是報表套裝中會顯示的名稱。
   1. 選擇要啟用的欄位 **已啟用**.

   1. 選擇路徑報表欄位 **已啟用**.



## 在Marketo即時個人化(RTP)中設定 {#set-up-in-marketo-real-time-personalization-rtp}

1. 在RTP平台中，前往 **帳戶設定**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 在 **帳戶設定**，按一下 **網域**.
1. 在 **Analytics，按一下** **Adobe Analytics**.
1. 轉彎 **開啟** 轉換、自訂和流量變數切換。
1. 指派轉換、事件和流量變數 **槽號** 與AA中建立的插槽號匹配
1. 按一下 **儲存**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>建議的插槽設定為
>
>**轉換變數**
>
>* 產業自訂轉換 — 插槽20
>* 組織自訂轉換 — 插槽21
>
>**自訂事件**
>
>* 促銷活動自訂事件 — 插槽20
>* 區段自訂事件 — 插槽21
>
>**流量變數**
>
>* 區段組織流量變數 — 槽20
>* 區段產業流量變數 — 插槽21
>* 促銷活動組織流量變數 — 槽22
>* 促銷活動產業流量變數 — 插槽23
>
>**請確定這些插槽編號與AA中建立的變數和事件編號一致。**

## 報表 {#reports}

根據組織名稱、產業和RTP區段以及即時行銷活動資料，建立增強的SiteAdobe Analytics報表。

AA中的自訂報表和控制面板範例包括：

* 依產業或定義區段的效能（以帳戶為基礎的命名清單）
* 按KPI績效劃分的行業
* 每個組織檢視的頁面
* 根據組織、產業、區段的行銷管道績效

**— 報表範例 —**

**熱門產業報告**

![](assets/top-industries-report.png)

**組織報表**

![](assets/image2014-11-29-12-3a29-3a42.png)

**建立RTP控制面板**

建立 [新儀表板](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html)，呼叫 **RTP控制面板**. 此控制面板將協助了解根據垂直和RTP區段的訪客劃分。

1. 按一下 **控制面板，** 按一下 **新增控制面板**.

1. 命名控制面板 **RTP控制面板**.

1. 選取 **控制面板大小** 3 x 2、2 x 2。

1. 建立 [小報告](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) 新增 [內容到控制面板](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard).

新增產業小報表至控制面板

1. 前往 **自訂轉換**，按一下 **產業**.

1. 將圖表配置為 **圓形圖**.

1. 按一下 **控制面板**，新增 **小報表**.

1. 為報表命名 **熱門產業**.

1. 在儀表板中放置 **RTP控制面板**.

1. 建立 **新增**.

新增區段小報表至控制面板

1. 前往 **網站量度**. 按一下 **自訂事件**, **區段**.

1. 將圖表配置為 **垂直條**.

1. 按一下 **控制面板**，新增 **小報表**.

1. 為報表命名 **排名在前的區段**.

1. 在儀表板中放置 **RTP控制面板**.

1. 建立 **新增**.

您的小報表將顯示在控制面板中。

## 在Adobe Analytics中檢視曝光次數和點按次數（轉換） {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. 按一下 **自訂連結**.

   ![](assets/sitecatalyst1-1.png)

1. 搜尋「曝光數」以檢視代表促銷活動曝光數的區段和促銷活動名稱。\
   ![](assets/sitecatalyst1.png)

1. 搜尋轉換以檢視代表促銷活動點按次數的群體和促銷活動名稱。

   ![](assets/sitecatalyst2.png)
