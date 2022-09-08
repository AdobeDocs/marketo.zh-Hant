---
unique-page-id: 2949711
description: 使用註冊代碼安裝Marketo Email Add-in for Outlook - Marketo Docs — 產品檔案
title: 使用註冊代碼安裝Outlook的Marketo Email Add-in
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
source-git-commit: 268a7f1ca441661e1d943a8d6abce7bdcf308a98
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 使用註冊代碼安裝Outlook的Marketo Email Add-in {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

如果用戶可以訪問其筆記型電腦上的管理設定，您可以直接向他們發送註冊代碼。

如果您未收到邀請電子郵件，請洽詢您的Marketo管理員以邀請您。

>[!PREREQUISITES]
>
>你必須 [核發Marketo電子郵件增益集授權](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>Windows用戶資料夾包含非英文字元的PC上不支援安裝。 此資料夾由Windows在 `<System Root>\Users\` 根據Windows用戶名，如果Windows用戶名為非英文名稱，則可能包含非英文字元。 請與IT團隊合作，確認您是否遇到安裝問題。

>[!NOTE]
>
>10/1/20上，最新版Outlook外掛程式已停止支援離線模式。

## 下載安裝程式 {#download-installer}

1. 識別 [Microsoft Outlook版本](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c)

1. 按一下連結以下載適合您版本Microsoft Outlook的安裝程式。

   >[!NOTE]
   >
   >目前，下列連結只能在Microsoft Edge中運作，或在Chrome中以滑鼠右鍵按一下。 給您帶來不便。

   | Outlook版本 | 32位Outlook | 64位Outlook |
   |---|---|---|
   | 2000年展望 | 不支援 | 不適用 |
   | 2003年展望 | [下載](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | 不適用 |
   | 2007年展望 | [下載](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | 不適用 |
   | 2010年展望 | [下載](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [下載](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | 2013年展望 | [下載](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [下載](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | 2016年展望 | [下載](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [下載](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | 2019年展望 | [下載](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [下載](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Mac展望 | 不支援 | 不支援 |
   | Outlook Web App | 不支援 | 不支援 |
   | Office 365* | [下載](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [下載](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |

   *Office 365版本：僅限Windows用戶端（在Windows 10、Enterprise或Pro上）。

## 複製您的註冊代碼 {#copy-your-registration-code}

1. 從您收到的邀請電子郵件複製註冊代碼。

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. 關閉Microsoft Outlook。

   ![](assets/ent-key-close-outlook-hand.png)

## 安裝 {#install}

1. 運行安裝程式。

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >如果你收到安全警告，別擔心！ 按一下 **執行**.

1. 按一下 **下一個**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. 填寫 **名字**, **姓氏**, **電子郵件地址**，然後複製並貼上 **註冊代碼** 從電子郵件移入表單，然後按一下 **下一個**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >如果安裝失敗，請洽詢您的IT部門，確保HTTPS流量不會遭到封鎖。 安裝程式需要開啟HTTPS流量。

1. 按一下 **下一個** 以在預設位置安裝。

   ![](assets/select-installation-folder-hand.png)

1. 按一下 **下一個**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >如果您收到有關未知發佈者的安全提示，請按一下 **是**.

1. 安裝現在已完成，請按一下 **關閉**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. 現在，開啟Microsoft Outlook並查看Marketo按鈕。

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   太棒了！ 現在Marketo的按鈕更好了。

進一步了解如何使用Marketo訊息及記錄搭配Marketo動作。

>[!MORELIKETHIS]
>
>* [使用Outlook的Marketo電子郵件增益集傳送及追蹤電子郵件](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md)
>* [使用Marketo範本從Outlook傳送及追蹤](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md)

