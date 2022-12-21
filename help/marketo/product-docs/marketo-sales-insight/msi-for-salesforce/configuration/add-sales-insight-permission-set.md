---
description: 新增Sales Insight權限集 — Marketo檔案 — 產品檔案
title: 添加Sales Insight權限集
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
source-git-commit: cccea2e9b7e1d0017e9be071ec85051f71e737bd
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# 添加Sales Insight權限集 {#add-sales-insight-permission-set}

使用下列步驟來新增對Salesforce中Sales Insight功能的存取權。 適用於Salesforce Classic和Lighting

>[!PREREQUISITES]
>
>[更新您的Sales Insight Salesforce套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;}到1.8000版或更高版本，以使用此功能。

>[!IMPORTANT]
>
>如果您先前已為所有用戶授予Sales Insight對所有配置檔案的訪問權和/或實施了Sales Insight，則必須 [移除設定檔層級存取權](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target=&quot;_blank&quot;}使用此權限集。

## 總覽 {#overview}

「Marketo應用程式」權限是Sales Insight Salesforce套件的一部分。 它包括對下列物件、頂端類別和視覺效果頁面的存取。 這些是訪問所有Sales Insight功能所必需的。

**物件設定**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>讀取、建立、編輯、刪除、全部查看、全部修改</td> 
  </tr> 
  <tr> 
   <td>最佳視圖詳細資訊</td> 
   <td>讀取、建立、編輯、刪除、全部查看、全部修改</td> 
  </tr> 
  <tr> 
   <td>最佳檢視</td> 
   <td>讀取、建立、編輯、刪除、全部查看、全部修改</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>讀取、建立、編輯、刪除、全部查看、全部修改</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>讀取、建立、編輯、刪除、全部查看、全部修改</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>讀取、建立、編輯、刪除、全部查看、全部修改</td> 
  </tr> 
  <tr> 
   <td>InterestedMomentsCache</td> 
   <td>讀取、建立、編輯、刪除、全部查看、全部修改</td> 
  </tr> 
  <tr> 
   <td>Marketo Sales Insight設定</td> 
   <td>讀取、建立、編輯、刪除、全部查看、全部修改</td> 
  </tr> 
  <tr> 
   <td>ScoringCache</td> 
   <td>讀取、建立、編輯、刪除、全部查看、全部修改</td> 
  </tr> 
  <tr> 
   <td>值</td> 
   <td>讀取、建立、編輯、刪除、全部查看、全部修改</td> 
  </tr> 
  <tr> 
   <td>WebActivityCache</td> 
   <td>讀取、建立、編輯、刪除、全部查看、全部修改</td> 
  </tr> 
 </tbody> 
</table>

* Apex類訪問：159個以&quot;mkto_si&quot;開頭的頂點類
* 視覺效果強制頁面存取：64以「mkto_si」開頭的視覺強制頁面
* 自訂設定定義：mkto_si.Marketo設定與mkto_si.User偏好設定

## 將Marketo應用程式權限集新增至使用者 {#adding-marketo-app-permission-set-to-users}

1. 登入您的Salesforce帳戶。

1. 按一下 **設定**.

   ![](assets/add-sales-insight-permission-set-1.png)

1. 在「管理員」下，按一下以展開 **管理使用者**，然後 **使用者**.

   ![](assets/add-sales-insight-permission-set-2.png)

1. 在「所有使用者」下，選取您要提供存取權的使用者，然後按一下 **權限集分配**.

   ![](assets/add-sales-insight-permission-set-3.png)

1. 按一下 **編輯分配**.

   ![](assets/add-sales-insight-permission-set-4.png)

1. 選擇 **Marketo應用程式存取** 從可用權限集，然後 **新增**. 按一下 **儲存**.

   ![](assets/add-sales-insight-permission-set-5.png)

1. 現在，當您向下捲動「使用者詳細資料」頁面時，權限集指派下會顯示「Marketo應用程式存取」。

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>無權存取Sales Insight的使用者會看到以下訊息：&quot;您沒有足夠的權限訪問此頁簽。&quot;

就這樣！ 您已成功新增Sales Insight存取權。 對您要為其新增存取權的任何其他設定檔重複相同步驟。
