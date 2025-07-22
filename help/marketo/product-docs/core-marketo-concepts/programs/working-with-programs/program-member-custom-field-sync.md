---
description: 程式成員自訂欄位同步 — Marketo檔案 — 產品檔案
title: 程式成員自訂欄位同步
exl-id: 7facfc79-a411-4ad9-b847-2002763af5bb
feature: Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 6%

---

# 程式成員自訂欄位同步 {#program-member-custom-field-sync}

>[!PREREQUISITES]
>
>* 建立[方案成員自訂欄位](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md){target="_blank"}
>* [將 [!DNL Salesforce] 行銷活動與程式同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}

>[!NOTE]
>
>程式成員物件最多可以有20個自訂欄位。 這些欄位適用於任何計畫。

## 將Salesforce欄位對應到方案成員自訂欄位 {#map-salesforce-fields-to-program-member-custom-fields}

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/program-member-custom-field-sync-1.png)

1. 按一下&#x200B;**[!DNL Salesforce]**，然後按一下[程式成員自訂欄位同步]旁的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/program-member-custom-field-sync-2.png)

1. 使用搜尋方塊來找出您要對應的[!DNL Salesforce]欄位。 在此範例中，我們使用「請勿呼叫」。

   ![](assets/program-member-custom-field-sync-3.png)

1. 按一下下拉式清單。

   ![](assets/program-member-custom-field-sync-4.png)

1. 選擇要對應的Marketo [!UICONTROL Program Member Custom Field]。

   ![](assets/program-member-custom-field-sync-5.png)

   >[!NOTE]
   >
   >下拉式清單只會顯示符合[!UICONTROL Program Member Custom Fields]欄位資料型別的[!DNL Salesforce]。

1. 如需其他欄位對應，請清除搜尋方塊並重複步驟3到5。

1. 完成時，按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/program-member-custom-field-sync-6.png)

   >[!IMPORTANT]
   >
   >對對應欄位上的方案成員資料所做的變更，日後將會在Marketo和[!DNL Salesforce]之間同步。

   >[!NOTE]
   >
   >如果您重新命名或變更[!DNL Salesforce]中欄位的資料型別，我們將以[!UICONTROL Program Member Custom Field]移除該欄位的所有對應。 但您可在檢閱後使用新欄位將其重新對應。

## 從方案成員自訂欄位中取消對應Salesforce欄位 {#unmap-salesforce-fields-from-program-member-custom-fields}

如果您想釋放欄位來取代它，或只是進行一般變更，則必須先執行取消對應。 方法如下。

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/program-member-custom-field-sync-7.png)

1. 按一下&#x200B;**[!DNL Salesforce]**，然後按一下[程式成員自訂欄位同步]旁的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/program-member-custom-field-sync-8.png)

1. 使用搜尋方塊來找出您要取消對應的欄位。 在此範例中，我們使用「請勿呼叫」。

   ![](assets/program-member-custom-field-sync-9.png)

   >[!TIP]
   >
   >您可以選取「**[!UICONTROL Mapped]**」核取方塊以僅檢視對應的欄位。

1. 按一下欄位旁的&#x200B;**X**&#x200B;以取消對應。

   ![](assets/program-member-custom-field-sync-10.png)

1. 對應現已移除。 按一下「**[!UICONTROL Save]**」。

   ![](assets/program-member-custom-field-sync-11.png)

## 資料型別對應 {#data-type-mapping}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>SFDC資料型別</th>
      <th>程式成員自訂欄位資料型別</th>
    </tr>
    <tr>
      <td>文字</td>
      <td>字串</td>
    </tr>
    <tr>
      <td>挑選清單</td>
      <td>字串</td>
    </tr>
    <tr>
      <td>多選挑選清單</td>
      <td>字串</td>
    </tr>
    <tr>
      <td>電話</td>
      <td>字串</td>
    </tr>
    <tr>
      <td>電子郵件</td>
      <td>字串</td>
    </tr>
    <tr>
      <td>數字(m)</td>
      <td>整數</td>
    </tr>
    <tr>
      <td>數字(m，n)</td>
      <td>浮點數</td>
    </tr>
    <tr>
      <td>核取方塊</td>
      <td>布林值</td>
    </tr>
    <tr>
      <td>URL</td>
      <td>URL</td>
    </tr>
    <tr>
      <td>日期</td>
      <td>日期</td>
    </tr>
    <tr>
      <td>日期時間</td>
      <td>日期時間</td>
    </tr>
    <tr>
      <td>查詢（參考）</td>
      <td>字串</td>
    </tr>
    <tr>
      <td>Base64</td>
      <td>字串</td>
    </tr>
  </tbody>
</table>

>[!MORELIKETHIS]
>
>* [變更方案成員資料](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-member-data.md){target="_blank"}
>* [檢視程式成員網格上的資料](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/manage-and-view-members.md){target="_blank"}
>* [SFDC同步 — Campaign同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
