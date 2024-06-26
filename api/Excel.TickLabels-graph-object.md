---
title: TickLabels object (Excel Graph)
keywords: vbagr10.chm5208056
f1_keywords:
- vbagr10.chm5208056
api_name:
- Excel.TickLabels
ms.assetid: d71b6cf2-c4ad-66f3-f7c2-8219f9ec21b1
ms.date: 04/06/2019
ms.localizationpriority: medium
---


# TickLabels object (Excel Graph)

Represents the tick-mark labels associated with tick marks on the specified chart axis. 

This object isn't a collection. There's no object that represents a single tick-mark label; you must return all the tick-mark labels as a unit.

## Remarks

Tick-mark label text for the category axis comes from the name of the associated category in the chart. The default tick-mark label text for the category axis is the number that indicates the position of the category relative to the left end of this axis. 

To change the number of unlabeled tick marks between tick-mark labels, you must change the **[TickLabelSpacing](excel.ticklabelspacing.md)** property for the category axis.

Tick-mark label text for the value axis is calculated based on the **[MajorUnit](excel.majorunit.md)**, **[MinimumScale](excel.minimumscale.md)**, and **[MaximumScale](excel.maximumscale.md)** properties of the value axis. To change the tick-mark label text for the value axis, you must change the values of these properties.

Use the **[TickLabels](excel.ticklabels-graph-property.md)** property to return the **TickLabels** object. 



## Example

The following example sets the number format for the tick-mark labels on the value axis in the chart.

```vb
myChart.Axes(xlValue).TickLabels.NumberFormat = "0.00"
```

## See also

- [Excel Graph Visual Basic Reference](overview/excel/graph-visual-basic-reference.md)
- [Excel Object Model Reference](overview/excel/object-model.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]