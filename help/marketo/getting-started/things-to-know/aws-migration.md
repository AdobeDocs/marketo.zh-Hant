---
description: AWS移轉 — Marketo Engage檔案 — 產品檔案
title: AWS移轉
feature: Getting Started
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 9a445d50781458b3342be0dd9c1a4262346a9f7f
workflow-type: tm+mt
source-wordcount: '835'
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
>如果您使用[外部表單](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"}，並且想要避免在移轉期間無法使用Marketo Engage時收集而遺失表單提交資料，請事先聯絡[Adobe支援](https://experienceleague.adobe.com/zh-hant/support){target="_blank"} **至少兩個工作日**，並提供表單ID和您訂閱的Munchkin ID。

## 識別您的資料中心/Pod {#identify}

在檢閱下清單格之前，[請先瞭解如何識別](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify)您的訂閱所在的資料中心和pod/伺服器。

## 排程 {#schedule}

新日期和Data Center/Pod資訊會定期新增或變更，因此請監視此排程以取得更新。

+++7月排程
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
   <td>AB54</td>
   <td>下午5點PDT</td>
   <td>已完成</td>
  </tr>
  <tr>
   <td>2026年7月23日</td>
   <td>AB48</td>
   <td>下午5點PDT</td>
   <td>已完成</td>
  </tr>
  <tr>
   <td>2026年7月31日</td>
   <td>AB43</td>
   <td>下午3點PDT</td>
   <td>已完成</td>
  </tr>
  </body>
</table>

+++

<table>
 <tbody>
  <tr>
   <th style="width:25%">日期</th>
   <th style="width:25%">資料中心/Pod</th>
   <th style="width:25%">時間</th>
   <th style="width:25%">狀態</th>
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
  <tr>
  <td>2026年8月13日</td>
   <td>AB68</td>
   <td>下午4點PDT</td>
   <td>準時發行</td>
  </tr>
  <tr>
  <td>2026年8月18日</td>
   <td>AB39</td>
   <td>下午5點PDT</td>
   <td>準時發行</td>
  </tr>
  <tr>
   <td>2026年8月20日</td>
   <td>AB42<br>
   AB44</td>
   <td>下午5點PDT<br>
   下午6點PDT</td>
   <td>準時發行<br>
   依排程</td>
  </tr>
  <tr>
   <td>2026年8月26日</td>
   <td>AB40<br>
   AB50</td>
   <td>下午5點PDT<br>
   下午6點PDT</td>
   <td>準時發行<br>
   依排程</td>
  </tr>
  <tr>
   <td>2026年8月28日</td>
   <td>AB53<br>
   AB56</td>
   <td>下午3點PDT<br>
   下午4點PDT</td>
   <td>準時發行<br>
   依排程</td>
  </tr>
  <tr>
   <td>2026年9月8日</td>
   <td>AB01<br>
   AB02</td>
   <td>下午5點PDT<br>
   下午6點PDT</td>
   <td>準時發行<br>
   依排程</td>
  </tr>
  <tr>
   <td>2026年9月10日</td>
   <td>AB03<br>
   AB04</td>
   <td>下午5點PDT<br>
   下午6點PDT</td>
   <td>準時發行<br>
   依排程</td>
  </tr>
  <tr>
   <td>2026年9月15日</td>
   <td>AB05<br>
   AB06</td>
   <td>下午5點PDT<br>
   下午6點PDT</td>
   <td>準時發行<br>
   依排程</td>
  </tr>
  <tr>
   <td>2026年9月17日</td>
   <td>AB07<br>
   AB08</td>
   <td>下午5點PDT<br>
   下午6點PDT</td>
   <td>準時發行<br>
   依排程</td>
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

## 常見問題集 {#faq}

**資料儲存於何處？**
所有Marketo使用者資料都儲存在Amazon Web Services (AWS)上。 Marketo已將其基礎架構從擁有的實體資料中心移轉至AWS的企業級雲端平台。

**個人資料的具體儲存位置？**
個人資料儲存在AWS完全受管理的關聯式資料庫服務Amazon Aurora中。 Aurora會以六種方式在AWS地區的三個獨立可用區中複製資料，以保護個人資料免於硬體故障、儲存裝置降級和本地化基礎架構事件。

**誰擁有儲存環境？**
儲存基礎建設由Amazon Web Services (AWS)所擁有和營運。 Adobe (Marketo)是以AWS客戶的身分來運作，並採用共同責任模式：AWS負責基礎建設的安全性和可用性，而Adobe則負責基礎建設中執行之資料和應用程式的安全性。

**生產、備份/DR位置和儲存技術的完整詳細資料為何？**
Marketo使用Amazon Aurora （完全由AWS管理的雲端原生關聯式資料庫引擎）作為主要資料庫技術。 Aurora會將運算與儲存分離，以六種方式自動複製生產區域內3個可用區中的資料，並需要四份法定復本才能確認任何寫入操作。

Aurora也會即時執行持續自動備份至Amazon S3，以便在設定的保留期間內，隨時進行時間點復原(PITR)。

目前，Marketo的Aurora部署可在單一AWS區域運作，無需跨區域復寫。 生產資料會保留在指定的區域基礎架構中，而災難回覆是透過Aurora的多可用區儲存備援和持續備份來提供，而不是透過地理容錯移轉至次要區域。 隨著Marketo的AWS基礎建設日漸成熟，可進一步評估這項作業。
