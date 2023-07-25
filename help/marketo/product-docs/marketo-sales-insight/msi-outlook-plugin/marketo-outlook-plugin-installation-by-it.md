---
unique-page-id: 11382815
description: Marketo Outlook外掛程式由IT安裝 — Marketo檔案 — 產品檔案
title: 由IT人員安裝Marketo Outlook外掛程式
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# 由IT人員安裝Marketo Outlook外掛程式 {#marketo-outlook-plugin-installation-by-it}

有時公司政策會要求其IT團隊在員工的電腦上安裝所有軟體。 在這些情況下，IT通常會使用自己的部署軟體從遠端執行這項作業。 本檔案提供您在部署程式期間用來作為遠端安裝Outlook外掛程式的輸入的命令列。

>[!PREREQUISITES]
>
>[設定](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) 企業金鑰。

以&#39;System&#39;或Administrative user account with /i switch to install的身分執行以下命令列。

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

若要進行疑難排解，您可以啟用記錄以建立輸出記錄檔。

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

若要指定記錄檔的位置，您可以在命令列中指定檔案路徑。

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>記錄檔的儲存位置必須存在，否則安裝將會中止。

請參閱 [Microsoft的完整交換器清單](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) 如果您想要嘗試不同的記錄層級或使用者介面層級。

>[!MORELIKETHIS]
>
>[Marketo Outlook外掛程式由IT解除安裝](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
