---
title: "IRepD3CharacteristicDiagramPointsAdditionalInt.UseDataReductionValues"
description: "Specifies whether DIAdem uses the measured values or the values from the data reduction to display the maximum and minimum points as well as the measuring point"
---

# IRepD3CharacteristicDiagramPointsAdditionalInt.UseDataReductionValues

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseDataReductionValues for 3DAdditionalCharacteristicDiagramPoints

Specifies whether DIAdem uses the measured values or the values from the data reduction to display the maximum and minimum points as well as the measuring points in a 3D axis system with the Map display type in DIAdem REPORT. DIAdem considers this setting only if the data has a triplet structure and if the display type is not a differential characteristic diagram.

## Signature

```python
obj.UseDataReductionValues
```

## Python example

```python
o3DAdditionalCharacteristicDiagramPoints = dd.Report.ActiveSheet.Objects.Item("My3DAxisSystem").Curves3D.Item("MyNew3DCurve").Shape.Extensions.MeasurementPoints
o3DAdditionalCharacteristicDiagramPoints.UseDataReductionValues  = True
o3DAdditionalCharacteristicDiagramPoints.Visible                 = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseDataReductionValues_IRepD3CharacteristicDiagramPointsAdditionalInt.htm`*
