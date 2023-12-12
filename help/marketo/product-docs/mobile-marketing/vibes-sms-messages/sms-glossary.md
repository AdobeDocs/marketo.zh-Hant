---
description: 檔案 — Marketo檔案 — 產品檔案
title: 檔案
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: ce43fe1848bb333caa2f73fde4c6ce8403b3e1e8
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 0%

---

# 簡訊字彙表 {#sms-glossary}

以下是您將Vibes SMS訊息與Marketo Engage搭配使用時可能會遇到的常見詞語。

<table>
<thead>
  <tr>
    <th>詞語</th>
    <th>定義</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>贏取促銷活動</td>
    <td>用來取得訂閱清單新訂閱者的行銷活動。 您可以透過Marketo網頁表單或傳送關鍵字文字將訂閱者新增至贏取促銷活動。</td>
  </tr>
  <tr>
    <td>行銷活動管理員</td>
    <td>Campaign Manager位於Vibes平台，您可在此處設定訂閱清單和贏取行銷活動。 擁有完整Vibes平台授權的使用者可存取其他行銷活動型別。</td>
  </tr>
  <tr>
    <td>公司金鑰</td>
    <td>company_key是您平台帳戶的唯一英數字元識別碼。 如果您在Vibes平台中有多個公司帳戶（例如子帳戶），則可能會有多個company_keys。 Marketo Engage的每個執行個體只能對應至一個Vibes company_key。</td>
  </tr>
  <tr>
    <td>CTA （行動號召）</td>
    <td>數位或實體招牌或口頭指令碼，用於取得定期簡訊節目或訂閱清單的訂閱者。 可以放線上上、社群媒體上、電子郵件中、印刷品等中。</td>
  </tr>
  <tr>
    <td>自訂短網域</td>
    <td>如果您使用Vibes連結縮短程式，則縮短的URL預設會顯示在Vibes短URL下方： https://vbs.cm/xxxxxx。 自訂簡短網域是您的品牌專屬的網域。 <a href="https://developer-platform.vibes.com/docs/creating-a-custom-short-domain">進一步瞭解自訂短網域</a>.<p>
    這僅適用於從Vibes平台傳送的訊息，特別是贏取促銷活動訊息和短程式碼預設訊息。<p>
    為了在您的Marketo程式中擁有點按資料，建議使用Marketo URL縮短程式。</td>
  </tr>
  <tr>
    <td>預設訊息</td>
    <td>短程式碼的必要訊息，可回覆HELP、STOP及無法辨識的訊息要求。</td>
  </tr>
  <tr>
    <td>中斷連接</td>
    <td>中斷連線是一種選擇退出的形式，因為行動電話號碼已從電信業者網路中移除。 中斷連線的原因包括：帳戶已完全關閉、預付帳戶資金不足，或因其他未知原因而從電信業者網路移除號碼。 中斷連線且未移植到其他行動電信業者的行動電話號碼會從Vibes平台中的所有訂閱清單中取消訂閱。</td>
  </tr>
  <tr>
    <td>雙重選擇加入</td>
    <td>一種贏取方法，需要潛在訂閱者確認其同意透過回應命令（如「Y」或郵遞區號）新增至訂閱清單。 使用雙重選擇加入提示可協助您遵守州和聯邦的文字訊息傳送方針。</td>
  </tr>
  <tr>
    <td>事件</td>
    <td>事件是可提交至Vibes平台的已定義發生次數，用於觸發API觸發的動作，包括訊息傳送。 每個事件都包含該事件特有的資料，包括event_type，用於判斷與哪個API觸發訊息行銷活動相對應。 事件API可透過Marketo Engage中的Webhook觸發。 進一步瞭解 <a href="https://developer-platform.vibes.com/reference/event-api">事件API參考</a>.</td>
  </tr>
  <tr>
    <td>關鍵字</td>
    <td>消費者傳送給短程式碼的短文字或英數字串，用以起始行動體驗。</td>
  </tr>
  <tr>
    <td>長程式碼(10DLC)</td>
    <td>在品牌和消費者之間傳送雙向訊息的寄件者ID。 美國長程式碼為10位數。</td>
  </tr>
  <tr>
    <td>MDN</td>
    <td>行動電話號碼，或個人電話號碼。 MDN和行動電話號碼在Marketo中不是唯一的識別碼。</td>
  </tr>
  <tr>
    <td>行動資料庫</td>
    <td>行動資料庫是Vibes儲存訂閱者資料的資料庫。 每個訂閱者都有唯一的「個人記錄」，行動電話號碼和任何相關聯的自訂欄位會填入。</td>
  </tr>
  <tr>
    <td>參與者</td>
    <td>與您的行動程式有一或多個行動互動（例如傳送簡訊）但尚未訂閱訂閱清單的人員。</td>
  </tr>
  <tr>
    <td>個人記錄</td>
    <td>個人記錄是特定行動電話號碼的資料集合。 每個個人記錄也會獲派一個唯一的person_key來識別。 Marketo ID會使用external_person_id欄位連結至Vibes。 進一步瞭解中的個人記錄 <a href="https://developer-platform.vibes.com/reference/person-api">Vibes人員API檔案</a>.</td>
  </tr>
  <tr>
    <td>簡短程式碼</td>
    <td>在品牌和消費者之間傳送雙向訊息的寄件者ID。 美國短程式碼為5-6位數。 加拿大短程式碼為4-6位數。 Marketo LaunchPoint與Vibes的整合支援每個執行個體使用一個短程式碼。</td>
  </tr>
  <tr>
    <td>簡訊</td>
    <td>簡訊服務。 此訊息僅包含文字。</td>
  </tr>
  <tr>
    <td>訂閱清單</td>
    <td>提供同意接收來自您程式之週期性訊息的行動電話號碼（及其對應人員記錄）清單。</td>
  </tr>
  <tr>
    <td>訂閱者</td>
    <td>訂閱訂閱訂閱清單的行動電話號碼。</td>
  </tr>
  <tr>
    <td>Vibes Platform</td>
    <td>您登入以管理行銷活動的網站。 前往 <a href="https://nexus.us.vibes.com/">https://nexus.us.vibes.com/</a> 以存取Vibes平台。</td>
  </tr>
</tbody>
</table>
