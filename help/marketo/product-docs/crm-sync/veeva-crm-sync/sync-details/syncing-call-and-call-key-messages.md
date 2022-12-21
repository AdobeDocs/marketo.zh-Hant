---
description: 同步呼叫和呼叫關鍵訊息 — Marketo檔案 — 產品檔案
title: 正在同步呼叫和呼叫密鑰消息
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
source-git-commit: bb020cba0bb0cb65761e15cba05147b6e9fffe50
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 2%

---

# 正在同步呼叫和呼叫密鑰消息 {#syncing-call-and-call-key-messages}

Veva CRM中的呼叫和呼叫金鑰訊息物件預設會同步至Marketo Engage。 Marketo會根據呼叫建立日期同步最多6個月的資料。

>[!NOTE]
>
>Marketo會自呼叫日期起保留最多6個月的呼叫資料。

**與呼叫和呼叫金鑰訊息相關的觸發器/篩選器為何？**

觸發器：

* 新增至呼叫
* 從呼叫中移除
* 新增至呼叫密鑰訊息
* 從呼叫密鑰消息中刪除
* 更新呼叫
* 更新呼叫密鑰消息

篩選器:

* 有呼叫
* 有呼叫密鑰消息

系統會同步呼叫和呼叫金鑰訊息的下列欄位，並可作為限制和觸發器使用。

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
      <td>呼叫</td>
      <td>會計</td>
      <td>查閱與呼叫相關聯的帳戶。</td>
      <td>Account_vod__c</td>
      <td>查閱（帳戶）</td>
    </tr>
    <tr>
      <td>呼叫</td>
      <td>呼叫類型</td>
      <td>根據呼叫的類型和內容而維護的呼叫類型。 此欄位用於報告用途。 有效值為：僅詳細資訊、帶樣本的詳細資訊、組詳細資訊、帶樣本的組詳細資訊、僅示例。 這些值不應更改，但這些選擇清單的翻譯可能會更改。 與會者的呼叫類型與標頭呼叫相同。 對於有3名專業人員的組呼，所有4條記錄的呼叫類型都為「組詳細資訊」</td>
      <td>Call_Type_vod__c</td>
      <td>選擇清單</td>
    </tr>
    <tr>
     <td>呼叫</td>
      <td>連絡人</td>
      <td>查閱與呼叫相關聯的連絡人（如果有）。</td>
      <td>Contact_vod__c</td>
      <td>查閱（聯繫人）</td>
    </tr>
    <tr>
      <td>呼叫</td>
      <td>日期</td>
      <td>首次儲存或提交呼叫的日期。 如果未提供date或datetime欄位，則此欄位通過觸發器設定為當前日期。</td>
      <td>Call_Date_vod__c</td>
      <td>日期</td>
    </tr>
    <tr>
      <td>呼叫</td>
      <td>是父呼叫嗎？</td>
      <td>公式欄位，確定呼叫記錄是父呼叫還是與會者呼叫記錄。 1表示記錄為父呼叫。 0表示它是與會者呼叫。</td>
      <td>Is_Parent_Call_vod__c</td>
      <td>公式（數字）</td>
    </tr>
    <tr>
      <td>呼叫</td>
      <td>狀態</td>
      <td>呼叫狀態 — 已計畫、已保存或已提交。 使用翻譯工作台來變更顯示值。 呼叫時觸發器會查看此欄位，查看呼叫是否已鎖定（提交）。 按下「儲存」或「提交」按鈕時，系統會為使用者設定此值。</td>
      <td>Status_vod__c</td>
      <td>選擇清單</td>
    </tr>
    <tr>
      <td>呼叫</td>
      <td>記錄類型</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>記錄類型</td>
    </tr>
    <tr>
      <td>呼叫密鑰消息</td>
      <td>呼叫</td>
      <td>查詢至呼叫。 每個關鍵消息都與呼叫相關聯。</td>
      <td>呼叫2_vod__c</td>
      <td>主詳細資訊（呼叫）</td>
    </tr>
    <tr>
      <td>呼叫密鑰消息</td>
      <td>類別</td>
      <td>記錄訊息的訊息類別。 主要用於報告。</td>
      <td>Category_vod__c</td>
      <td>選擇清單</td>
    </tr>
    <tr>
      <td>呼叫密鑰消息</td>
      <td>CLM演示名稱</td>
      <td>已加註CLM演示文稿名稱</td>
      <td>Clm_Presentation_Name_vod__c</td>
      <td>文本(80)</td>
    </tr>
    <tr>
      <td>呼叫密鑰消息</td>
      <td>密鑰消息名稱</td>
      <td>加註戳的鍵消息名稱</td>
      <td>Key_Message_Name_vod__c</td>
      <td>文本(80)</td>
    </tr>
    <tr>
      <td>呼叫密鑰消息</td>
      <td>產品名稱</td>
      <td> </td>
      <td>Product_Name__c</td>
      <td>公式（文本）</td>
    </tr>
    <tr>
      <td>呼叫密鑰消息</td>
      <td>反應</a>
      </td>
      <td>對消息的反應清單。 編輯選擇清單以更改反應值。</td>
      <td>Reaction_vod__c</td>
      <td>選擇清單</td>
    </tr>
  </tbody>
</table>
