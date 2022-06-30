---
unique-page-id: 11387674
description: Marketo術語更新 — Marketo文檔 — 產品文檔
title: 更新Marketo術語
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# 更新Marketo術語 {#updates-to-marketo-terminology}

我們正在對我們的平台進行一些更改，這將影響某些東西的名稱。 如果您在2016年3月有新的Marketo實例，或者您的公司在2016年7月之後續訂，您現在可能會看到新術語。

雖然您可能在Marketo文檔中看到不同的術語，但請放心，每篇文章都將很快更新以反映這些更改。 所有說明都相同。

那麼，有什麼變化？

## 潛在顧客現在是人 {#lead-is-now-person}

最大的變化是將Lead/Lead更名為Person/People。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>舊</strong></td> 
   <td><strong>新建</strong></td> 
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

在某些情況下，&quot;Lead&quot;一詞被簡單刪除。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>舊</strong></td> 
   <td><strong>新建</strong></td> 
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

線索和人員 **是一樣的**。

## 令牌 {#tokens}

帶有&quot;lead&quot;字樣的標籤 **沒有更改**。 我們為任何混亂表示歉意；但是，如果更改所有令牌以匹配新術語，則會中斷當前使用的所有令牌。 因此您仍然會看到「」等標籤`{{lead.First Name}}`&quot; 沒有特定於個人的令牌。

>[!NOTE]
>
>在那裡 *是* 一個名為「Person Notes」的令牌，但該令牌始終存在。 它通常用於CRM中的描述欄位（如果有）。

## 欄位管理 {#field-management}

包含術語Lead的欄位已被Person替換，或者Lead已被刪除。 但是，一個顯著的例外是「銷售線索責任人」欄位。 它現在被稱為「銷售所有者」。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>舊</strong></td> 
   <td><strong>新建</strong></td> 
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
>有關受影響的欄位名稱的完整清單，請訪問 [支援文章](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target=&quot;_blank&quot;}。

## 即時個性化(RTP)現在是Web個性化 {#real-time-personalization-rtp-is-now-web-personalization}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>舊</strong></td> 
   <td><strong>新建</strong></td> 
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

除了更改名稱外，它現在還由四個獨立的應用組成：

| **[Web個性化](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target=&quot;_blank&quot;** | 在主螢幕上有自己的磁貼 |
|---|---|
| **[基於帳戶的Web營銷](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target=&quot;_blank&quot;** | 可通過Web個性化磁貼訪問 |
| **[個性化重定位](https://docs.marketo.com/display/DOCS/Website+Retargeting){target=&quot;_blank&quot;** | 可通過Web個性化磁貼訪問 |
| **[預測內容](https://docs.marketo.com/display/DOCS/Predictive+Content){target=&quot;_blank&quot;** | 在主螢幕上有自己的磁貼 |

>[!NOTE]
>
>在主螢幕上可見的磁貼將反映所購買的模組。

感謝您在此更新過程中的耐心。
