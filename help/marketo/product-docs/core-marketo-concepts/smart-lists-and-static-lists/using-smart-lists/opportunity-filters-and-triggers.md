---
unique-page-id: 8159286
description: 機會篩選和觸發器-Marketo文檔——產品文檔
title: 業務機會篩選器和觸發器
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Opportunity Filters和觸發器{#opportunity-filters-and-triggers}

業務機會篩選和觸發器可讓您從Salesforce追蹤業務機會事件。 與其他篩選器和觸發器相比，它們有些不同。

## 業務機會篩選器{#opportunity-filters}

業務機會篩選可讓您深入瞭解擁有業務機會的Salesforce客源。 編輯智慧清單時，可在元件面板的Opportunities資料夾中找到它們。 它們有幾種口味。

* Optys數
* 產品總額
* 預計總營收
* 有機會
* 已添加機會
* 已刪除機會
* 已更新業務機會

如果您正在查找Opportunity欄位（自定義或標準），請使用&#x200B;**Has Opportunity**&#x200B;篩選器或&#x200B;**Opportunity was`[Added/Removed/Updated]`**&#x200B;篩選器或觸發器。

**選件數、選件總額、預計選件總收入**

使用這些篩選器，您可以根據銷售機會的總數、金額或預期收入來尋找銷售機會。

![](assets/image2015-6-11-12-3a29-3a34.png)

**Has Opportunity（已添加到Opportunity中）已從Opportunity中刪除**

如果您正在查找基於條件組合而具有機會的潛在客戶，請使用&#x200B;**Has Opportunity** 、 **Was Added to Opportunity**&#x200B;或&#x200B;**Was Removed from Opportunity**&#x200B;篩選器。 他們告訴你：

* **有機會**:如果此銷售線索當前有任何匹配的機會
* **已添加到Opportunity**:如果此銷售機會已添加到匹配的銷售機會中
* **已從Opportunity中刪除**:如果此銷售機會從匹配的銷售機會中刪除

在篩選器上將搜尋准則新增為&#x200B;**Constraints**。 限制包括您的業務機會標準和自定義欄位：

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

例如，假設您想要尋找機會至少$5,000的潛在客戶。 在&#x200B;**Has Opportunity**&#x200B;過濾器中拖動並使用&#x200B;**Is Closed**&#x200B;和&#x200B;**Amount**&#x200B;約束：

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>當您使用多個Opportunity篩選器時，可能會得到不正確的答案。 如果您使用兩個Opportunity篩選器構建上述示例，您將得到一個銷售機會清單，這些銷售機會至少為$5,000，而所有銷售機會都已關閉，即使這些銷售機會是單獨的。

**已更新業務機會**

**Opportunity was Updated**&#x200B;篩選器會在特定的opportunity欄位更新時查找任何機會。 選擇要檢查的欄位，然後使用約束縮小更改集。

例如，此篩選器將顯示在過去30天內有關閉日期變更的所有銷售線索：

![](assets/image2015-6-11-12-3a33-3a7.png)

## 業務機會觸發器{#opportunity-triggers}

可以使用以下機會觸發器。 它們的運作方式與對應的篩選器（如前所述）相同，只不過它們可在事件發生時直接觸發促銷活動：

* 業務機會已更新
* 添加到Opportunity
* 從Opportunity中刪除

例如，您可以使用此智慧清單在任何銷售線索添加到任何業務機會時觸發。 在流程中，您可以將其新增至「暫停行銷」清單，或傳送定位電子郵件給他們。

![](assets/image2015-6-11-12-3a33-3a48.png)

要觸發業務機會自定義欄位，請使用&#x200B;**Opportunity is Updated**&#x200B;觸發器並選擇下拉式清單中的欄位：

![](assets/image2015-6-11-12-3a33-3a34.png)
