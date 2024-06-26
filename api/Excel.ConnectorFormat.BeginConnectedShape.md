---
title: ConnectorFormat.BeginConnectedShape property (Excel)
keywords: vbaxl10.chm646078
f1_keywords:
- vbaxl10.chm646078
api_name:
- Excel.ConnectorFormat.BeginConnectedShape
ms.assetid: 9ff6c949-72c7-32e9-d1dc-6a0a3b861135
ms.date: 04/23/2019
ms.localizationpriority: medium
---


# ConnectorFormat.BeginConnectedShape property (Excel)

Returns a **[Shape](Excel.Shape.md)** object that represents the shape that the beginning of the specified connector is attached to. Read-only.


## Syntax

_expression_.**BeginConnectedShape**

_expression_ A variable that represents a **[ConnectorFormat](Excel.ConnectorFormat.md)** object.


## Remarks

If the beginning of the specified connector isn't attached to a shape, this property generates an error.


## Example

This example assumes that _myDocument_ already contains two shapes attached by a connector named Conn1To2. The code adds a rectangle and a connector to _myDocument_. The beginning of the new connector will be attached to the same connection site as the beginning of the connector named Conn1To2, and the end of the new connector will be attached to connection site one on the new rectangle.

```vb
Set myDocument = Worksheets(1) 
With myDocument.Shapes 
 Set r3 = .AddShape(msoShapeRectangle, 450, 190, 200, 100) 
 .AddConnector(msoConnectorCurve, 0, 0, 10, 10).Name = _ 
 "Conn1To3" 
 With .Item("Conn1To2").ConnectorFormat 
 beginConnSite1 = .BeginConnectionSite 
 Set beginConnShape1 = .BeginConnectedShape 
 End With 
 With .Item("Conn1To3").ConnectorFormat 
 .BeginConnect beginConnShape1, beginConnSite1 
 .EndConnect r3, 1 
 End With 
End With
```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]