---
description: 最新發行說明 - Marketo 文件 - 產品文件
title: 最新發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 2ae776fb67e590c4ccad711e4dfa55e6fc558c3b
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 2%

---

# 發行說明： 2024年10月 {#release-notes-oct-24}

下方提供2024年10月發行版本包含的所有功能。 檢查您的Adobe Marketo Engage版本是否有功能可用。

您可以在](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}找到專為Adobe Dynamic Chat[的發行說明。

>[!AVAILABILITY]
>
>以星號（![星號](assets/yellow-star.png)）表示的功能是付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2024年10月4日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行功能和日期可能會有所變更。 請檢查每個功能旁的狀態。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">狀態</th>
   <th style="width:25%">檔案</th>
  </tr>
    <tr> 
   <td><strong>互動式網路研討會參與儀表板的增強型註冊資料</strong>：您現在可以看到哪些公司的出席率最高，並在參與儀表板提供的報表中，以潛在客戶層級更新公司、職稱和產業。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
    <tr> 
   <td><strong>互動式網路研討會的權杖化</strong>：您現在可以使用權杖在電子郵件和登陸頁面中推廣互動式網路研討會，而無需手動新增網路研討會詳細資訊。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr> 
   <td><strong>智慧清單「設定為影響」計數</strong>：檢視編輯Smart Campaign的資格規則時會影響多少人。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr> 
   <td><strong>導覽邊欄中的「我的帳戶」按鈕</strong>：對於已移轉至AdobeIdentity Management系統的使用者，左側導覽邊欄中新的「我的帳戶」按鈕可讓您設定時區並存取訂閱詳細資料。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   <tr> 
   <td><strong>電子郵件效能報告增強功能</strong>：已針對電子郵件報告量度和活動追蹤進行多項改進，以提供其他深入分析並改善準確性。
   <ul>
   <li>從電子郵件效能量度篩選刪除和合併的人員</li>
   <li>電子郵件在等待回應活動三天後現在分類為<i>已中止</i></li>
   <li>在行銷活動層級開啟的帳戶電子郵件</li>
   <li>透過調整追蹤畫素位置改善電子郵件活動追蹤</li>
   </td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **QR碼淘汰**：自2024年10月4日起，推播通知和應用程式內訊息資產中使用的QR碼功能將被淘汰。 這包括使用新測試裝置的QR碼，以及使用QR碼建立新資產。 淘汰使用率較低的功能，可讓我們重新分配其資源，以便整體維護Marketo Engage。

* **Munchkin變更**

   * **新版本**：自2024年9月17日起，[Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164將開始推出以Marketo Engage在&#x200B;**Admin** > **Treasure Chest**&#x200B;中啟用「Munchkin Beta」設定的執行個體。 排程在10月29日開始推出至所有其他執行個體。 此版本會更新Munchkin Cookie的建立。 功能沒有變更。

   * **已移除URL中的字元**： Munchkin JS建立的「瀏覽網頁」和「點按連結」活動現在會移除所有URL欄位中的非URL編碼控制字元。 此變更旨在防止這些型別的字元傳播到不支援這些字元且在Marketo Engage中沒有有效使用的系統時發生錯誤。
