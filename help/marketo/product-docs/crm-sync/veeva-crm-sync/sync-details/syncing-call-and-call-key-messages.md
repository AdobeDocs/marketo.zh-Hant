---
description: 同步呼叫和呼叫重要訊息 — Marketo檔案 — 產品檔案
title: 同步呼叫和呼叫重要訊息
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 3%

---

# 同步呼叫和呼叫重要訊息 {#syncing-call-and-call-key-messages}

[!DNL Veeva] CRM中的Call和Call鍵訊息物件預設會同步至Marketo Engage。 Marketo會根據通話建立日期同步最多6個月前的資料。

>[!NOTE]
>
>Marketo會保留通話資料最長為通話當日起六個月。

**與通話和通話金鑰訊息相關的觸發器/篩選器是什麼？**

觸發器：

* 已新增至通話
* 從通話中移除
* 已新增至通話金鑰訊息
* 從通話金鑰訊息中移除
* 已更新通話
* 已更新通話金鑰訊息

篩選器：

* 有呼叫
* 具有呼叫鍵訊息

會同步呼叫和呼叫金鑰訊息的下列欄位，並可用作限制和觸發器。

<table>
  <colgroup>
    <col>
    <col>
    <col>
    <col>
    <col>
  </colgroup>
  <thead>
    <tr>
      <th>
        物件
      </th>
      <th>
        欄位標籤
      </th>
      <th>
        說明
      </th>
      <th>
        欄位名稱
      </th>
      <th>
        資料類型
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>號召</td>
      <td>會計師</td>
      <td>查詢與通話相關聯的帳戶。</td>
      <td>Account_vod__c</td>
      <td>查詢（帳戶）</td>
    </tr>
    <tr>
      <td>號召</td>
      <td>呼叫型別</td>
      <td>根據呼叫的型別和內容由系統維護的呼叫型別。 此欄位用於報表用途。 有效值為：僅限明細、含範例的明細、群組明細、含範例的群組明細、僅限範例。 這些值不應變更，但這些選擇清單的翻譯可能會變更。 出席者的通話型別與標頭通話相同。 如果是有3名專業人員的群組通話，全部4筆記錄的通話型別為「群組詳細資料」</td>
      <td>Call_Type_vod__c</td>
      <td>挑選清單</td>
    </tr>
    <tr>
     <td>號召</td>
      <td>聯絡人</td>
      <td>查詢與通話相關聯的連絡人（如果有的話）。</td>
      <td>Contact_vod__c</td>
      <td>查詢（連絡人）</td>
    </tr>
    <tr>
      <td>號召</td>
      <td>日期</td>
      <td>通話的首次儲存或提交日期。 若未提供日期或日期時間欄位，則會透過觸發器將此欄位設定為目前的日期。</td>
      <td>Call_Date_vod__c</td>
      <td>日期</td>
    </tr>
    <tr>
      <td>號召</td>
      <td>是父級通話嗎？</td>
      <td>公式欄位，用以判斷通話記錄是上階通話記錄還是出席者通話記錄。 1表示該記錄是父呼叫。 0表示這是出席者通話。</td>
      <td>Is_Parent_Call_vod__c</td>
      <td>公式（數字）</td>
    </tr>
    <tr>
      <td>號召</td>
      <td>狀態</td>
      <td>通話狀態 — 已計畫、已儲存或已提交。 使用轉譯維護作業來變更顯示值。 呼叫觸發程式會檢視此欄位，以檢視呼叫是否已鎖定（提交）。 當按下「儲存」或「提交」按鈕時，此值會針對使用者設定。</td>
      <td>Status_vod__c</td>
      <td>挑選清單</td>
    </tr>
    <tr>
      <td>號召</td>
      <td>記錄型別</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>記錄型別</td>
    </tr>
    <tr>
      <td>呼叫鍵訊息</td>
      <td>號召</td>
      <td>查詢呼叫。 每個重要訊息都與呼叫相關聯。</td>
      <td>Call2_vod__c</td>
      <td>Master-Detail（呼叫）</td>
    </tr>
    <tr>
      <td>呼叫鍵訊息</td>
      <td>類別</td>
      <td>紀錄訊息的訊息類別。 主要用於報表。</td>
      <td>Category_vod__c</td>
      <td>挑選清單</td>
    </tr>
    <tr>
      <td>呼叫鍵訊息</td>
      <td>CLM簡報名稱</td>
      <td>加註戳記的CLM簡報名稱</td>
      <td>Clm_Presentation_Name_vod__c</td>
      <td>文字(80)</td>
    </tr>
    <tr>
      <td>呼叫鍵訊息</td>
      <td>金鑰訊息名稱</td>
      <td>加註戳記的金鑰訊息名稱</td>
      <td>Key_Message_Name_vod__c</td>
      <td>文字(80)</td>
    </tr>
    <tr>
      <td>呼叫鍵訊息</td>
      <td>產品名稱</td>
      <td> </td>
      <td>Product_Name__c</td>
      <td>公式（文字）</td>
    </tr>
    <tr>
      <td>呼叫鍵訊息</td>
      <td>回應</a>
      </td>
      <td>訊息的回應挑選清單。 編輯挑選清單以變更反應值。</td>
      <td>Reaction_vod__c</td>
      <td>挑選清單</td>
    </tr>
  </tbody>
</table>
