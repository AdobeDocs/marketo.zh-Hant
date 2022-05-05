---
description: 預設Veeva欄位映射 — Marketo文檔 — 產品文檔
title: 預設Veeva欄位映射
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 27%

---

# 預設Veeva欄位映射 {#default-veeva-field-mapping}

當您最初將Marketo Engage帳戶與Veeva同步時，Marketo會自動在您內置的Veeva欄位和Marketo欄位之間進行這些關聯。 Marketo還將同步帳戶和聯繫人上的自定義欄位。

## 聯繫人欄位 {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>SFDC欄位</th>
      <th>Marketo場</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>出生日期</td>
      <td>出生日期</td>
    </tr>
    <tr>
      <td>建立日期</td>
      <td>SFDC建立日期</td>
    </tr>
    <tr>
      <td>聯繫人描述</td>
      <td>人員備注</td>
    </tr>
    <tr>
      <td>電子郵件</td>
      <td>電子郵件地址</td>
    </tr>
    <tr>
      <td>商務傳真</td>
      <td>傳真號碼</td>
    </tr>
    <tr>
      <td>名字</td>
      <td>名字</td>
    </tr>
    <tr>
      <td>電子郵件選擇退出</td>
      <td>退訂</td>
    </tr>
    <tr>
      <td>已刪除</td>
      <td>已刪除SFDC</td>
    </tr>
    <tr>
      <td>姓氏</td>
      <td>姓氏</td>
    </tr>
    <tr>
      <td>潛在客戶來源</td>
      <td>來源</td>
    </tr>
    <tr>
      <td>潛在客戶分數</td>
      <td>得分</td>
    </tr>
    <tr>
      <td>郵寄城市</td>
      <td>城市</td>
    </tr>
    <tr>
      <td>郵寄國家/地區</td>
      <td>國家</td>
    </tr>
    <tr>
      <td>郵寄郵遞區號</td>
      <td>郵遞區號</td>
    </tr>
    <tr>
      <td>郵寄狀態</td>
      <td>州</td>
    </tr>
    <tr>
      <td>郵寄街</td>
      <td>地址</td>
    </tr>
    <tr>
      <td>手機</td>
      <td>手機號碼</td>
    </tr>
    <tr>
      <td>商務電話</td>
      <td>電話號碼</td>
    </tr>
    <tr>
      <td>稱謂</td>
      <td>稱謂</td>
    </tr>
    <tr>
      <td>標題</td>
      <td>職稱</td>
    </tr>
  </tbody>
</table>

## 帳戶欄位 {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>SFDC欄位</th>
      <th>Marketo場</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>年營業額</td>
      <td>年營業額</td>
    </tr>
    <tr>
      <td>帳單寄送城市</td>
      <td>帳單寄送城市</td>
    </tr>
    <tr>
      <td>帳單寄送國家</td>
      <td>帳單寄送國家</td>
    </tr>
    <tr>
      <td>開單郵遞區號</td>
      <td>帳單郵遞區號</td>
    </tr>
    <tr>
      <td>開單州/省</td>
      <td>帳單寄送州</td>
    </tr>
    <tr>
      <td>計費街</td>
      <td>帳單寄送地址</td>
    </tr>
    <tr>
      <td>帳戶說明</td>
      <td>公司說明</td>
    </tr>
    <tr>
      <td>行業</td>
      <td>行業</td>
    </tr>
    <tr>
      <td>已刪除</td>
      <td>已刪除SFDC</td>
    </tr>
    <tr>
      <td>帳戶名</td>
      <td>公司名稱</td>
    </tr>
    <tr>
      <td>員工</td>
      <td>員工數</td>
    </tr>
    <tr>
      <td>帳戶電話</td>
      <td>主要電話</td>
    </tr>
    <tr>
      <td>標準產業分類（SIC）代碼</td>
      <td>標準產業分類（SIC）代碼</td>
    </tr>
    <tr>
      <td>帳戶站點</td>
      <td>現場</td>
    </tr>
    <tr>
      <td>帳戶類型</td>
      <td>SFDC類型</td>
    </tr>
    <tr>
      <td>網站</td>
      <td>網站</td>
    </tr>
  </tbody>
</table>

## Marketo的Veeva相關系統欄位（只讀） {#veeva-related-system-fields-in-marketo}

這些欄位是在Marketo建立的，但無法由客戶調整。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>欄位</th>
      <th>說明</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>維娃ID</td>
      <td>18個字元的Salesforce Id</td>
    </tr>
    <tr>
      <td>維瓦類型</td>
      <td>聯繫。 如果空，則該線索僅作為一個人存在於Marketo</td>
    </tr>
    <tr>
      <td>維埃瓦建立日期</td>
      <td>在SFDC中建立的日期(可與在Marketo建立的日期不同)</td>
    </tr>
    <tr>
      <td>已刪除Veeva</td>
      <td>以前在SFDC但被刪除，現在只住在Marketo</td>
    </tr>
  </tbody>
</table>
