---
unique-page-id: 2949711
description: 使用註冊代碼為 [!DNL Outlook] 安裝Marketo電子郵件增益集 — Marketo檔案 — 產品檔案
title: 使用註冊代碼為 [!DNL Outlook] 安裝Marketo電子郵件增益集
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 4%

---

# 使用註冊代碼為[!DNL Outlook]安裝Marketo電子郵件增益集 {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

如果使用者可以存取其筆記型電腦上的管理員設定，您可以直接將註冊代碼傳送給他們。

如果您尚未收到邀請電子郵件，請洽詢Marketo管理員以邀請您。

>[!PREREQUISITES]
>
>您必須是[已核發Marketo電子郵件增益集授權](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md)。

>[!IMPORTANT]
>
>在Windows使用者資料夾包含非英文字元的電腦上不支援安裝。 此資料夾是由Windows根據Windows使用者名稱在`<System Root>\Users\`下自動產生，如果Windows使用者名稱是非英文名稱，則可能包含非英文字元。 請與您的IT團隊合作，確認您是否遇到安裝問題。

>[!NOTE]
>
>Sales Insight的Gmail和Outlook電子郵件外掛程式中不提供「銷售Insight動作」功能，包括「傳送銷售電子郵件」、「新增至銷售促銷活動」和「工作」。 目前，使用者只有在使用銷售Marketo電子郵件外掛程式時，才能從電子郵件使用者端傳送包含或不包含Insight電子郵件範本的可追蹤電子郵件。

## 下載安裝程式 {#download-installer}

1. 識別您的[Microsoft Outlook版本](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}。

1. 在下表中，按一下連結，即可下載適用於您Microsoft Outlook版本的適當.ZIP檔案。

1. 解壓縮檔案以存取必要的.MSI檔案，然後繼續安裝。

   >[!NOTE]
   >
   >目前，下列連結僅在[!DNL Microsoft Edge]中運作，或在[!DNL Chrome]中按一下滑鼠右鍵。 造成任何不便，敬請見諒。

<table><thead>
  <tr>
    <th>Outlook版本</th>
    <th>32位元Outlook</th>
    <th>64位元Outlook</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Outlook 2000</td>
    <td>不支援</td>
    <td>不適用</td>
  </tr>
  <tr>
    <td>Outlook 2003</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下載</a></td>
    <td>不適用</td>
  </tr>
  <tr>
    <td>Outlook 2007</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下載</a></td>
    <td>不適用</td>
  </tr>
  <tr>
    <td>Outlook 2010</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下載</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">下載</a></td>
  </tr>
  <tr>
    <td>Outlook 2013</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下載</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">下載</a></td>
  </tr>
  <tr>
    <td>Outlook 2016</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下載</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">下載</a></td>
  </tr>
  <tr>
    <td>Outlook 2019</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下載</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">下載</a></td>
  </tr>
  <tr>
    <td>適用於Mac的Outlook</td>
    <td>不支援</td>
    <td>不支援</td>
  </tr>
  <tr>
    <td>Outlook Web App</td>
    <td>不支援</td>
    <td>不支援</td>
  </tr>
  <tr>
    <td>Office 365*</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下載</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">下載</a></td>
  </tr>
</tbody></table>

*[!DNL Office] 365版本：僅[!DNL Windows]使用者端（[!DNL Windows] 10、[!DNL Enterprise]或[!DNL Pro]）。

>[!IMPORTANT]
>
>Microsoft已發行適用於Windows [的](https://techcommunity.microsoft.com/t5/outlook-blog/new-outlook-for-windows-now-available/ba-p/3932068){target="_blank"}新版Outlook。 這個新版本不支援現有的MSI Outlook外掛程式。 MSI Outlook外掛程式將繼續在執行Classic版Outlook的Windows案頭上運作。 若要進一步瞭解適用於組織的新版Windows Outlook，[請按一下這裡](https://techcommunity.microsoft.com/t5/outlook-blog/the-new-outlook-for-windows-for-organization-admins/ba-p/3929169){target="_blank"}。

## 複製您的註冊代碼 {#copy-your-registration-code}

1. 從您收到的邀請電子郵件複製註冊代碼。

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. 關閉[!DNL Microsoft Outlook]。

   ![](assets/ent-key-close-outlook-hand.png)

## 安裝 {#install}

1. 執行安裝程式。

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >如果您收到安全性警告，請不要擔心！ 只需按一下&#x200B;**執行**。

1. 按一下「**[!UICONTROL Next]**」。

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. 填入&#x200B;**[!UICONTROL First Name]**、**[!UICONTROL Last Name]**、**[!UICONTROL Email Address]**，然後複製電子郵件中的&#x200B;**[!UICONTROL Registration code]**&#x200B;並貼入表單，然後按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >如果安裝失敗，請洽詢您的IT部門，以確保不會封鎖HTTPS流量。 安裝程式需要開啟HTTPS流量。

1. 按一下&#x200B;**[!UICONTROL Next]**&#x200B;以安裝在預設位置。

   ![](assets/select-installation-folder-hand.png)

1. 按一下「**[!UICONTROL Next]**」。

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >如果您收到有關未知發行者的安全性提示，請按一下&#x200B;**[!UICONTROL Yes]**。

1. 安裝現已完成，請按一下&#x200B;**[!UICONTROL Close]**。

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. 現在開啟[!DNL Microsoft Outlook]並檢視Marketo按鈕。

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   太好了！ 現在Marketo按鈕的位置更好了。

進一步瞭解如何使用Marketo訊息並記錄與Marketo動作。

>[!MORELIKETHIS]
>
>* [使用Outlook的Marketo電子郵件增益集傳送及追蹤電子郵件](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [使用Marketo範本從Outlook傳送及追蹤](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
