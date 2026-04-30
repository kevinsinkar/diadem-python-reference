---
title: "IRepD3ShapeObjIsolinesInt.NumberOfIsoChannels"
description: "Specifies the number of isolines in a 3D axis system which DIAdem REPORT uses in the Isolines display mode."
---

# IRepD3ShapeObjIsolinesInt.NumberOfIsoChannels

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: NumberOfIsoChannels for 3DIsolines

Specifies the number of isolines in a 3D axis system which DIAdem REPORT uses in the Isolines display mode.

## Signature

```python
return_value = obj.NumberOfIsoChannels
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeIsolines, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.IsolineType = dd.e3DIsolineTypeXY
oMyShape.XChannel.Reference = "[4]/[1]"
oMyShape.YChannel.Reference = "[4]/[2]"
oMyShape.NumberOfIsoChannels.Count = 3
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_NumberOfIsoChannels_IRepD3ShapeObjIsolinesInt.htm`*
