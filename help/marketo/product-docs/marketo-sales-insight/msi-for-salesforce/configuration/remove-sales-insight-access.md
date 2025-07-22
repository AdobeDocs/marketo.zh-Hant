---
description: 移除銷售Insight存取權 — Marketo檔案 — 產品檔案
title: 移除銷售Insight存取權
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 3%

---

# 移除[!DNL Sales Insight]存取權 {#remove-sales-insight-access}

使用以下步驟，移除對[!DNL Sales Insight]中[!DNL Salesforce]功能的存取權。 適用於[!DNL Salesforce] Classic和Lightning。

## 概觀 {#overview}

存取所有[!DNL Sales Insight]功能需要下列物件、Apex類別和Visualforce頁面的許可權。 移除這些專案將會移除[!DNL Sales Insight]的存取權。

**物件設定**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>[!DNL Best Bets] 檢視詳細資料</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>[!DNL Best Bets] 檢視</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>InterestedMentsCache</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>[!DNL Marketo Sales Insight] 設定</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>評分快取</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>值</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>WebActivityCache</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
 </tbody> 
</table>

* Apex類別存取：以「mkto_si」開頭的159個Apex類別
* Visualforce頁面存取：64個以「mkto_si」開頭的Visualforce頁面
* 自訂設定定義：mkto_si.Marketo設定和mkto_si.User偏好設定

## 正在移除[!DNL Sales Insight]的存取權 {#removing-access-to-sales-insight}

1. 登入您的[!DNL Salesforce]帳戶。

1. 按一下「**[!UICONTROL Setup]**」。

   ![](assets/remove-sales-insight-access-1.png)

1. 在[!UICONTROL Administrator]底下，按一下&#x200B;**[!UICONTROL Manage Users]**，然後按&#x200B;**[!UICONTROL Profiles]**。

1. 按一下您要更新的設定檔，然後&#x200B;**[!UICONTROL Edit]**。

1. 向下捲動至「[!UICONTROL Custom Tab Settings]」下的「[!UICONTROL Tab Settings]」。

1. 從[!UICONTROL Tab Hidden] Config和MSI [!DNL Marketo Sales Insight]寄件匣的下拉式清單中選取「[!DNL Marketo Sales]」選項。

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. 向下捲動至&quot;[!UICONTROL Custom Object Permissions]&quot;。

1. 移除下列物件的「讀取、建立、編輯、刪除」存取權：

   * BestBetsCache
   * [!DNL Best Bets]檢視詳細資料
   * [!DNL Best Bets]個檢視
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestedMentsCache
   * [!DNL Marketo Sales Insight]設定
   * 評分快取
   * 值
   * WebActivityCache

1. 向下捲動至&quot;[!UICONTROL Enabled Apex Class Access]&quot;區段。 按一下「**[!UICONTROL Edit]**」。

1. 從&quot;[!UICONTROL Enabled Apex Classes]&quot;區段中，選取所有以&quot;mkto_si&quot;開頭的類別。 這最多可新增159個類別。

1. 按一下&#x200B;**[!UICONTROL Remove]**，然後按&#x200B;**[!UICONTROL Save]**。

   ![](assets/remove-sales-insight-access-4.png)

1. 向下捲動至[!UICONTROL Enabled Visualforce Page Access]區段。 按一下「**[!UICONTROL Edit]**」。

1. 從「[!UICONTROL Enabled Visualforce Pages]」區段中，選取所有以「mkto_si」開頭的頁面。 最多可新增64頁。

1. 按一下&#x200B;**[!UICONTROL Remove]**，然後按&#x200B;**[!UICONTROL Save]**。

   ![](assets/remove-sales-insight-access-5.png)

1. 向下捲動至&quot;[!UICONTROL Enabled Custom Setting Definitions Access]&quot;區段。 按一下「**[!UICONTROL Edit]**」。

1. 選取「Marketo Sales Insight.mkto_si.Marketo設定」和「Marketo Sales Insight.mkto_si.User偏好設定」。

1. 按一下&#x200B;**[!UICONTROL Remove]**，然後按&#x200B;**[!UICONTROL Save]**。

   ![](assets/remove-sales-insight-access-6.png)

完成了！您已成功移除[!DNL Sales Insight]存取權。 對您要移除其存取權的任何其他設定檔重複相同的步驟。
