---
description: 許可權 — Marketo檔案 — 產品檔案
title: 權限
feature: Dynamic Chat
exl-id: 06798ac4-636b-476e-bbb1-498062844406
source-git-commit: 38e1e2d8c2fef7163f77d7774837571008075b5f
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 4%

---

# 權限 {#permissions}

共有五個預設設定檔具有預先定義的許可權，您可以在Dynamic Chat中編輯。 您也可以建立具有自訂許可權集的自訂設定檔。 我們來看看這兩個。

## 編輯現有許可權 {#edit-existing-permissions}

1. 在[Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}中，按一下&#x200B;**Dynamic Chat**。

   ![](assets/permissions-1.png)

1. 在&#x200B;**產品設定檔**&#x200B;索引標籤中，選取您要編輯的設定檔。 在此範例中，我們選擇&#x200B;**即時代理程式**。

   ![](assets/permissions-2.png)

1. 按一下「**許可權**」標籤。

   ![](assets/permissions-3.png)

1. 選取要編輯的設定檔區域。 在此範例中，我們選擇「即時交談」。 按一下鉛筆圖示。

   ![](assets/permissions-4.png)

1. 可用的許可權專案會列在左側。 您可以選擇逐一新增許可權，或一次新增所有許可權。 按一下&#x200B;**+**&#x200B;符號。

   ![](assets/permissions-5.png)

   >[!NOTE]
   >
   >啟用自動包含會將所有許可權專案新增至包含的清單。 當新的許可權專案可用時，會自動納入該產品設定檔中。

1. 按一下&#x200B;**儲存**。

   ![](assets/permissions-6.png)

您現在可以為任何/所有其他Dynamic Chat區域重複此程式。

![](assets/permissions-7.png)

## 建立設定檔 {#create-a-profile}

1. 在[Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}中，按一下&#x200B;**Dynamic Chat**。

   ![](assets/permissions-8.png)

1. 在&#x200B;**產品設定檔**&#x200B;索引標籤中，按一下&#x200B;**新增設定檔**。

   ![](assets/permissions-9.png)

1. **為您的產品設定檔命名**。 您可以選擇為其提供顯示名稱和/或說明，並選擇在使用者新增/移除時通知使用者。 完成時，按一下&#x200B;**儲存**。

   ![](assets/permissions-10.png)

1. 您的新設定檔會出現在產品設定檔索引標籤中。 選取它。

   ![](assets/permissions-11.png)

1. 現在，請對每個所需區域執行上述[區段](#edit-existing-permissions)中的步驟3-6。

## 許可權清單 {#list-of-permissions}

在下方，您會找到每個區域的所有可用許可權清單。

<table>
<thead>
  <tr>
    <th style="width:25%">Dynamic Chat區域</th>
    <th>權限</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>交談管理</td>
    <td><li>檢視對話方塊</li>
    <li>管理對話方塊（建立、刪除）</li>
    <li>Publish對話方塊</li>
    <li>檢視對話流程</li>
    <li>管理對話流程（建立、刪除）</li>
    <li>Publish對話流程</li></td>
  </tr>
  <tr>
    <td>即時聊天</td>
    <td><li>檢視我的交談</li>
    <li>檢視所有交談</li>
  </tr>
  <tr>
    <td>會議</td>
    <td><li>管理所有會議</li>
  </tr>
  <tr>
    <td>Analytics</td>
    <td><li>檢視全域效能報表</li>
    <li>檢視即時聊天報告</li>
    <li>檢視會議報告</li>
    <li>匯出報告</li></td>
  </tr>
  <tr>
    <td>專員設定</td>
    <td><li>管理即時聊天可用性</li>
    <li>連線您的行事曆</li>
    <li>管理行事曆可用性</li></td>
  </tr>
  <tr>
    <td>管理員設定</td>
    <td><li>檢視循環配置資源</li>
    <li>檢視自訂規則</li>
    <li>管理自訂規則（新增、編輯、刪除）</li>
    <li>檢視帳戶清單<b>*</b></li>
    <li>管理帳戶（新增、編輯、刪除） <b>*</b></li>
    <li>管理聊天機器人設定</li>
    <li>管理對話流程設定</li>
    <li>管理隱私權與安全性</li>
    <li>管理整合</li>
    <li>管理代理程式</li>
    <li>檢視代理程式群組<b>*</b></li>
    <li>管理代理程式團隊（新增、編輯、刪除） <b>*</b></li></td>
  </tr>
</tbody>
</table>

**&#42;**&#x200B;目前僅適用於Dynamic Prime使用者

<p>

## 預設設定檔許可權 {#default-profile-permissions}

以下是預設啟用的五個預設設定檔和許可權。

<table>
<thead>
  <tr>
    <th style="width:25%">設定檔</th>
    <th>預設許可權</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>行銷使用者</td>
    <td><i>交談管理</i>
    <li>檢視對話方塊</li>
    <li>管理對話方塊（建立、刪除）</li>
    <li>Publish對話方塊</li>
    <li>檢視對話流程</li>
    <li>管理對話流程（建立、刪除）</li>
    <li>Publish對話流程</li>
    <br>
    <i>即時交談</i>
    <li>不適用</li>
    <br>
    <i>會議</i>
    <li>不適用</li>
    <br>
    <i>分析</i>
    <li>檢視全域效能報表</li>
    <li>檢視即時聊天報告</li>
    <li>檢視會議報告</li>
    <br>
    <i>代理程式設定</i>
    <li>不適用</li>
    <br>
    <i>管理員設定</i>
    <li>檢視循環配置資源</li>
    <li>檢視自訂規則</li>
    <li>檢視帳戶清單<b>*</b></li>
    <li>檢視代理程式群組<b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>即時代理程式</b></td>
    <td><i>交談管理</i>
    <li>檢視對話方塊</li>
    <li>檢視對話流程</li>
    <br>
    <i>即時交談</i>
    <li>檢視我的交談</li>
    <br>
    <i>會議</i>
    <li>不適用</li>
    <br>
    <i>分析</i>
    <li>檢視全域效能報表</li>
    <li>檢視即時聊天報告</li>
    <li>檢視會議報告</li>
    <br>
    <i>代理程式設定</i>
    <li>管理即時聊天可用性</li>
    <li>連線您的行事曆</li>
    <li>管理行事曆可用性</li>
    <br>
    <i>管理員設定</i>
    <li>檢視循環配置資源</li>
    <li>檢視自訂規則</li>
    <li>檢視帳戶清單<b>*</b></li>
    <li>檢視代理程式群組<b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>行事曆代理程式</b></td>
    <td><i>交談管理</i>
    <li>檢視對話方塊</li>
    <li>檢視對話流程</li>
    <br>
    <i>即時交談</i>
    <li>不適用</li>
    <br>
    <i>會議</i>
    <li>不適用</li>
    <br>
    <i>分析</i>
    <li>檢視全域效能報表</li>
    <li>檢視即時聊天報告</li>
    <li>檢視會議報告</li>
    <br>
    <i>代理程式設定</i>
    <li>連線您的行事曆</li>
    <li>管理行事曆可用性</li>
    <br>
    <i>管理員設定</i>
    <li>檢視循環配置資源</li>
    <li>檢視自訂規則</li>
    <li>檢視帳戶清單<b>*</b></li>
    <li>檢視代理程式群組<b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>行銷管理員</b></td>
    <td><i>交談管理</i>
    <li>檢視對話方塊</li>
    <li>管理對話方塊（建立、刪除）</li>
    <li>Publish對話方塊</li>
    <li>檢視對話流程</li>
    <li>管理對話流程（建立、刪除）</li>
    <li>Publish對話流程</li>
    <br>
    <i>即時交談</i>
    <li>不適用</li>
    <br>
    <i>會議</i>
    <li>不適用</li>
    <br>
    <i>分析</i>
    <li>檢視全域效能報表</li>
    <li>檢視即時聊天報告</li>
    <li>檢視會議報告</li>
    <li>匯出報告</li>
    <br>
    <i>代理程式設定</i>
    <li>不適用</li>
    <br>
    <i>管理員設定</i>
    <li>檢視循環配置資源</li>
    <li>檢視自訂規則</li>
    <li>管理自訂規則（新增、編輯、刪除）</li>
    <li>檢視帳戶清單<b>*</b></li>
    <li>管理帳戶（新增、編輯、刪除） <b>*</b></li>
    <li>管理聊天機器人設定</li>
    <li>管理對話流程設定</li>
    <li>管理隱私權與安全性</li>
    <li>管理整合</li>
    <li>檢視代理程式群組<b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>銷售管理員</b></td>
    <td><i>交談管理</i>
    <li>檢視對話方塊</li>
    <li>檢視對話流程</li>
    <br>
    <i>即時交談</i>
    <li>檢視我的交談</li>
    <li>檢視所有交談</li>
    <br>
    <i>會議</i>
    <li>管理所有會議</li>
    <br>
    <i>分析</i>
    <li>檢視全域效能報表</li>
    <li>檢視即時聊天報告</li>
    <li>檢視會議報告</li>
    <li>匯出報告</li>
    <br>
    <i>代理程式設定</i>
    <li>管理即時聊天可用性</li>
    <li>連線您的行事曆</li>
    <li>管理行事曆可用性</li>
    <br>
    <i>管理員設定</i>
    <li>檢視循環配置資源</li>
    <li>檢視自訂規則</li>
    <li>管理自訂規則（新增、編輯、刪除）</li>
    <li>檢視帳戶清單<b>*</b></li>
    <li>管理帳戶（新增、編輯、刪除） <b>*</b></li>
    <li>管理代理程式</li>
    <li>檢視代理程式群組<b>*</b></li>
    <li>管理代理程式群組<b>*</b></li>
    </td>
  </tr>
</tbody>
</table>

**&#42;**&#x200B;目前僅適用於Dynamic Prime使用者
