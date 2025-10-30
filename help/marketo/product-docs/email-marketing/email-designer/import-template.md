---
solution: Marketo Engage
product: marketo
title: 範本匯入
description: 瞭解如何將您現有的電子郵件範本從傳統編輯器匯入新的電子郵件Designer。
level: Beginner, Intermediate
feature: Email Designer
badge: Beta
hide: true
hidefromtoc: true
source-git-commit: 316d5b59c7ea573f9246613ab3df2de86bdf4706
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 1%

---

# 範本匯入 {#template-import}

將您現有的電子郵件範本從傳統編輯器順暢地匯入新的電子郵件Designer，保留您的設計，並使用熟悉且可重複使用的結構加快範本建立。 檢閱[最佳實務](#best-practices)並瞭解[限制和補救措施](#limitations-and-remedies)。

1. 移至&#x200B;**設計工作室**。

   熒幕擷圖

1. 按一下&#x200B;**電子郵件範本**&#x200B;並選取&#x200B;**電子郵件範本（新增）**。

   熒幕擷圖

1. 按一下&#x200B;**建立範本**。

   熒幕擷圖

1. 輸入&#x200B;_名稱_&#x200B;和（選擇性） _描述_。

   熒幕擷圖

1. 按一下&#x200B;**Marketo範本**，然後選擇在傳統電子郵件編輯器中建立的現有範本。

   熒幕擷圖

   >[!NOTE]
   >
   >只能匯入已核准且已與目前工作區共用的範本和範本。

1. 選取所需的範本。

   熒幕擷圖

1. 按一下「使用此範本」。

   熒幕擷圖

1. 匯入的範本會在「電子郵件Designer」中開啟。

1. 檢閱元件以取得正確的轉換，並使用Designer進行任何需要的調整。 當您對範本感到滿意時，請核准它以用於電子郵件中。

## 建立內容片段 {#create-fragments}

建議您建立可重複區段的片段以供日後使用。

1. 按一下頂端的&#x200B;**...更多**&#x200B;按鈕，然後選取&#x200B;**另存為片段**。

   熒幕擷圖

1. 選取元件或結構，然後按一下[建立]。**&#x200B;**

   熒幕擷圖

1. 輸入名稱（和選用的說明），然後按一下&#x200B;**儲存**。

   熒幕擷圖

## 最佳做法 {#best-practices}

* 由於自由式HTML的差異可能很大，匯入工具可能不會總是完美地解譯每個元件。 請檢閱匯入的範本，以確保所有區段都可編輯且正確對應。 如果零件無法選取，則只要重新建立該區段以獲得最佳結果即可。

* 匯入後，您可以將可重複使用的區段儲存為片段，並核准電子郵件作者使用。 套用品牌主題以維持一致性和法規遵循。

* 您可以繼續使用Velocity指令碼，並考慮使用片段和條件式內容的組合重新實作較舊的程式碼片段，以提升彈性和控制能力。

## 限制與補救措施 {#limitations-and-remedies}

<table><thead>
  <tr>
    <th>限制</th>
    <th>原因</th>
    <th>補救措施</th>
  </tr></thead>
<tbody>
  <tr>
    <td>在傳統電子郵件編輯器中定義的變數，無法在電子郵件層級使用。</td>
    <td>當編輯器尚未提供WYSIWYG功能時，變數原本旨在簡化電子郵件編輯。 在電子郵件Designer中，使用者可以透過可用控制項獲得類似的彈性。 匯入工具會維護現有範本的結構和元件，協助您在電子郵件Designer中有效率地重建範本。</td>
    <td>使用者應該能夠在Designer中達成此目的。 <p>
    針對模組，您可以將不同的區段儲存為片段。 核准的片段將可用於電子郵件層級。</td>
  </tr>
  <tr>
    <td>如果來源HTML包含巢狀區塊，則較深的圖層無法在Designer中定址。</td>
    <td>電子郵件Designer不支援巢狀註釋。</td>
    <td>即使Designer不允許編輯巢狀結構，也應準確呈現。 請務必先測試範本。<p>
    使用「格點」重新建立結構。</td>
  </tr>
  <tr>
    <td>有時按鈕會匯入為包含文字的簡單容器。</td>
    <td>在匯入期間，可能會誤解某些使用HTML的實作樣式。</td>
    <td>在Designer中重新建立按鈕。</td>
  </tr>
  <tr>
    <td>按鈕有時可能過大。</td>
    <td>Marketo電子郵件的CSS與其他較低層級元素(<code>&lt;span&gt;</code>)之間發生衝突</td>
    <td>嘗試在Designer中調整按鈕的邊界和邊框間距。</td>
  </tr>
  <tr>
    <td>專案符號本身不受支援。</td>
    <td>電子郵件Designer目前不提供專案符號。</td>
    <td>考慮使用替代技術重新實作專案符號。</td>
  </tr>
  <tr>
    <td>容器的內容與值屬性值不相符時，垂直對齊會扭曲。</td>
    <td><code>valign</code> 不會在範本中定義的容器內運作。</td>
    <td>嘗試在「電子郵件Designer」中調整按鈕的邊界和邊框間距。</td>
  </tr>
  <tr>
    <td>範本層級的程式層級Personalization Token (My Token)可能會發生驗證錯誤。</td>
    <td>電子郵件範本不支援方案層級權杖。</td>
    <td>將它們替換為範本內的其他代號型別，並在個別電子郵件內替換為我的Token 。</td>
  </tr>
  <tr>
    <td>可能無法選取分隔線元件。</td>
    <td>此發行版本未涵蓋分隔線元件。</td>
    <td>不適用</td>
  </tr>
  <tr>
    <td>如果原始HTML有任何格式錯誤的結構，則這些結構可能會移轉過來。</td>
    <td>原始HTML發生問題。</td>
    <td>匯入前需要修正問題。</td>
  </tr>
  <tr>
    <td>對於匯入的內容，使用內容預覽不是可靠的指標。</td>
    <td>Designer的預覽功能不支援自訂HTML。</td>
    <td>建議您使用<b>模擬內容</b>畫面中的<i>傳送校樣</i>選項來測試電子郵件。</td>
  </tr>
  <tr>
    <td>舊範本中的程式碼片段無法用於電子郵件Designer。</td>
    <td>電子郵件Designer不支援代碼片段。</td>
    <td>將您的程式碼片段重新實作為片段搭配條件式內容。</td>
  </tr>
</tbody></table>
