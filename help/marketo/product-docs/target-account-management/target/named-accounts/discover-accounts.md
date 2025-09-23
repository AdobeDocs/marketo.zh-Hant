---
unique-page-id: 11378812
description: 探索帳戶 — Marketo檔案 — 產品檔案
title: 探索帳戶
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
feature: Target Account Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 1%

---

# 探索帳戶 {#discover-accounts}

使用Discover選項來識別潛在的目標帳戶。

## [!UICONTROL Discover CRM Accounts] {#discover-crm-accounts}

從您的CRM識別潛在目標帳戶。

>[!NOTE]
>
>將CRM連線至Marketo TAM後，**[!UICONTROL Discover CRM Accounts]**&#x200B;會顯示所有CRM帳戶和相關資訊，協助您選擇正確的具名帳戶。 Marketo會針對從CRM收到的內容新增其他資訊。

**[!UICONTROL People]** （在[!UICONTROL Discover CRM Accounts]和[!UICONTROL Discover Marketo Companies]中）：包含連絡人和潛在客戶。 可使用Marketo的[銷售線索與帳戶的比對](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)來探索銷售線索。

**[!UICONTROL Potential People]** （在[!UICONTROL Discover CRM Accounts]和[!UICONTROL Discover Marketo Companies]中）：顯示Marketo找到多少潛在客戶可能屬於CRM帳戶。

**自訂CRM欄位** （僅適用於Discover CRM帳戶）：這可協助您調整銷售和行銷組織，以選取正確的目標帳戶。 使用Marketo TAM [對應自訂CRM欄位](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md)後，我們將顯示對應的資料，以協助您識別目標帳戶。

1. 在[!UICONTROL Named Accounts]中，按一下&#x200B;**[!UICONTROL New]**&#x200B;下拉式清單並選取&#x200B;**[!UICONTROL Discover CRM Accounts]**。

   ![](assets/disc-crm-one.png)

1. 將會開啟新視窗/標籤。 選取您要新增至[!UICONTROL Named Accounts]的CRM帳戶，然後按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/disc-crm-two.png)

1. 預覽畫面會確認您選擇的數量。 按一下「**[!UICONTROL Create]**」。

   ![](assets/disc-three.png)

   這就是所有步驟！

   ![](assets/disc-four.png)

## [!UICONTROL Discover Marketo Companies] {#discover-marketo-companies}

識別目標定位的正確公司。

>[!NOTE]
>
>在[!UICONTROL Discover Marketo Companies]中，您會看到並非來自您CRM的Marketo公司。

1. 在[!UICONTROL Named Accounts]中，按一下&#x200B;**[!UICONTROL New]**&#x200B;下拉式清單並選取&#x200B;**[!UICONTROL Discover Marketo Companies]**。

   ![](assets/one-1.png)

1. 將會開啟新視窗/標籤。 選取您要新增至[!UICONTROL Named Accounts]的公司，然後按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >在[!UICONTROL Discover Marketo Companies]和探索CRM中，Marketo會自動：
   >
   >* 從您的Marketo資料庫中尋找記錄中列出該公司的人員。 如果您看到某些屬性（例如「產業」）的多個值，是因為Marketo發現針對這些個人列出的不同值。 點選次數最多的屬性會獲勝
   >
   >僅在&#x200B;**探索CRM**&#x200B;中，Marketo會自動：
   >
   >* 同步並關聯CRM連絡人與[!UICONTROL Named Account]
   >
   >僅在&#x200B;**[!UICONTROL Discover Marketo Companies]**&#x200B;中，Marketo會自動：
   >
   >* 將大多數網際網路服務提供者和公用網域(例如yahoo.com、gmail.com)篩選為公司名稱
   >
   >* 刪除CRM帳戶的重複專案。 如果您有一筆記錄中有「Acme」且「Acme Inc」（或下列任一尾碼：Co， Corp， Corporation， Gmbh， Inc， Incorporated， LLC， LLP， LP， Ltd， PA， PC， PLC， PLLC），我們會將它們合併到TAM中，就像「Acme」一樣

1. 按一下[!UICONTROL Named Account]欄下方的向下箭頭以顯示下拉式清單。

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >今後，這些選定公司中的任何新人員都會自動指派給其個別具名帳戶。 請仔細檢查這些公司，並確定已將它們指派給正確的[!UICONTROL Named Account]。

1. 若要選取現有的帳戶，請按一下&#x200B;**[!UICONTROL Named Account]**&#x200B;下拉式清單，選擇想要的帳戶，然後按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/disc-comp-four.png)

   您也可以選擇直接在下拉式方塊中輸入所要的名稱，以建立新的[!UICONTROL Named Account]。 完成時，按一下離開方塊……

   ![](assets/disc-comp-five.png)

   ...您將會看到新的[!UICONTROL Named Account]。 此時，只要按一下步驟4中的&#x200B;**[!UICONTROL Next]** （類似）即可。

   ![](assets/disc-comp-six.png)

1. 按一下「**[!UICONTROL Create]**」。

   ![](assets/disc-comp-seven.png)

   做得好！

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>如果您看到選取的CRM帳戶與Discover CRM格線中的帳戶不相符，可能是因為下列一或多個原因：
>
>* 擁有名稱類似，但已進行重複資料刪除的不同CRM帳戶
>* 下一個排定的同步尚未發生

>[!MORELIKETHIS]
>
>[銷售機會帳戶相符](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
