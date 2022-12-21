---
unique-page-id: 11382829
description: Marketo Outlook外掛程式由IT解除安裝 — Marketo檔案 — 產品檔案
title: Marketo Outlook外掛程式由IT卸載
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---

# Marketo Outlook外掛程式由IT卸載 {#marketo-outlook-plugin-uninstall-by-it}

以下說明IT如何遠程卸載Marketo Outlook Plugin。

以「System」或具有/x開關的管理用戶帳戶的形式運行以下命令行以卸載。

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

要進行故障排除，您可以啟用記錄以建立輸出日誌檔案。

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

要指定日誌檔案的位置，可以在命令行中指定檔案路徑。

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>遠程卸載插件將強制關閉用戶電腦上的Outlook。

請參閱 [Microsoft交換機的完整清單](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) 如果您想要嘗試不同的記錄層級或使用者介面層級。
