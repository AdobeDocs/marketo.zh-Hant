---
description: 同步呼叫和呼叫密鑰消息 — Marketo文檔 — 產品文檔
title: 同步呼叫和呼叫密鑰消息
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
source-git-commit: bb020cba0bb0cb65761e15cba05147b6e9fffe50
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# 同步呼叫和呼叫密鑰消息 {#syncing-call-and-call-key-messages}

預設情況下，Veeva CRM中的調用和調用密鑰消息對象將同步到Marketo Engage。 Marketo根據呼叫建立日期同步最多6個月的資料。

>[!NOTE]
>
>Marketo保留自呼叫之日起至6個月的呼叫資料。

**與呼叫和呼叫密鑰消息相關的觸發器/過濾器是什麼？**

觸發器：

* 添加到呼叫
* 已從呼叫中刪除
* 已添加到呼叫密鑰消息
* 已從呼叫密鑰消息中刪除
* 已更新呼叫
* 已更新的呼叫密鑰消息

篩選器：

* 有呼叫
* 有呼叫密鑰消息

呼叫和呼叫密鑰消息上的以下欄位將同步，並可用作約束和觸發器。

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
        對象
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
      <td>查找呼叫關聯的帳戶。</td>
      <td>帳戶_vod_c</td>
      <td>查找（帳戶）</td>
    </tr>
    <tr>
      <td>呼叫</td>
      <td>呼叫類型</td>
      <td>根據呼叫的類型和內容維護的呼叫的類型。 此欄位用於報告目的。 有效值為：僅詳細資訊、帶樣例的詳細資訊、組詳細資訊、帶樣例的組詳細資訊、僅示例。 不應更改這些值，但可以更改這些選擇清單的翻譯。 與會者的呼叫類型與標題呼叫相同。 對於有3名專業人員的組呼叫，所有4條記錄的呼叫類型均為「組詳細資訊」</td>
      <td>調用類型_vod_c</td>
      <td>選擇清單</td>
    </tr>
    <tr>
     <td>呼叫</td>
      <td>聯繫人</td>
      <td>查找與呼叫關聯的聯繫人（如果有）。</td>
      <td>聯繫人_vod_c</td>
      <td>查找（聯繫人）</td>
    </tr>
    <tr>
      <td>呼叫</td>
      <td>日期</td>
      <td>首次保存或提交呼叫的日期。 如果未提供date或datetime欄位，則通過觸發器將此欄位設定為當前日期。</td>
      <td>調用_日期_vod_c</td>
      <td>日期</td>
    </tr>
    <tr>
      <td>呼叫</td>
      <td>是父呼叫嗎？</td>
      <td>公式欄位，用於確定呼叫記錄是父呼叫還是與會者呼叫記錄。 1表示該記錄為「父呼叫」。 0表示它是與會者呼叫。</td>
      <td>Is_Parent_Call_vod_c</td>
      <td>公式（數字）</td>
    </tr>
    <tr>
      <td>呼叫</td>
      <td>狀態</td>
      <td>呼叫的狀態 — 已計畫、已保存或已提交。 使用轉換工作台更改顯示值。 呼叫觸發器查看此欄位以查看呼叫是否已鎖定（已提交）。 按「保存」或「提交」按鈕時，將為用戶設定此值。</td>
      <td>狀態_vod_c</td>
      <td>選擇清單</td>
    </tr>
    <tr>
      <td>呼叫</td>
      <td>記錄類型</td>
      <td> </td>
      <td>記錄類型ID</td>
      <td>記錄類型</td>
    </tr>
    <tr>
      <td>呼叫密鑰消息</td>
      <td>呼叫</td>
      <td>查找呼叫。 每個密鑰消息與呼叫相關聯。</td>
      <td>調用2_vod_c</td>
      <td>主詳細資訊（呼叫）</td>
    </tr>
    <tr>
      <td>呼叫密鑰消息</td>
      <td>類別</td>
      <td>記錄消息的消息類別。 主要用於報告。</td>
      <td>類別_vod_c</td>
      <td>選擇清單</td>
    </tr>
    <tr>
      <td>呼叫密鑰消息</td>
      <td>CLM演示文稿名稱</td>
      <td>標籤的CLM演示名稱</td>
      <td>Clm_Presentation_Name_vod_c</td>
      <td>文本(80)</td>
    </tr>
    <tr>
      <td>呼叫密鑰消息</td>
      <td>密鑰消息名稱</td>
      <td>標籤的密鑰消息名稱</td>
      <td>鍵_消息_名稱_vod_c</td>
      <td>文本(80)</td>
    </tr>
    <tr>
      <td>呼叫密鑰消息</td>
      <td>產品名稱</td>
      <td> </td>
      <td>產品名稱_c</td>
      <td>公式（文本）</td>
    </tr>
    <tr>
      <td>呼叫密鑰消息</td>
      <td>反應</a>
      </td>
      <td>對消息的反應選擇清單。 編輯選擇清單以更改反應值。</td>
      <td>反應_vod_c</td>
      <td>選擇清單</td>
    </tr>
  </tbody>
</table>
