---
description: 用戶和許可證管理 — Marketo文檔 — 產品文檔
title: 用戶和許可證管理
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
source-git-commit: f3a6427520dff6f4e98bfe3c1afbc1b4fe5ea325
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 用戶和許可證管理 {#user-and-license-management}

瞭解如何添加和刪除用戶以及查看當前許可證。

## 添加用戶 {#add-a-user}

1. 轉到 **管理** 的子菜單。

   ![](assets/user-and-license-management-1.png)

1. 按一下 **互動式網路研討會**。

   ![](assets/user-and-license-management-2.png)

1. 按一下 **添加/刪除用戶**。

   ![](assets/user-and-license-management-3.png)

1. 按一下「可用用戶」(Available Users)下拉清單，選擇要添加的用戶，然後按一下 **確定**。

   ![](assets/user-and-license-management-4.png)

## 刪除用戶 {#remove-a-user}

1. 轉到 **管理** 的子菜單。

   ![](assets/user-and-license-management-5.png)

1. 按一下 **互動式網路研討會**。

   ![](assets/user-and-license-management-6.png)

1. 按一下 **添加/刪除用戶**。

   ![](assets/user-and-license-management-7.png)

1. 選中要刪除的用戶，然後按鍵盤上的刪除鍵。 按一下 **確定** 完成。

   ![](assets/user-and-license-management-8.png)

## 許可證使用 {#license-usage}

互動式網路研討會提供建立Adobe Connect活動的特定許可證。 每次添加許可證時，都會出現新的許可證使用框。 Marketo管理員可以按照以下步驟查看（不編輯）許可證。 聯繫Adobe客戶團隊（您的客戶經理）以獲取其他許可證。

1. 轉到 **管理** 的子菜單。

   ![](assets/user-and-license-management-9.png)

1. 按一下 **互動式網路研討會**。

   ![](assets/user-and-license-management-10.png)

1. 向下滾動到許可證使用卡。

   ![](assets/user-and-license-management-11.png)

<table> 
  <tr> 
   <td><b>開始日期</b></td>
   <td>許可證開始的日期。</td>
  </tr>
  <tr> 
   <td><b>到期日</b></td>
   <td>許可證過期的日期。</td>
  </tr>
  <tr> 
   <td><b>類型</b></td>
   <td>購買的許可證類型。 有三種類型可用：共用事件許可證、共用檔案室許可證、其他儲存許可證。</td>
  </tr>
  <tr> 
   <td><b>事件容量</b></td>
   <td>可在活動中容納的參與者的最大數量。</td>
  </tr>
  <tr> 
   <td><b>事件總數</b></td>
   <td>使用此許可證設定的事件總數。</td>
  </tr>
  <tr> 
   <td><b>已使用的事件</b></td>
   <td>已完成事件的總數。</td>
  </tr>
  <tr> 
   <td><b>儲存容量</b></td>
   <td>可用於儲存錄音、抵押物、hero images、文檔和其他資產的儲存量。</td>
  </tr>
  </tbody>
</table>

**要注意的事項**

* 「其他儲存許可證」類型只提供儲存，因此每個欄位中的值 _除_ 儲存容量將僅列為「 — 」。

* 「Shared Room License」類型具有無限制的事件，「Additional Storage License」僅提供儲存，因此這些許可證的「Total Events」欄位將僅列為「 — 」。

* 每次建立事件時，它都會從各自的許可證中被計算為「已使用」（除非它是共用房許可證）。 如果「共用事件許可證」和「共用室許可證」都具有相同容量，則將優先選擇「共用事件許可證」。 如果事件尚未傳送，並且在計畫時間之前刪除了事件程式，則通過從「已消耗事件」中減去事件來補充事件計數。

* 許可證用完後，其磁貼將保留在「管理」部分的「互動式網路研討會」螢幕上，「總事件」和「已使用事件」具有相同的值。 只有在許可證過期時，才會將其從螢幕中刪除。
