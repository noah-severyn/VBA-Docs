---
title: Workbook.AfterXmlExport event (Excel)
keywords: vbaxl10.chm503100
f1_keywords:
- vbaxl10.chm503100
api_name:
- Excel.Workbook.AfterXmlExport
ms.assetid: fe1e0a53-9f4e-ac88-58f7-fe420e57cabd
ms.date: 05/25/2019
ms.localizationpriority: medium
---


# Workbook.AfterXmlExport event (Excel)

Occurs after Microsoft Excel saves or exports XML data from the specified workbook. 


## Syntax

_expression_.**AfterXmlExport** (_Map_, _Url_, _Result_)

_expression_ A variable that represents a **[Workbook](Excel.Workbook.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Map_|Required| **[XmlMap](Excel.XmlMap.md)**|The schema map that was used to save or export data.|
| _Url_|Required| **String**|The location of the XML file that was exported.|
| _Result_|Required| **[XlXmlExportResult](excel.xlxmlexportresult.md)**|Indicates the results of the save or export operation.|

## Return value

**Nothing**




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]