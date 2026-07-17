---
description: AWS移轉 — Marketo Engage檔案 — 產品檔案
title: AWS移轉
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: cd0b1dece6129df76deb7eb9c8953711d4d29e45
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 5%

---

# AWS移轉 {#aws-migration}

在接下來的幾個月中，所有Marketo Engage訂閱都將從私人資料中心移轉至AWS公用雲端，以提升可靠性、擴充性和速度。

您將在移轉前約30天收到電子郵件和應用程式內通知。 使用本指南進行準備。

## 建議的動作 {#actions}

在移轉期間，所有Marketo Engage服務都將無法使用。 建議您採取下列步驟，以免對業務造成任何影響。

* **避免建立或更新銷售機會/人員**，或執行修改人員記錄的程式。

* **不要觸發後續程式**，因為排程的行銷活動將會暫停。

* **暫時停用所有傳送資料給Marketo Engage或從接收資料的整合**。

* **避免執行**&#x200B;資料匯入或匯出，或任何主要的銷售機會/人員產生行銷活動。

* **檢閱並更新IP允許清單**，以取得登入、API存取、電子郵件傳送、網頁追蹤和整合。

* **新增IP位址**&#x200B;並保留您目前的IP不變。 檢視要透過下方[&#128279;](#ip-addresses)的表格新增的IP位址。

## 預期的服務影響 {#impacts}

您無需對下列影響執行任何動作。

* **CRM整合和LaunchPoint服務**&#x200B;將會停用，但之後應該會自動繼續。
* **登陸頁面、表單和資料彙集**&#x200B;將無法使用，而將會顯示維護訊息。

>[!NOTE]
>
>如果您使用[外部表單](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"}，並且想要在移轉期間保留資料，請聯絡[Adobe支援](https://experienceleague.adobe.com/zh-hant/support){target="_blank"}，並提供表單ID和您訂閱的Munchkin ID。

## 識別您的資料中心/Pod {#identify}

在檢閱下清單格之前，[請先瞭解如何識別](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify)您的訂閱所在的資料中心和pod/伺服器。

## 排程 {#schedule}

新的日期和資料中心/Pod資訊會定期新增，因此請務必回到這裡檢視詳細資訊。

<table>
 <tbody>
  <tr>
   <th style="width:25%">日期</th>
   <th style="width:25%">資料中心/Pod</th>
   <th style="width:25%">時間</th>
   <th style="width:25%">狀態</th>
  </tr>
  <tr>
   <td>2026年7月8日</td>
   <td>AB69<br>
   AB64</td>
   <td>下午5點PDT<br>
   下午6點PDT</td>
   <td>已完成<br>
   已完成</td>
  </tr>
  <tr>
   <td>2026年7月9日</td>
   <td>AB70</td>
   <td>下午5點PDT</td>
   <td>已完成</td>
  </tr>
  <tr>
   <td>2026年7月11日</td>
   <td>AB46</td>
   <td>上午10點PDT</td>
   <td>已完成</td>
  </tr>
  <tr>
   <td>2026年7月13日</td>
   <td>NLD101</td>
   <td>上午10點PDT</td>
   <td>已完成</td>
  </tr>
  <tr>
   <td>2026年7月15日</td>
   <td>NLD102<br>
   NLD104</td>
   <td>上午10點PDT<br>
   上午11點PDT</td>
   <td>已完成<br>
   已完成</td>
  </tr>
  <tr>
   <td>2026年7月17日</td>
   <td>NLD103<br>
   NLD105</td>
   <td>上午10點PDT<br>
   上午11點PDT</td>
   <td>已完成<br>
   已完成</td>
  </tr>
  <tr>
   <td>2026年7月21日</td>
   <td>AB54<br>
   AB56</td>
   <td>下午5點PDT<br>
   下午6點PDT</td>
   <td>準時發行<br>
   依排程</td>
  </tr>
  <tr>
   <td>2026年7月23日</td>
   <td>AB48</td>
   <td>下午5點PDT</td>
   <td>準時發行</td>
  </tr>
  <tr>
   <td>2026年7月31日</td>
   <td>AB43</td>
   <td>下午3點PDT</td>
   <td>準時發行</td>
  </tr>
  <tr>
   <td>2026年8月12日</td>
   <td>AB61<br>
   AB17</td>
   <td>下午3點PDT<br>
   下午4點PDT</td>
   <td>準時發行<br>
   依排程</td>
  </tr>
  <td>2026年8月13日</td>
   <td>AB68</td>
   <td>下午4點PDT</td>
   <td>準時發行</td>
  </tr>
  </body>
</table>

## 要新增的IP位址 {#ip-addresses}

根據您的資料中心，與您的IT部門合作，以新增個別IP位址。

<table>
<tbody>
<tr>
  <th style="width:25%">資料中心</th>
  <th style="width:75%">IP位址</th>
</tr>
<tr>
  <td>AB</td>
  <td>54.160.246.246<br>
  54.237.141.197<br>
  52.20.211.99</td>
</tr>
<tr>
  <td>NLD</td>
  <td>34.247.24.245<br>
18.200.201.81<br>
54.220.138.65</td>
</tr>
</body>
</table>

## 更新與支援 {#support}

如需最新更新，請將此頁面加入書籤。 如果您有任何問題，請透過Admin Console的支援入口網站或[Experience League](https://experienceleague.adobe.com/zh-hant/support){target="_blank"}聯絡Adobe支援。
