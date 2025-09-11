---
unique-page-id: 11377395
description: 新增其他品牌領域 — Marketo檔案 — 產品檔案
title: 新增其他品牌化網域
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: de2f73f932fd38211dba96d8697ef4bb4fd0f0da
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 3%

---

# 新增其他品牌化網域 {#add-an-additional-branding-domain}

當您從單一Marketo執行個體執行多個品牌，並希望每個品牌都有自己的品牌追蹤連結時，請新增一個品牌網域。

>[!PREREQUISITES]
>
>在新增其他品牌網域之前，您必須[以品牌網域取代一般追蹤連結](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/add-an-additional-branding-domain-1.png)

1. 按一下「**[!UICONTROL Email]**」。

   ![](assets/add-an-additional-branding-domain-2.png)

1. 按一下&#x200B;**[!UICONTROL Add]**&#x200B;以新增其他品牌化網域。

   ![](assets/add-an-additional-branding-domain-3.png){width="600"}

1. 輸入您新品牌化網域的名稱，選取&#x200B;_建立主要網域_&#x200B;和/或&#x200B;_產生SSL憑證_ （兩者皆為選用），然後按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _設為主要網域_：設為主要網域，並將所有現有未傳送電子郵件設為[預設]，所有新建立的電子郵件將預設為主要網域。 您可以[以每封電子郵件為基礎](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}覆寫此專案。
>
>* _產生SSL憑證_：您可以使用建立網域來建立安全通訊端層(SSL)。 第一個追蹤網域將啟動可能需要幾個小時的一次性基礎結構設定。 完成後，您將會收到通知，然後您可以設定第一個網域。 若要將SSL新增至您現有的網域，請聯絡[Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。

## 編輯現有網域的SSL

請依照下列步驟，為您現有的網域啟用SSL。

1. 從&#x200B;_[!UICONTROL Admin]_&#x200B;區域，選取&#x200B;**[!UICONTROL Email]**。

1. 在&#x200B;_[!UICONTROL Domain]_&#x200B;索引標籤上，選取網域列並按一下&#x200B;**[!UICONTROL Add SSL]**。

   ![管理員 — 電子郵件 — 網域 — 新增SSL](./assets/admin-email-branding-domain-add-ssl.png){width="600"}

1. 在對話方塊中，按一下&#x200B;**[!UICONTROL Confirm]**。

   ![新增SSL — 確認](./assets/generate-ssl-cert-confirm.png){width="400"}

## 錯誤訊息 {#error-messages}

<table><thead>
  <tr>
    <th>錯誤</th>
    <th>詳細資料</th>
  </tr></thead>
<tbody>
<tr>
    <td><i>網域已經存在。</i></td>
    <td>已有相同名稱的網域存在。</td>
  </tr>
  <tr>
    <td><i>網域未對應到預設網域。</i></td>
    <td>自訂網域未正確對應到預設網域。 請驗證網域對應設定，並確定DNS設定指向正確的預設網域。</td>
  </tr>
  <tr>
    <td><i>因為不支援的CAA記錄，所以無法發行SSL憑證。 請要求您的IT更新您的CAA記錄。</i></td>
    <td>CAA記錄不是最新的。 若是使用Marketo Engage管理的SSL憑證，CAA記錄需要更新為供應商建議的憑證。 請聯絡您的IT部門以更新CAA記錄。 如需其他詳細資訊，請參閱<a href="https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305#M2246">此頁面</a>。</td>
  </tr>
  <tr>
    <td><i>SSL憑證已發行。</i></td>
    <td>此自訂網域已存在SSL憑證。 除非憑證已過期或需要重新核發，否則不需要進一步動作。</td>
  </tr>
  <tr>
    <td><i>找不到預設網域。 請聯絡支援以尋求協助。</i></td>
    <td>嘗試尋找預設網域時發生問題。 請洽詢支援人員，以便他們進行調查。</td>
  </tr>
  <tr>
    <td><i>建立網域時遇到未預期的錯誤。 請聯絡支援以尋求協助。</i></td>
    <td>發生非預期的錯誤。 請收集記錄檔和錯誤詳細資料，並將問題升級至<a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo支援</a>。</td>
  </tr>
</tbody></table>

## 注意事項 {#things-to-note}

* **網域與Marketo Engage的DNS對應**：在UI中新增網域之前，您必須[將CNAME對應到Marketo提供的網域](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}。

* **自訂SSL**：如果您需要自訂SSL，請提交[支援票證](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。 請勿使用自助核取方塊來建立SSL。

* **預先存在的SSL**：新增網域時，系統會檢查預先存在的SSL （可能之前已手動建立）。 如果您遇到此驗證，請在不選取SSL建立的情況下建立您的網域，我們會為您連線。 [連絡支援人員](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}更多詳細資料/選項。

* **刪除網域**：自動刪除網域&#x200B;**不會**&#x200B;刪除SSL憑證。 此護欄可防止使用者發生導致網站沒有SSL憑證的錯誤。 如果您確實要移除SSL憑證，[請連絡支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。

>[!MORELIKETHIS]
>
>[編輯您的預設品牌化網域](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
