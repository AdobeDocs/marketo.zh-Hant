---
unique-page-id: 5472615
description: 瞭解系統管理的欄位 — Marketo檔案 — 產品檔案
title: 瞭解系統管理的欄位
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: fc25a088005ee1d552f6e61e2fa7b953e2fde862
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 8%

---

# 瞭解系統管理的欄位 {#understanding-system-managed-fields}

您可能已注意到[個人詳細資料頁面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}有一連串由Marketo建立的不可編輯欄位。 這些資料來自各種來源，而且可以顯示無數值。

## 欄位型別 {#field-types}

<table><thead>
  <tr>
    <th>欄位名稱</th>
    <th>定義</th>
  </tr></thead>
<tbody>
  <tr>
    <td>原始來源類型</td>
    <td>首次發現個人或網站訪客的位置（範例：清單匯入、網頁造訪）</td>
  </tr>
  <tr>
    <td>原始來源資訊</td>
    <td>該位置的詳細資訊（範例：清單名稱、網頁URL）</td>
  </tr>
  <tr>
    <td>原始搜尋引擎</td>
    <td>將人員轉至原始專案來源的搜尋引擎（如適用）</td>
  </tr>
  <tr>
    <td>原始搜尋片語</td>
    <td>如果適用，會使用將人員轉至原始專案來源的搜尋字詞</td>
  </tr>
  <tr>
    <td>原始反向連結</td>
    <td>託管原始登入來源的URL</td>
  </tr>
  <tr>
    <td>註冊Source型別</td>
    <td>活動首次成為個人的位置（例如：清單匯入、網頁造訪）</td>
  </tr>
  <tr>
    <td>註冊Source資訊</td>
    <td>該位置的詳細資訊（範例：清單名稱、網頁URL）</td>
  </tr>
  <tr>
    <td>匿名 IP</td>
    <td>表示個人的IP位址</td>
  </tr>
  <tr>
    <td>推斷的公司</td>
    <td>Marketo對個人公司的最佳猜測（根據IP）</td>
  </tr>
  <tr>
    <td>推斷的城市</td>
    <td>Marketo對個人城市的最佳猜測（根據IP）</td>
  </tr>
  <tr>
    <td>推斷的州別區域</td>
    <td>Marketo對個人所在州或地區的最佳猜測（根據IP）</td>
  </tr>
  <tr>
    <td>推斷的郵遞區號</td>
    <td>Marketo對個人郵遞區號的最佳猜測（根據IP）</td>
  </tr>
  <tr>
    <td>推斷的國家</td>
    <td>Marketo對個人所在國家/地區的最佳猜測（根據IP）</td>
  </tr>
  <tr>
    <td>推斷的大都會區</td>
    <td>Marketo對個人大都會區域的最佳猜測（根據IP）</td>
  </tr>
  <tr>
    <td>推斷的電話區碼</td>
    <td>Marketo對個人區碼的最佳猜測（根據IP）</td>
  </tr>
</tbody></table>

## 原始和註冊Source型別的可能值 {#possible-values-for-original-and-registration-source-type}

以下是一些可能的值及其含義。

<table><thead>
  <tr>
    <th>原始來源類型</th>
    <th>定義</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Salesforce.com</td>
    <td>從Salesforce同步處理探索到人員</td>
  </tr>
  <tr>
    <td>網頁瀏覽次數</td>
    <td>從網頁發現人員</td>
  </tr>
  <tr>
    <td>網頁表單轉出</td>
    <td>填寫表單後發現人員</td>
  </tr>
  <tr>
    <td>清單匯入</td>
    <td>從清單匯入中發現人員</td>
  </tr>
  <tr>
    <td>新人員</td>
    <td>已將人員手動輸入資料庫</td>
  </tr>
  <tr>
    <td>Web連結點按</td>
    <td>按一下連結後發現人員</td>
  </tr>
  <tr>
    <td>銷售電子郵件</td>
    <td>已透過Sales Insight電子郵件增益集傳送電子郵件給人員</td>
  </tr>
  <tr>
    <td>個人</td>
    <td>已將個人從Salesforce同步為個人</td>
  </tr>
  <tr>
    <td>連絡人</td>
    <td>已將人員從Webhook同步為聯絡人</td>
  </tr>
  <tr>
    <td>Munchkin API</td>
    <td>Marketo EngageMunchkin API已發現人員</td>
  </tr>
  <tr>
    <td>社交應用程式</td>
    <td>由社交Widget探索人員</td>
  </tr>
  <tr>
    <td>網站服務API</td>
    <td>透過網站服務API發現人員</td>
  </tr>
  <tr>
    <td>活動合作夥伴</td>
    <td>透過同步網路研討會服務發現人員</td>
  </tr>
  <tr>
    <td>關聯銷售機會</td>
    <td>透過「關聯銷售機會API」呼叫合併的人員</td>
  </tr>
</tbody></table>

<table><thead>
  <tr>
    <th>註冊Source型別</th>
    <th>定義</th>
  </tr></thead>
<tbody>
  <tr>
    <td>清單匯入</td>
    <td>透過清單匯入成為個人</td>
  </tr>
  <tr>
    <td>Salesforce.com</td>
    <td>透過Salesforce同步成為人員</td>
  </tr>
  <tr>
    <td>網頁表單轉出</td>
    <td>填寫表單後成為人員</td>
  </tr>
  <tr>
    <td>銷售電子郵件</td>
    <td>已透過Sales Insight電子郵件增益集傳送電子郵件給人員</td>
  </tr>
  <tr>
    <td>網站服務API</td>
    <td>已透過SOAP/REST API建立人員</td>
  </tr>
  <tr>
    <td>新人員</td>
    <td>已將人員手動輸入資料庫</td>
  </tr>
  <tr>
    <td>Munchkin API</td>
    <td>透過Marketo的Munchkin API成為人</td>
  </tr>
  <tr>
    <td>社交應用程式</td>
    <td>透過社交Widget變成人</td>
  </tr>
  <tr>
    <td>活動合作夥伴</td>
    <td>透過連結的網路研討會服務成為個人</td>
  </tr>
</tbody>
</table>
