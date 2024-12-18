---
description: 最新發行說明 - Marketo 文件 - 產品文件
title: 最新發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: bf6525359d8bc206ed01220823b6c1de5734df55
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 2%

---

# 發行說明： 2025年1月 {#release-notes-jan-25}

以下是2025年1月發行版本包含的所有功能。 檢查您的Adobe Marketo Engage版本是否有功能可用。

您可以在](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}找到專為Adobe Dynamic Chat[的發行說明。

>[!AVAILABILITY]
>
>以星號（![星號](assets/yellow-star.png)）表示的功能是付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2025年1月17日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行功能和日期可能會有所變更。 請檢查每個功能旁的狀態。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">狀態</th>
   <th style="width:25%">檔案</th>
  </tr>
    <tr> 
   <td><strong>新電子郵件Designer</strong>：使用Marketo Engage中的新原生電子郵件Designer建立現代且有效的電子郵件。 存取其中一個預先設計的現成電子郵件範本，或輕鬆建立您自己的範本。 使用動態內容並從Adobe Experience Manager雲端服務存取影像。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>在互動式網路研討會中取消註冊註冊者</strong>：現在，如果您由於任何原因不想讓註冊者參加網路研討會，可以取消註冊。 工作流程會從Marketo事件計畫和Adobe Connect中移除註冊者。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>停用封存的行銷活動</strong>：停用作用中觸發行銷活動，並在封存時取消資料夾中行銷活動的任何排程批次執行。 由於對包含有效行銷活動的封存資料夾有額外的許可權檢查（啟用觸發行銷活動和排程批次行銷活動），因此此功能在此版本中預設為停用，並可在您的Marketo Engage訂閱中導覽至<b>管理員</b> &gt; <b>Treasure Chest</b>來啟用。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **取得方案成員API更新**：我們已增強[取得方案成員](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} API以支援擷取方案成員識別碼的功能。 做法是將ID新增至API請求的欄位引數中指定的欄位清單中。

* **Rest API &#39;access_token&#39;引數淘汰**：用於驗證Marketo REST API呼叫的`access_token`查詢引數已淘汰，並將於2025年6月30日後無法使用。 所有新的和現有的整合應該使用&#39;Authorization&#39;標頭[驗證REST API呼叫，如此處所述](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API淘汰**：對Marketo SOAP API的支援將於2025年10月31日結束。 使用SOAP API功能的服務應該移轉至[REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
