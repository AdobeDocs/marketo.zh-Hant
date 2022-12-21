---
unique-page-id: 27656223
description: 為Professional Edition客戶安裝Salesforce自訂 — Marketo檔案 — 產品檔案
title: 為專業版客戶安裝Salesforce定制
exl-id: dc004a28-b580-4449-9fde-e744681ac53a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 為專業版客戶安裝Salesforce定制 {#install-salesforce-customization-for-professional-edition-customers}

使用Salesforce Professional Edition的客戶必須遵循這些步驟來安裝自定義。

>[!PREREQUISITES]
>
>* Sales Connect管理員需要連接其Salesforce和Sales Connect帳戶。
>* 使用的Salesforce執行個體需要有空間來安裝十三個自訂活動欄位。


## 安裝 {#installation}

1. 在Sales Connect中，按一下右上角的齒輪表徵圖並選擇 **設定**.

   ![](assets/one-4.png)

1. 在「管理設定」下，按一下 **Salesforce**.

   ![](assets/two-4.png)

1. 確認您已連接到Salesforce帳戶。

   >[!CAUTION]
   >
   >如果已連接，您會看到綠色的「安裝」按鈕。 **不要** 按一下此按鈕，繼續執行步驟4。

1. 登入您所連線的Salesforce帳戶，然後按一下 [此連結](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0b000001oWEZ).
1. 您將被發送到Sales Connect安裝頁。

   ![](assets/install-package.png)

1. 選擇要為以下項目安裝自定義項的用戶：僅限管理員、所有使用者或特定設定檔。
1. 按一下 **安裝** 按鈕以安裝自定義。
1. 若要確認安裝是否成功，請登入您的Salesforce帳戶。
1. 按一下 **設定**，在搜索欄中搜索「已安裝的包」，然後按一下 **已安裝的軟體包**.

   您將在此處看到Marketo Sales Connect自定義。

   要在Salesforce實例中配置Sales Connect，請按照《安裝指南》第7頁「配置SALES ENGAGE SALESFORCE包」部分開始的步驟操作。

   >[!NOTE]
   >
   >Sales Engage是Sales Connect的前一個名稱。

## 指南 {#guides}

[Salesforce Classic安裝指南](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

[Salesforce Lightning的安裝指南](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
