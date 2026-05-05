---
unique-page-id: 10100266
description: 追蹤企業特定人員動作的自訂活動概覽、其與自訂物件的差異，以及建立活動和API實作的兩個步驟設定。
title: 了解自訂活動
exl-id: 0bb74d9d-3a9d-4ef7-8c8c-2de36cd6190b
feature: Custom Activities
source-git-commit: 7fe6ed8b9fcb1aacf0e651a11ab90eaf0ae07937
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 3%

---

# 了解自訂活動 {#understanding-custom-activities}

透過自訂活動追蹤個人針對您的企業採取的行動。

## 什麼是活動 {#what-are-activities}

個人可與您的組織互動的方式有幾種。 他們可能會造訪您公司的網站、參加您的其中一個貿易展，或按一下傳送給他們的電子郵件中的連結。 這些動作即是活動，無論它們採取什麼動作，Marketo都會加以擷取，好讓您的行銷團隊更能瞭解如何即時傳送相關通訊給他們。

## 自訂活動 {#custom-activities}

自訂活動可協助您追蹤與Marketo表單、電子郵件或登入頁面無關的活動。 若要追蹤何時有人存有支票，請使用自訂活動。 若要追蹤某人何時參加網路研討會，請使用自訂活動。

>[!NOTE]
>
>自訂活動與自訂物件不同。 值可以變更時使用自訂物件（即「汽車顏色」從藍色變更為紅色）。 當追蹤已發生的時間及其詳細資料無法變更時（即「購買的汽車」），請使用自訂活動。

## 欄位 {#fields}

您可以新增要與活動建立關聯的[其他欄位](/help/marketo/product-docs/administration/marketo-custom-activities/add-edit-delete-marketo-custom-activity-fields.md)。 和主要欄位一樣，它們也可在智慧清單中作為篩選條件使用。

## 快速入門 {#getting-started}

自訂活動的運作方式與標準活動類似。 然而，設定這些變數需要兩個步驟。

步驟1：在您的Marketo帳戶中[建立自訂活動](/help/marketo/product-docs/administration/marketo-custom-activities/create-a-custom-activity.md)

步驟2：接下來，貴組織中使用Marketo API的員工就可以開始實作。 如需詳細資訊，請前往此處： [自訂活動API](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/addCustomActivityUsingPOST)
