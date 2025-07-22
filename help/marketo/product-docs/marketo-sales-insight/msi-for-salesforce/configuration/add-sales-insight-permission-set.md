---
description: 新增銷售Insight許可權集 — Marketo檔案 — 產品檔案
title: 新增銷售Insight許可權集
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 1%

---

# 新增[!DNL Sales Insight]許可權集 {#add-sales-insight-permission-set}

使用以下步驟，新增對[!DNL Sales Insight]中[!DNL Salesforce]功能的存取權。 適用於[!DNL Salesforce]傳統及燈光

>[!PREREQUISITES]
>
>[將您的 [!DNL Sales Insight] [!DNL Salesforce]封裝](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}更新至1.8000版或更新版本，以使用此功能。

>[!IMPORTANT]
>
>如果您先前已授予[!DNL Sales Insight]所有設定檔的存取權和/或為您所有使用者實作[!DNL Sales Insight]，則您必須[移除設定檔層級的存取權](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"}才能使用此許可權集。

## 概觀 {#overview}

「Marketo應用程式」許可權是[!DNL Sales Insight] [!DNL Salesforce]套件的一部分。 其中包含下列提及物件、頂點類別和visualforce頁面的存取權。 若要存取所有[!DNL Sales Insight]功能，這些是必要的。

**物件設定**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>最佳化檢視詳細資料</td> 
   <td>讀取、建立、編輯、刪除、檢視全部、修改全部</td> 
  </tr> 
  <tr> 
   <td>最佳化檢視</td> 
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
   <td>Marketo [!DNL Sales Insight]設定</td> 
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

## 新增Marketo應用程式許可權集至使用者 {#adding-marketo-app-permission-set-to-users}

1. 登入您的[!DNL Salesforce]帳戶。

1. 按一下「**[!UICONTROL Setup]**」。

   ![](assets/add-sales-insight-permission-set-1.png)

1. 在「管理員」底下，按一下以展開&#x200B;**[!UICONTROL Manage Users]**，然後按一下&#x200B;**[!UICONTROL Users]**。

   ![](assets/add-sales-insight-permission-set-2.png)

1. 在[所有使用者]下，選取您要提供存取許可權的使用者，然後按一下[**[!UICONTROL Permission Set Assignments]**]。

   ![](assets/add-sales-insight-permission-set-3.png)

1. 按一下「**[!UICONTROL Edit Assignments]**」。

   ![](assets/add-sales-insight-permission-set-4.png)

1. 從可用的許可權集中選取&#x200B;**[!UICONTROL Marketo App Access]**，然後選取&#x200B;**[!UICONTROL Add]**。 按一下「**[!UICONTROL Save]**」。

   ![](assets/add-sales-insight-permission-set-5.png)

1. 現在，當您向下捲動「使用者詳細資訊」頁面時，會在「許可權集指派」下方看到「Marketo應用程式存取」。

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>沒有[!DNL Sales Insight]存取許可權的使用者將會看到此訊息：「您沒有足夠的許可權可存取此索引標籤。」

完成了！您已成功新增[!DNL Sales Insight]存取權。 對您要為其新增存取權的任何其他設定檔重複相同的步驟。
