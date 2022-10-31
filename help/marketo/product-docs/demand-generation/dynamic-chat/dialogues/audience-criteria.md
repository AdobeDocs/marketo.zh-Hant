---
description: 對象條件 — Marketo檔案 — 產品檔案
title: 對象條件
exl-id: 9b70b03e-229e-469e-bd65-07aaf2dcbec6
source-git-commit: f71ac0398b3a93d2c46201a696dd41e6ccd89000
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 1%

---

# 對象條件 {#audience-criteria}

與Marketo智慧清單類似，受眾條件屬性可讓您定義目標受眾。 您可以使用推斷、人員或公司屬性（或其組合）來鎖定已知或未知的人。

## 優先順序 {#priority}

優先順序決定銷售機會在有資格獲得多個對話時會收到哪個對話。 這是你第一次 [建立對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}。 您可以開啟現有對話方塊，然後前往 **對話框詳細資訊** 在「對象條件」標籤中。

![](assets/audience-criteria-1.png)

## 事件 {#events}

![](assets/audience-criteria-2.png)

事件可讓您根據訪客捲動的次數或在您的頁面/網站上停留的時間來鎖定訪客。 在以下範例中，我們將目標定位於某個特定頁面上超過20秒的訪客。

1. 抓住 **頁面逗留時間** 事件並拖曳至右側。

   ![](assets/audience-criteria-3.png)

1. 將「大於」時間設為20秒。

   ![](assets/audience-criteria-4.png)

1. 在中新增所需頁面的URL [目標](#target) 區段。

   ![](assets/audience-criteria-5.png)

## 屬性 {#attributes}

![](assets/audience-criteria-6.png)

**已知人員**

有 _many_ 要選擇的屬性組合。 在以下範例中，我們鎖定所有 **已知人** 在有50多名員工的公司工作。

1. 抓住 **人員狀態** 屬性並拖曳至右側。

   ![](assets/audience-criteria-7.png)

1. _是_ 預設為。 在「選擇值」欄位中，鍵入CA（您也可以按一下下拉式清單並從清單中選擇）。

   ![](assets/audience-criteria-8.png)

1. 抓住 **公司規模** 屬性，並拖曳到顯示的位置 _拖放屬性至此_.

   ![](assets/audience-criteria-9.png)

   >[!NOTE]
   >
   >您也可以按一下屬性，以選擇屬性 **+** 表徵圖。

1. 按一下運算子下拉式清單，然後選取 **大於**.

   ![](assets/audience-criteria-10.png)

1. 輸入50，然後按一下畫面上的其他位置以儲存。

   ![](assets/audience-criteria-11.png)

就這樣！

**匿名人員**

有一種簡單的方法可以專門定位尚未在資料庫中的人員。 在此範例中，我們會鎖定所有 **匿名人員** 位於紐約地區。

1. 抓住 **人員電子郵件** 屬性並拖曳至右側。

   ![](assets/audience-criteria-12.png)

1. 按一下運算子下拉式清單，然後選取 **空白**.

   ![](assets/audience-criteria-13.png)

1. 抓住 **推斷狀態** 屬性，並拖曳到顯示的位置 _拖放屬性至此_.

   ![](assets/audience-criteria-14.png)

   >[!NOTE]
   >
   >當有人瀏覽您的網站時， [蒙奇金](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) 將它們加入系統。 我們在一個特殊的資料庫中查找他們的IP，並推斷出各種好的資訊。

1. _是_ 預設為。 在「選取值」欄位中，輸入NY（您也可以按一下下拉式清單，然後從清單中選取）。

   ![](assets/audience-criteria-15.png)

## 新增群組 {#add-groups}

您也可以選擇將屬性分組，以備您想擁有所有特定屬性以及其他屬性的「全部或任何」時使用。 您可以新增多個群組。

![](assets/audience-criteria-16.png)

![](assets/audience-criteria-17.png)

## 目標 {#target}

在此處輸入要顯示特定對話方塊的URL。 您也可以選擇新增排除項目。

可接受的格式：

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>使用星號可當作全包王牌。 So `https://*.website.com` 會將對話方塊放在網站的每個頁面上，包括子網域(例如： `support.website.com`)。 和 `https://website.com/folder/*` 會將對話方塊放在後續資料夾的每個HTML頁面上(例如：在此案例中，假設資料夾為「sports」，因此：website.com/sports/baseball.html、website.com/sports/football.html等)。

**排除**

使用排除項目來確保對話方塊可執行 **not** 顯示在您網站的特定頁面/區域上。 排除會遵循與包含相同的格式。

![](assets/audience-criteria-18.png)

>[!MORELIKETHIS]
>
>* [建立對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [串流設計工具](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md){target=&quot;_blank&quot;}
>* [報表](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}

