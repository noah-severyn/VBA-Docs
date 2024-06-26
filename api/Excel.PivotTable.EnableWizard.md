---
title: PivotTable.EnableWizard property (Excel)
keywords: vbaxl10.chm235108
f1_keywords:
- vbaxl10.chm235108
api_name:
- Excel.PivotTable.EnableWizard
ms.assetid: 3e87af08-711d-cddb-bcc1-0b9179e71cb1
ms.date: 05/08/2019
ms.localizationpriority: medium
---


# PivotTable.EnableWizard property (Excel)

**True** if the PivotTable Wizard is available. The default value is **True**. Read/write **Boolean**.


## Syntax

_expression_.**EnableWizard**

_expression_ A variable that represents a **[PivotTable](Excel.PivotTable.md)** object.


## Remarks

When this property is set, the field wells aren't displayed on the worksheet.


## Example

This example disables the PivotTable Wizard for the first PivotTable report on worksheet one.

```vb
Worksheets(1).PivotTables("Pivot1").EnableWizard = False
```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]