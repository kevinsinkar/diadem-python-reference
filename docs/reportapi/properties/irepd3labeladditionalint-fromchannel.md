---
title: "IRepD3LabelAdditionalInt.FromChannel"
description: "Specifies whether DIAdem REPORT uses values from another channel for the additional curve labels of a 3D curve. Assign the value TRUE to the Visible property so"
---

# IRepD3LabelAdditionalInt.FromChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: FromChannel for 3DAdditionalLabel

Specifies whether DIAdem REPORT uses values from another channel for the additional curve labels of a 3D curve. Assign the value TRUE to the Visible property so that DIAdem REPORT displays the values.

## Signature

```python
return_value = obj.FromChannel
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMyShape.ZChannel.Reference = "[6]/[3]"
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = True
oMyLabel.FromChannel.Visible = False
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_FromChannel_IRepD3LabelAdditionalInt.htm`*
