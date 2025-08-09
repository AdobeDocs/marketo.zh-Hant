---
description: 使用者和授權管理 — Marketo檔案 — 產品檔案
title: 使用者和授權管理
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
feature: Interactive Webinars
source-git-commit: fe167b4a70a23f129d56ed20ac6c1ed1130049ef
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# 使用者和授權管理 {#user-and-license-management}

瞭解如何新增和移除使用者，以及檢視您目前的授權。

## 新增使用者 {#add-a-user}

1. 移至&#x200B;**管理員**&#x200B;區域。

   ![](assets/user-and-license-management-1.png)

1. 按一下&#x200B;**互動式網路研討會**。

   ![](assets/user-and-license-management-2.png)

1. 按一下&#x200B;**新增/移除使用者**。

   ![](assets/user-and-license-management-3.png)

1. 按一下「可用的使用者」下拉式清單，選取您要新增的使用者，然後按一下「確定」****。

   ![](assets/user-and-license-management-4.png)

## 移除使用者 {#remove-a-user}

1. 移至&#x200B;**管理員**&#x200B;區域。

   ![](assets/user-and-license-management-5.png)

1. 按一下&#x200B;**互動式網路研討會**。

   ![](assets/user-and-license-management-6.png)

1. 按一下&#x200B;**新增/移除使用者**。

   ![](assets/user-and-license-management-7.png)

1. 反白您要移除的使用者，然後按鍵盤上的Delete鍵。 完成時，按一下&#x200B;**確定**。

   ![](assets/user-and-license-management-8.png)

## 授權使用情況 {#license-usage}

互動式網路研討會提供特定授權，可建立由Adobe Connect支援的事件。 每次新增授權時，都會顯示新的授權使用方塊。 Marketo管理員可依照下列步驟檢視（而非編輯）授權。 聯絡Adobe客戶團隊（您的客戶經理）以取得其他授權。

1. 移至&#x200B;**管理員**&#x200B;區域。

   ![](assets/user-and-license-management-9.png)

1. 按一下&#x200B;**互動式網路研討會**。

   ![](assets/user-and-license-management-10.png)

1. 向下捲動至「授權使用」卡。

   ![](assets/user-and-license-management-11.png)

<table>
  <tr>
   <td width="20%"><b>開始日期</b></td>
   <td width="80%">授權開始日期。</td>
  </tr>
  <tr>
   <td width="20%"><b>到期日</b></td>
   <td width="80%">授權到期日。</td>
  </tr>
  <tr>
   <td width="20%"><b>類型</b></td>
   <td width="80%">購買的授權型別。 可用的型別有三種：共用事件授權、共用房間授權、其他儲存空間授權。</td>
  </tr>
  <tr>
   <td width="20%"><b>事件容量</b></td>
   <td width="80%">事件中可容納的最大參與者人數。</td>
  </tr>
  <tr>
   <td width="20%"><b>事件總數</b></td>
   <td width="80%">已使用此授權布建的事件總數。</td>
  </tr>
  <tr>
   <td width="20%"><b>使用的事件</b></td>
   <td width="80%">所有已完成和目前排程的事件。 <a href="#things-to-note">了解更多</a></td>
  </tr>
  <tr>
   <td width="20%"><b>儲存容量</b></td>
   <td width="80%">可用於儲存錄製、抵押品、主圖影像、檔案和其他資產的儲存空間。</td>
  </tr>
  </tbody>
</table>

### 注意事項 {#things-to-note}

* 每次建立事件時，都會將其個別授權計為「已使用」（除非其為共用房間授權）。 如果同時有相同容量的「共用事件授權」和「共用房間授權」，則會將「共用事件授權」指定給偏好設定。 如果事件尚未傳遞，且在排程時間之前刪除了事件程式，則會補充事件計數。 如果事件未傳遞，且在排程時間之前未刪除事件程式，則不會補充事件。

* 型別「額外儲存授權」僅提供儲存空間，因此&#x200B;_儲存容量以外的每個欄位_&#x200B;中的值將僅列為「 — 」。

* 「共用房間授權」型別有不限數量的事件，而「其他儲存空間授權」僅提供儲存空間，因此這些授權的「事件總數」欄位將僅列為「 — 」。

* 授權耗盡後，其圖磚會保留在「管理員」區段的「互動式網路研討會」畫面中，「總事件」和「消費的事件」會有相同的值。 只有當授權到期時，才會從畫面中移除授權。

## 使用者存取 {#user-access}

互動式網路研討會可授予Marketo Engage使用者建立和傳遞互動式網路研討會的許可權，進而具備規範使用情形的功能。 但是，互動式網路研討會使用者（或非使用者）仍可讀取/編輯其他使用者建立的互動式網路研討會事件程式。

擁有互動式網路研討會許可權且擁有特定互動式網路研討會活動計畫的Marketo使用者，將可執行與該計畫相關的所有互動式網路研討會功能。 這包括：建立、存取、修改、複製、移動和刪除該程式。 但是，一旦該使用者不再是互動式網路研討會使用者，方案所有者將能夠存取和移動方案，但不能執行任何其他功能。

已獲得互動式網路研討會許可權且擁有特定互動式網路研討會活動計畫之&#x200B;_非_&#x200B;所有者的Marketo使用者，將能在這些計畫上執行有限的功能。 Marketo的非管理員使用者將能夠存取及復製程式，但如果他們擁有互動式網路研討會的許可權，則將無法執行任何其他功能。 不過，Marketo Admin使用者&#x200B;_將_&#x200B;能夠執行所有功能，例如存取、修改、複製、移動和刪除該程式（只要他們擁有互動式網路研討會的許可權）。 在撤銷Marketo管理員和非管理員使用者的此許可權後，他們將無法僅存取互動式網路研討會活動計畫，也無法執行任何其他功能。

可操作函式的限制會以灰色的動作按鈕和暫留訊息表示。 灰色動作按鈕的部分範例為「設計您的網路研討會」或「輸入您的網路研討會」。 對於不可操作的功能，將會顯示一則訊息，強調限制。 請參閱下列範例：

![](assets/user-and-license-management-12.png)
