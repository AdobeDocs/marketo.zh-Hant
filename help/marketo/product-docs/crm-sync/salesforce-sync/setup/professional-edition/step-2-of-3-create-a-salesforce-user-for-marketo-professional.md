---
unique-page-id: 3571797
description: 第2步（共3步）-建立適用於行銷人員的Salesforce使用者（專業人員）-行銷人員檔案——產品檔案
title: 第2步（共3步）-建立適用於行銷人員的Salesforce使用者（專業人員）
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---


# 步驟2（共3步）:建立適用於行銷人員的Salesforce使用者（專業版） {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>這些步驟必須由Salesforce管理員完成

>[!PREREQUISITES]
>
>* [步驟1（共3步）:將行銷人員欄位新增至Salesforce（專業版）](step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

>



在本文中，您將使用Salesforce頁面配置來自訂欄位權限，並建立Marketo-Salesforce同步使用者。

## 設定頁面版面 {#set-page-layouts}

Salesforce Professional會使用「頁面版面」來設定欄位層級的協助工具，而非Salesforce Enterprise/Unlimited的「設定檔」。 依照這些步驟，Marketo將可讓使用者同步更新自訂欄位。

1. 在導 **覽列中輸入頁面** ，而不按 **Enter**，然後按一下Leads下方的「頁 **面配置******」。

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. 按一 **下** 「銷售線索配置」旁的「編輯」。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 按一下並拖曳新的 **「區段** 」至頁面版面。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. 在「區段名稱」中輸 **入「行銷人員** 」，然後按 **一下「確定**」。

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. 按一下並拖曳欄位「 **贏取日期** 」至 **Marketo區段** 。

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. 對下列欄位重複上述步驟：

   * 贏取計畫
   * 贏取計畫ID
   * 選擇退出電子郵件
   * 推斷城市
   * 推斷的公司
   * 推斷國家
   * 推斷的都市區
   * 推斷的電話區號
   * 推斷的郵遞區號
   * 推斷的州區
   * 銷售線索分數
   * 原始反向連結
   * 原始搜尋引擎
   * 原始搜尋片語
   * 原始來源資訊
   * 原始來源類型

   >[!NOTE]
   >
   >這些欄位必須位於頁面版面上，好讓Marketo能夠讀取／寫入。

   >[!TIP]
   >
   >拖曳至頁面右側，為欄位建立兩欄。 您可以將欄位從一側移至另一側，以平衡欄長。

1. 新增欄 **位後** ，按一下「儲存」。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. 對「Salesforce連絡人頁面配置」重複上述 **所有步驟**。

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. 使用「連絡 **人頁面** 」版面完成時，請記 **得按一下「儲存」**。

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >請確定「全 **天事件** 」欄位已新增至「事件 **頁面配置」**。

## 建立同步用戶 {#create-sync-user}

Marketo需要認證才能存取Salesforce。 使用以下步驟建立的專用使用者，最好能完成此作業。

>[!NOTE]
>
>如果您的組織沒有額外的Salesforce授權，您可以將現有的 **Marketing使用者與系統管** 理員設定檔一起使用 **** 。

1. 在導覽搜尋列中輸入「使用者」，然後按一下「管 **理使** 用 **者」下的「使用者」**。

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 按一 **下「新使用者**」。

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 填寫必填欄位，選取「使用者 **授權」:Salesforce**，請設定 **Profile:系統管理員**，勾選「 **行銷使用者** 」並按一 **下「儲存**」。

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >請確定您輸入的電子郵件地址有效。 您必須以同步使用者身分登入，才能重設密碼。

太棒了！ 現在，您擁有Marketo可用來連線至Salesforce的帳戶。 我們來吧。

>[!NOTE]
>
>**相關文章**
>
>* [步驟3（共3步）:將行銷人員與Salesforce（專業版）連結](step-3-of-3-connect-marketo-and-salesforce-professional.md)

>



