---
unique-page-id: 2359675
description: 瞭解如何在Marketo中停用表單欄位的預填。 停止已知訪客資料自動填寫欄位。
title: 停用表單欄位預先填入
exl-id: c600e0ce-1b94-4f7b-b75d-f550a2904799
feature: Forms
TQID: https://experienceleague.adobe.com/loH0b6d25kDL0dReI7lU62IFyXGr3p8tygqwTPx-OVk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 180
ht-degree: 10%

---

# 停用表單欄位預先填入 {#disable-pre-fill-for-a-form-field}

當網路訪客是已知的（已編碼），Marketo表單預設會使用欄位資訊預先填寫欄位。 如果您想要關閉此功能，請參閱以下操作說明。

>[!NOTE]
>
>預設會啟用&#x200B;**表單預填**。 登陸頁面層級預填設定和管理員層級預填設定優先於表單層級設定：
>
>表單>登陸頁面>管理員

## 如何停用預填 {#how-to-disable-pre-fill}

1. 前往 **[!UICONTROL Marketing Activities]**。

   ![](assets/login-marketing-activities-7.png)

1. 選取您的表單並按一下&#x200B;**[!UICONTROL Edit Form]**。

   ![](assets/image2014-9-15-14-3a26-3a46.png)

   >[!CAUTION]
   >
   >將表單內嵌在您自己的頁面上時，表單預填無法運作。 它只適用於Marketo登陸頁面。

1. 選取其中一個欄位並將&#x200B;**[!UICONTROL Form Pre-fill]**&#x200B;設為&#x200B;**[!UICONTROL Disabled]**。

   ![](assets/image2014-9-15-14-3a26-3a54.png)

   >[!TIP]
   >
   >您也可以停用登入頁面層級或管理員層級的表單預填。

1. 按一下「**[!UICONTROL Finish]**」。

   ![](assets/image2014-9-15-14-3a27-3a1.png)

1. 按一下「**[!UICONTROL Approve and Close]**」。

   ![](assets/image2014-9-15-14-3a27-3a6.png)

## 敏感欄位 {#sensitive-fields}

當您[將欄位標示為敏感欄位](/help/marketo/product-docs/administration/field-management/mark-a-field-as-sensitive.md)，以防止其值預先填入表單時，您會在預先填入選項中看到此選項。

![](assets/disable-pre-fill.png)
