---
description: 推送克隆 — Marketo文檔 — 產品文檔
title: 推送克隆
hide: true
hidefromtoc: true
source-git-commit: 8920bc525075923b32e7330da20debb7b8f47b06
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 推送克隆 {#push-clone}

此功能允許您以靜態清單的形式將位於Adobe Experience Platform的段推送到Marketo。

>[!PREREQUISITES]
>
>* [建立API用戶](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) 在Marketo。
>* 然後，轉到 **管理** > **朗奇波因特**。 查找您剛建立的角色的名稱，然後按一下 **查看詳細資訊**。 複製並保存資訊 **客戶端ID** 和 **客戶端密碼**，因為您需要它。


1. 登錄到 [Adobe Experience Platform](https://experience.adobe.com/)。

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. 按一下網格表徵圖並選擇 **Experience Platform**。

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. 在左導航中，按一下 **目標**。

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. 按一下 **目錄**。

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. 查找Marketo Engage磁貼，然後按一下 **激活段**。

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. 按一下 **配置新目標**。

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. 在「帳戶類型」下，選擇「現有帳戶」或「新建帳戶」單選按鈕(在本例中，我們選擇 **現有帳戶**)。 按一下「選擇帳戶」表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

1. 選擇目標帳戶並按一下 **選擇**。

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

接下來，你必須選擇是僅匹配現有的Marketo人，還是匹配現有的Marketo人，並在Marketo創造失蹤的人。 下面是概述如何執行每個操作的部分。

## 匹配Marketo現有人創造Marketo失蹤人口 {#match-existing-marketo-people-create-missing-people}

執行上面步驟1-8後……

1. 輸入目標 **名稱** 和可選說明。 按一下「人員建立」(Person Creation)下拉框並選擇 **匹配Marketo現有人創造Marketo失蹤人口**。

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

1. 此部分是可選的。 按一下 **建立** 跳過。

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. 選擇您建立的目標，然後按一下 **下一個**。

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. 選擇要發送到Marketo的段，然後按一下 **下一個**。

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

1. 按一下 **添加新映射**。

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. 按一下映射表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. 通過選擇映射名 **名字** 按一下 **選擇**。

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

1. 通過按一下 **添加新映射** 重複步驟7兩次，選擇lastName，然後選擇companyName。

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. 現在是繪製電子郵件地址的時候了。 按一下 **添加新映射** 的雙曲餘切值。

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. 按一下映射表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. 按一下「選擇標識名稱空間」單選按鈕，選擇  **電子郵件**，然後按一下 **選擇**。

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

1. 現在是時候選擇源欄位了。 對於電子郵件，按一下游標表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. 按一下「選擇標識名稱空間」單選按鈕，查找並選擇 **電子郵件**，然後按一下 **選擇**。

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

莫里

## 僅匹配現有Marketo人 {#match-existing-marketo-people-only}

>[!NOTE]
>
>身份被用來在Marketo尋找火柴。 如果找到匹配項，則會將該人員添加到靜態清單中。 如果找不到匹配項，則會刪除這些人(即，不在Marketo建立)。

1. _在Marketo_、建立靜態清單，或查找並選擇已建立的清單。 從URL的末尾複製映射ID。

PICC

>[!NOTE]
>
>要獲得最佳結果，請確保您在Marketo引用的清單為空。

1. 回到Adobe Experience Platform，輸入您剛複製的ID。 選擇您的開始日期。 人員將連續同步，直到選定的結束日期。 對於不確定的同步，將結束日期留空。 按一下 **下一個** 完成。

PICC

1. 確認更改並按一下 **完成**。

PICC
