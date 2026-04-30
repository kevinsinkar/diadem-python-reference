---
title: "IRepD3ShapeObjLineSettingsInt"
description: "The 3DLineSettings object provides the properties of the curve parameters of a 3D axis system in the 3D curve display mode in DIAdem REPORT."
---

# IRepD3ShapeObjLineSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DLineSettings

The 3DLineSettings object provides the properties of the curve parameters of a 3D axis system in the 3D curve display mode in DIAdem REPORT.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeLine, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[3]/[1]"
oMyShape.YChannel.Reference = "[3]/[2]"
oMyShape.ZChannel.Reference = "[3]/[3]"
oMyShape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyShape.Settings.Line.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3shapeobjlinesettingsint-displayas3dcurve/">DisplayAs3DCurve</a> | <a href="../../properties/irepd3shapeobjlinesettingsint-line/">Line</a> | <a href="../../properties/irepd3shapeobjlinesettingsint-palette/">Palette</a> | <a href="../../properties/irepd3shapeobjlinesettingsint-projecttocoordinateplanexy/">ProjectToCoordinatePlaneXY</a> | <a href="../../properties/irepd3shapeobjlinesettingsint-projecttocoordinateplanexz/">ProjectToCoordinatePlaneXZ</a> | <a href="../../properties/irepd3shapeobjlinesettingsint-projecttocoordinateplaneyz/">ProjectToCoordinatePlaneYZ</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjlineint/">3DLine</a>.<a href="../../properties/irepd3shapeobjlineint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjLineSettingsInt.htm`*
