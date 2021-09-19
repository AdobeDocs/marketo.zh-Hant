---
description: 對話方塊 — Marketo檔案 — 產品檔案
title: 對話方塊
hide: true
hidefromtoc: true
source-git-commit: c46902686f1d5af63a51f5eaae2dc0e6afe99629
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 對話方塊 {#dialogues}

對話是您設定的特定聊天對話。 可依外觀、說的內容和看到者來自訂。

## 建立新對話方塊 {#create-a-new-dialogue}

1. 按一下&#x200B;**對話框**。

PICC

1. 按一下&#x200B;**新建**&#x200B;按鈕。

PICC

1. 輸入名稱（說明為可選），設定優先順序級別，然後按一下&#x200B;**Save**。

PICC

>[!NOTE]
>
>說明優先順序層級

## 對象條件 {#audience-criteria}

與Marketo智慧清單類似，受眾條件屬性可讓您定義目標受眾。

有數個屬性可供選擇。 在此示例中，我們選擇了Lead State _is_ California，而公司大小&#x200B;_大於_ 50。

1. 抓取「銷售機會狀態」屬性並將其拖曳至右側。

PICC

1. __ Isis預設設定。在「選擇值」欄位中，鍵入CA（您也可以按一下下拉式清單並從清單中選擇）。

PICC

1. 抓取「公司規模」屬性，並將其拖曳至右側。

PICC

1. 按一下運算子下拉式清單，然後選取「大於」。

PICC

1. 輸入50，然後按一下畫面上的其他位置以儲存。

PICC

## 新增群組 {#add-groups}

您也可以選擇將屬性分組，以備您想要擁有所有特定屬性以及其他屬性的「任何」時使用。

完成此操作

## 目標 {#target}

在此處輸入要顯示特定對話方塊的特定URL。

可接受的格式：

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>使用星號可當作全包王牌。 因此， `https://*.website.com`會將對話方塊放在網站的每個頁面上，包括子網域(例如：support.website.com)。 而`https://website.com/folder/*`會將對話方塊放在後續資料夾中的每個HTML頁面上(例如：在此案例中，假設資料夾為「sports」，因此：website.com/sports/baseball.html、website.com/sports/football.html等)。
