---
unique-page-id: 27656223
description: 安裝Professional Edition客戶的 [!DNL Salesforce] 自訂 — Marketo檔案 — 產品檔案
title: 安裝Professional Edition客戶的 [!DNL Salesforce] 自訂
exl-id: dc004a28-b580-4449-9fde-e744681ac53a
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# 安裝Professional Edition客戶的[!DNL Salesforce]自訂 {#install-salesforce-customization-for-professional-edition-customers}

擁有[!DNL Salesforce] Professional Edition的客戶必須依照下列步驟安裝自訂。

>[!PREREQUISITES]
>
>* [!DNL Sales Connect]管理員需要連線其[!DNL Salesforce]和[!DNL Sales Connect]帳戶。
>* [!DNL Salesforce]個使用的執行個體需要空間來安裝13個自訂活動欄位。

## 安裝 {#installation}

1. 在[!DNL Sales Connect]中，按一下右上方的齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/one-4.png)

1. 在[!UICONTROL Admin Settings]底下，按一下&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/two-4.png)

1. 確認您已連線至您的[!DNL Salesforce]帳戶。

   >[!CAUTION]
   >
   >如果您已連線，則會看到綠色的&quot;[!UICONTROL Install]&quot;按鈕。 **不要**&#x200B;按一下此按鈕，請改為繼續執行步驟4。

1. 登入您連線的[!DNL Salesforce]帳戶，然後按一下[此連結](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0b000001oWEZ)。
1. 您將會被送到[!DNL Sales Connect]安裝頁面。

   ![](assets/install-package.png)

1. 選擇您要安裝自訂的使用者：僅限管理員、所有使用者或特定設定檔。
1. 按一下&#x200B;**[!UICONTROL Install]**&#x200B;按鈕以安裝自訂。
1. 若要確認安裝成功，請登入您的[!DNL Salesforce]帳戶。
1. 按一下&#x200B;**[!UICONTROL Setup]**，在搜尋列中搜尋「已安裝的封裝」，然後按一下&#x200B;**[!UICONTROL Installed Packages]**。

   您會在該處看到Marketo Sales Connect自訂。

   若要在[!DNL Sales Connect]執行個體中設定[!DNL Salesforce]，請依照《安裝指南》第7頁的「設定SALES ENGAGE SALESFORCE套件」一節中所述的步驟操作。

   >[!NOTE]
   >
   >[!DNL Sales Engage]是[!DNL Sales Connect]的先前名稱。

## 指南 {#guides}

[Salesforce Classic安裝指南](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

[Salesforce Lightning安裝指南](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
