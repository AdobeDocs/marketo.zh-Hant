---
unique-page-id: 11387674
description: Marketo 術語更新 - Marketo 文件 - 產品文件
hide: true
hidefromtoc: true
title: Marketo 術語更新
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '328'
ht-degree: 100%

---

# Marketo 術語更新 {#updates-to-marketo-terminology}

我們正在對平台進行變更，而這會影響某些項目的名稱。若您在 2016 年 3 月前有新的 Marketo 執行個體，或者您的公司在 2016 年 7 月之後續約，則您現在所看到的應該是新術語。

雖然您可能會在 Marketo 文件中看到不同的術語，但請放心，每篇文章很快便會更新來反映這些變更內容。所有指示維持不變。

變更的內容有哪些？

## 「商機」現在為「人員」 {#lead-is-now-person}

最大的變更是將「商機」重新命名為「人員」。

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>舊版</strong></td>
   <td><strong>新版</strong></td>
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

在部分情況下是直接移除「商機」一詞。

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>舊版</strong></td>
   <td><strong>新版</strong></td>
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

「商機」與「人員」**是指同樣的事情**。

## 權杖 {#tokens}

含有「lead」一詞的權杖&#x200B;**沒有變更**。對於所造成的任何混淆，我們深表歉意；但是，若為了符合新術語而變更所有權杖，會大量破壞目前正在使用的權杖。因此您仍然會看到諸如「`{{lead.First Name}}`」的權杖。沒有任何人員特定的權杖。

>[!NOTE]
>
>的確是&#x200B;*有*&#x200B;一個名為「人員備註」的權杖，但該權杖一直以來都有。其通常用於 CRM 中的描述欄位 (若有)。

## 欄位管理 {#field-management}

含有術語「商機」的欄位已經替換為「人員」，或者刪除「商機」一詞。然而，有一個值得注意的例外是「商機所有者」欄位。其現在名為「銷售所有者」。

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>舊版</strong></td>
   <td><strong>新版</strong></td>
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
>若要受影響之欄位名稱的完整清單，請造訪此[支援文章](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target="_blank"}。

## 「即時個人化」(RTP) 現在為「網頁個人化」 {#real-time-personalization-rtp-is-now-web-personalization}

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>舊版</strong></td>
   <td><strong>新版</strong></td>
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

除了名稱變更之外，其現在由四個獨立的應用程式組成：

| **[網頁個人化](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target="_blank"}** | 在主畫面上有其自己的圖磚 |
|---|---|
| **[帳戶型網頁行銷](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target="_blank"}** | 可透過網頁個人化圖磚存取 |
| **[個人化重定向](https://docs.marketo.com/display/DOCS/Website+Retargeting){target="_blank"}** | 可透過網頁個人化圖磚存取 |
| **[預測內容](https://docs.marketo.com/display/DOCS/Predictive+Content){target="_blank"}** | 在主畫面上有其自己的圖磚 |

>[!NOTE]
>
>主畫面上顯示的圖磚會反映所購買的模組。

感謝您在本次更新期間的耐心等候。
