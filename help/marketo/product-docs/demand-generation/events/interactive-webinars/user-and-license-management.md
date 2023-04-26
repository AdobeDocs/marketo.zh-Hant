---
description: 使用者與授權管理 — Marketo檔案 — 產品檔案
title: 使用者和授權管理
hide: true
hidefromtoc: true
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
source-git-commit: f60c40441be4bcfcc277b620f6d4e19b2047caef
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 使用者和授權管理 {#user-and-license-management}

簡介。

## 新增使用者 {#add-a-user}

1. 前往 **管理** 的上界。

   ![](assets/user-and-license-management-1.png)

1. 按一下 **互動式網路研討會**.

   ![](assets/user-and-license-management-2.png)

1. 按一下 **添加/刪除用戶**.

   ![](assets/user-and-license-management-3.png)

1. 按一下「可用使用者」下拉式清單，選取您要新增的使用者，然後按一下 **確定**.

   ![](assets/user-and-license-management-4.png)

## 移除使用者 {#remove-a-user}

1. 前往 **管理** 的上界。

   ![](assets/user-and-license-management-5.png)

1. 按一下 **互動式網路研討會**.

   ![](assets/user-and-license-management-6.png)

1. 按一下 **添加/刪除用戶**.

   ![](assets/user-and-license-management-7.png)

1. 選中要刪除的用戶，然後按鍵盤上的Delete鍵。 按一下 **確定** 時才能使用。

   ![](assets/user-and-license-management-8.png)

## 授權使用 {#license-usage}

互動式網路研討會提供建立Adobe Connect活動的特定授權。 每次新增授權時，都會出現新的授權使用方塊。 Marketo管理員可依照下列步驟檢視（非編輯）授權。 請連絡Adobe客戶團隊（您的客戶經理）以取得其他授權。

1. 前往 **管理** 的上界。

   ![](assets/user-and-license-management-9.png)

1. 按一下 **互動式網路研討會**.

   ![](assets/user-and-license-management-10.png)

1. 向下捲動至「License Usage（許可證使用）」卡。

   ![](assets/user-and-license-management-11.png)

<table> 
  <tr> 
   <td><b>開始日期</b></td>
   <td>許可的開始日期。</td>
  </tr>
  <tr> 
   <td><b>到期日</b></td>
   <td>許可證過期的日期。</td>
  </tr>
  <tr> 
   <td><b>類型</b></td>
   <td>購買的授權類型。 可用的類型有三種：共用事件許可證、共用室許可證、其他儲存許可證。</td>
  </tr>
  <tr> 
   <td><b>事件容量</b></td>
   <td>可在事件中容納的參與者人數上限。</td>
  </tr>
  <tr> 
   <td><b>事件總計</b></td>
   <td>已使用此授權布建的事件總數。</td>
  </tr>
  <tr> 
   <td><b>使用的事件</b></td>
   <td>已完成事件的總數。</td>
  </tr>
  <tr> 
   <td><b>儲存容量</b></td>
   <td>可用於儲存記錄、抵押物、hero images、文檔和其他資產的儲存量。</td>
  </tr>
  </tbody>
</table>

**注意事項**

* 「其他儲存許可證」類型只提供儲存，因此每個欄位中的值 _bess_ 儲存容量將僅列為「 — 」。

* 「共用室許可證」類型具有不限數量的事件，而「其他儲存許可證」僅提供儲存，因此這些許可證的「事件總數」欄位將僅列為「 — 」。

* 每次建立事件時，都會從其各自的許可證（除非是共用室許可證）計算為「已使用」。 如果「共用事件許可證」和「共用室許可證」具有相同容量，則將優先選擇「共用事件許可證」。 如果尚未傳送事件，並且在排程時間之前刪除了事件程式，則會從已使用的事件中減去事件來補充事件計數。

* 一旦授權用盡後，其圖磚會保留在「管理員」的「互動式網路研討會」畫面上，其中使用的事件和事件總數會具有相同的值。 只有當授權過期時，才會從畫面中移除。
