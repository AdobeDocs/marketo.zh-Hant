---
description: 預設Veeva欄位對應 — Marketo檔案 — 產品檔案
title: 預設Veeva欄位對應
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 33%

---

# 預設Veeva欄位對應 {#default-veeva-field-mapping}

當您初次將Marketo Engage帳戶與Veeva同步時，Marketo會自動在內建Veeva和Marketo欄位之間建立這些關聯。 Marketo也會同步您帳戶和連絡人上的自訂欄位。

## 連絡人欄位 {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>SFDC欄位</th>
      <th>Marketo欄位</th>
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
      <td>連絡人說明</td>
      <td>個人附註</td>
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
      <td>SFDC 已刪除</td>
    </tr>
    <tr>
      <td>姓氏</td>
      <td>姓氏</td>
    </tr>
    <tr>
      <td>銷售機會來源</td>
      <td>來源</td>
    </tr>
    <tr>
      <td>銷售機會分數</td>
      <td>分數</td>
    </tr>
    <tr>
      <td>郵寄城市</td>
      <td>城市</td>
    </tr>
    <tr>
      <td>郵寄國家</td>
      <td>國家</td>
    </tr>
    <tr>
      <td>郵遞區號</td>
      <td>郵遞區號</td>
    </tr>
    <tr>
      <td>MailingState</td>
      <td>州別</td>
    </tr>
    <tr>
      <td>郵寄街</td>
      <td>地址</td>
    </tr>
    <tr>
      <td>行動電話</td>
      <td>手機號碼</td>
    </tr>
    <tr>
      <td>商務電話</td>
      <td>電話號碼</td>
    </tr>
    <tr>
      <td>問候語</td>
      <td>問候語</td>
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
      <th>Marketo欄位</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>年收入</td>
      <td>年收入</td>
    </tr>
    <tr>
      <td>帳單城市</td>
      <td>帳單城市</td>
    </tr>
    <tr>
      <td>帳單國家</td>
      <td>帳單國家</td>
    </tr>
    <tr>
      <td>帳單郵遞區號</td>
      <td>帳單郵遞區號</td>
    </tr>
    <tr>
      <td>帳單州/省</td>
      <td>帳單州別</td>
    </tr>
    <tr>
      <td>帳單街道</td>
      <td>帳單地址</td>
    </tr>
    <tr>
      <td>帳戶說明</td>
      <td>公司備註</td>
    </tr>
    <tr>
      <td>產業</td>
      <td>產業</td>
    </tr>
    <tr>
      <td>已刪除</td>
      <td>SFDC 已刪除</td>
    </tr>
    <tr>
      <td>帳戶名稱</td>
      <td>公司名稱</td>
    </tr>
    <tr>
      <td>員工</td>
      <td>員工人數</td>
    </tr>
    <tr>
      <td>帳戶電話</td>
      <td>主要電話</td>
    </tr>
    <tr>
      <td>SIC 代碼</td>
      <td>SIC 代碼</td>
    </tr>
    <tr>
      <td>帳戶網站</td>
      <td>網站</td>
    </tr>
    <tr>
      <td>帳戶型別</td>
      <td>SFDC 類型</td>
    </tr>
    <tr>
      <td>網站</td>
      <td>網站</td>
    </tr>
  </tbody>
</table>

## Marketo中的Veeva相關系統欄位（唯讀） {#veeva-related-system-fields-in-marketo}

這些欄位是在Marketo中建立的，但客戶無法調整。

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
      <td>Veeva Id</td>
      <td>18個字元的Salesforce Id</td>
    </tr>
    <tr>
      <td>Veeva型別</td>
      <td>連絡人。 如果留空，則潛在客戶只會以Marketo中的個人身分存在</td>
    </tr>
    <tr>
      <td>Veeva建立日期</td>
      <td>在SFDC中建立的日期(可以與Marketo中建立的日期不同)</td>
    </tr>
    <tr>
      <td>Veeva已刪除</td>
      <td>此人員之前在SFDC中，但已被刪除，現在僅居住在Marketo中</td>
    </tr>
  </tbody>
</table>
