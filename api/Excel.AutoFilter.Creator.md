---
title: AutoFilter.Creator property (Excel)
keywords: vbaxl10.chm537074
f1_keywords:
- vbaxl10.chm537074
api_name:
- Excel.AutoFilter.Creator
ms.assetid: 15231f8b-f5ce-8560-f157-15676d038f89
ms.date: 04/13/2019
ms.localizationpriority: medium
---


# AutoFilter.Creator property (Excel)

Returns a 32-bit integer that indicates the application in which this object was created. Read-only **Long**.


## Syntax

_expression_.**Creator**

_expression_ A variable that represents an **[AutoFilter](Excel.AutoFilter.md)** object.


## Remarks

If the object was created in Microsoft Excel, this property returns the string XCEL, which is equivalent to the hexadecimal number 5843454C. The **Creator** property is designed to be used in Microsoft Excel for the Macintosh, where each application has a four-character creator code. For example, Microsoft Excel has the creator code XCEL.




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]