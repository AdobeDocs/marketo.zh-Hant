---
unique-page-id: 1147031
description: 從SFDC刪除人員 — Marketo檔案 — 產品檔案
title: 從SFDC中刪除人員
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# 從SFDC中刪除人員 {#delete-person-from-sfdc}

如果您需要從Salesforce中刪除一組特定的銷售線索，但將其保留為Marketo中的人員，則可以使用「從SFDC流中刪除人員」操作。

>[!NOTE]
>
>僅在與Salesforce整合時可用。

1. 在資料庫中，按一下要從Salesforce中刪除的人員。 然後按一下 **人員動作** 選取 **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. 選擇 **從SFDC中刪除人員**.

   ![](assets/delete-person-from-sfdc.png)

1. 請確定 **在Marketo中刪除** 設定 **false**，然後按一下 **立即運行**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   流程步驟執行後，您的人員將不再是Salesforce中的主管，但將保留在Marketo。

   >[!CAUTION]
   >
   >如果您設定 **在Marketo中刪除** to **true** 刪除Marketo的人員和Salesforce的銷售線索，他們就永遠消失了。 這無法復原。
