---
description: 最新發行說明 - Marketo 文件 - 產品文件
title: 最新發行說明
hide: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
TQID: 'https://experienceleague.adobe.com/RZsCx9HAyJuDLO46WfshT30be-rMMDZjnygvU32NGfk'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
  - id: af97ce94-35fa-4fa9-b85a-46b752ac4028
    internal-label: Release information
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 9eb8c0e78a581bc9093f0f017a3ad3525d2b9667
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 18%
---
# 發行說明： 2026年10月 {#release-notes-oct-26}

您將會找到2026年10月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 標準發行週期功能 {#standard-release-cycle-features}

以下功能屬於標準發行週期，並將於&#x200B;**2026年10月23日**&#x200B;開始發行，並在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。 請查看各項功能旁邊的狀態。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>複製至此程式/資料夾</strong>：在Marketo Engage中復製作業現在會一致地提供「此資料夾」或「此程式」選項，作為選擇複製資產的目的地時的首要選擇。 選擇此選項會將資產複製到目前資產的父方案或資料夾。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <tr>
   <td><strong>CRM同步處理立即警示</strong>：啟用或停用環境的本機CRM同步處理現在會觸發通知，通知已訂閱CRM通知通道的使用者。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **棄用從網頁抓取影像**：為了符合現代安全性和隱私權的最佳實務，從10月發行版本起，[從網頁抓取影像](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"}功能將被棄用。

* **自訂活動屬性的API名稱限制**：透過API或UI建立的自訂活動屬性的API名稱現在只能包含英數字元和底線，而且必須以英數字元開頭。

* **取得潛在客戶活動與取得潛在客戶變更的靜態清單大小限制**：自2026年9月30日起，如果目標清單包含10,000個或更多潛在客戶，對含有`listId`引數的Get Lead Activities或Get Lead Changes端點的呼叫會以1003錯誤碼（表示目標靜態清單具有太多記錄）開始失敗。 如需詳細資訊，請參閱[移轉指南](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}。
