---
description: 對話方塊 — Marketo檔案 — 產品檔案
title: 對話方塊
hide: true
hidefromtoc: true
source-git-commit: d5c1c1d0ce2a521898eaa4f6610bf1ce04b4f66b
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# 對話方塊 {#dialogues}

對話是您將設定的個別聊天對話。 了解如何以視覺化方式自訂頁面、決定其上顯示的頁面，以及決定說明的內容以及看見者。

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

與Marketo智慧清單類似，受眾條件屬性可讓您定義目標受眾。 您可以使用推斷、銷售機會或公司屬性（或其組合）來鎖定已知或未知的銷售機會。

有許多&#x200B;_屬性組合可供選擇。_&#x200B;在此範例中，我們鎖定在加州，在有超過50名員工的公司工作的所有已知銷售機會。

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

如何捕獲ANON線索

注意 — 可能提到推斷的工作/顯示方式和使用案例，銷售機會電子郵件為空白

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
>使用星號可當作全包王牌。 因此， `https://*.website.com`會將對話方塊放在網站的每個頁面上，包括子網域(例如：`support.website.com`)。 而`https://website.com/folder/*`會將對話方塊放在後續資料夾中的每個HTML頁面上(例如：在此案例中，假設資料夾為「sports」，因此：website.com/sports/baseball.html、website.com/sports/football.html等)。

## 串流設計工具 {#stream-designer}

流設計器包含可添加的不同資訊卡，以形成聊天對話。

<table>
 <tr>
  <td><strong>訊息</strong></td>
  <td>當您想要做陳述而不需要回應時使用(例如：「嗨！ 使用代碼SAVE25」時，所有項目今天可節省25%。
</td>
 </tr>
 <tr>
  <td><strong>問題</strong></td>
  <td>當您想要詢問多選題時使用，您會提供可用的回應(例如：你對哪種車感興趣？ 回應= SUV、小型車、卡車等)。</td>
 </tr>
 <tr>
  <td><strong>資訊捕獲</strong></td>
  <td>收集資訊時使用。 要選擇的三個欄位是「電子郵件地址」、「電話號碼」和「文字」（這可讓訪客自行撰寫訊息）。</td>
 </tr>
 <tr>
  <td><strong>約會排程器</strong></td>
  <td>為訪客提供可用日期的日曆，以排程後續作業。 日曆可用性反映[下一個代理程式行](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing)。</td>
 </tr>
 <tr>
  <td><strong>目標</strong></td>
  <td>這是訪客唯一看不到的卡片。 您可以決定在哪個時間點在特定聊天內達成目標(例如：如果收集訪客的電子郵件是您的目標，請將「目標」卡放在資料流中的「資訊擷取」之後)。</td>
 </tr>
</table>

可能的專屬區段

顯示下面的示例