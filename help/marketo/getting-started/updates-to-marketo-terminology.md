---
unique-page-id: 11387674
description: Marketo術語更新 — Marketo檔案 — 產品檔案
hide: true
hidefromtoc: true
title: Marketo術語更新
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 1%

---

# Marketo術語更新 {#updates-to-marketo-terminology}

我們正在對平台進行一些變更，這些變更將會影響某些專案的名稱。 如果您在2016年3月有新的Marketo執行個體，或是您的公司在2016年7月之後續約，您現在可能會看到新術語。

雖然您在Marketo檔案中可能會看到不同的術語，但請放心，每篇文章將很快更新，以反映這些變更。 所有指示都相同。

那麼，變更了哪些內容？

## 潛在客戶現在是人員 {#lead-is-now-person}

最大變更是將銷售機會/銷售機會重新命名為人員/人員。

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>舊</strong></td>
   <td><strong>新增</strong></td>
  </tr>
  <tr>
   <td>
    <div>
     <img width="295" src="assets/leads.png" data-linked-resource-id="11387678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674">
    </div></td>
   <td>
    <div>
     <img width="295" src="assets/people.png" data-linked-resource-id="11387679" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674">
    </div></td>
  </tr>
 </tbody>
</table>

在某些情況下，「銷售機會」一詞會被直接移除。

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>舊</strong></td>
   <td><strong>新增</strong></td>
  </tr>
  <tr>
   <td>
    <div>
     <img src="assets/lead-database.png" data-linked-resource-id="11387676" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674">
    </div></td>
   <td>
    <div>
     <p><img src="assets/database.png" data-linked-resource-id="11387677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"></p>
    </div></td>
  </tr>
 </tbody>
</table>

潛在客戶與人員&#x200B;**為相同專案**。

## Token {#tokens}

包含單字lead **的權杖未變更**。 很抱歉造成任何混淆；但變更所有代號以符合新術語會中斷目前使用的許多代號。 所以您仍會看到&quot;`{{lead.First Name}}`&quot;之類的權杖。 沒有人員特定的Token。

>[!NOTE]
>
>有&#x200B;*有*&#x200B;個稱為「個人附註」的權杖，但該權杖永遠存在。 如果有的話，它通常用於CRM中的說明欄位。

## 欄位管理 {#field-management}

包含「銷售機會」一詞的欄位已被「人員」取代，或是「銷售機會」一詞已被捨棄。 然而，「潛在客戶擁有者」欄位是一個顯著的例外。 現在稱為「銷售負責人」。

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>舊</strong></td>
   <td><strong>新增</strong></td>
  </tr>
  <tr>
   <td>
    <div>
     <img src="assets/lead-owner.png" data-linked-resource-id="11387757" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674">
    </div></td>
   <td>
    <div>
     <img src="assets/sales-owner.png" data-linked-resource-id="11387758" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674">
    </div></td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>如需受影響的欄位名稱完整清單，請造訪此[支援文章](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target="_blank"}。

## 即時Personalization (RTP)現在是Web Personalization {#real-time-personalization-rtp-is-now-web-personalization}

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>舊</strong></td>
   <td><strong>新增</strong></td>
  </tr>
  <tr>
   <td>
    <div>
     <img src="assets/rtp.png" data-linked-resource-id="11387692" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674">
    </div></td>
   <td>
    <div>
     <img src="assets/web.png" data-linked-resource-id="11387693" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674">
    </div></td>
  </tr>
 </tbody>
</table>

除了名稱變更外，現在它包含四個不同的應用程式：

| **[網頁Personalization](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target="_blank"}** | 在主畫面上擁有自己的圖磚 |
|---|---|
| **[以帳戶為基礎的網頁行銷](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target="_blank"}** | 可透過網頁Personalization圖磚存取 |
| **[個人化重新目標定位](https://docs.marketo.com/display/DOCS/Website+Retargeting){target="_blank"}** | 可透過網頁Personalization圖磚存取 |
| **[預測性內容](https://docs.marketo.com/display/DOCS/Predictive+Content){target="_blank"}** | 在主畫面上擁有自己的圖磚 |

>[!NOTE]
>
>主畫面上顯示的圖磚會反映所購買的模組。

感謝您在此更新期間耐心等候。
