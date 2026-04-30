---
title: "IRepD3ShapeObjSurfaceSettingsInt.Type"
description: "Specifies in DIAdem REPORT the type of surface and line display of a 3D axis system in the Surface display mode."
---

# IRepD3ShapeObjSurfaceSettingsInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for 3DSurfaceSettings

Specifies in DIAdem REPORT the type of surface and line display of a 3D axis system in the Surface display mode.

## Signature

```python
obj.Type
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
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Type = dd.e3DSurfaceTypeLineY
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepD3ShapeObjSurfaceSettingsInt.htm`*
