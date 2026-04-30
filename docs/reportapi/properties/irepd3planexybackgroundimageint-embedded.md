---
title: "IRepD3PlaneXYBackgroundImageInt.Embedded"
description: "Specifies whether DIAdem REPORT embeds the background graphic of the xy-plane in a 3D axis system in the layout file."
---

# IRepD3PlaneXYBackgroundImageInt.Embedded

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Embedded for 3DPlaneXYBackgroundImage

Specifies whether DIAdem REPORT embeds the background graphic of the xy-plane in a 3D axis system in the layout file.

## Signature

```python
obj.Embedded
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMy3DAxisSystem.Settings
oMyBackground = oMySettings.PlaneXY.BackgroundImage
oMyBackground.FileName = "Example1.png"
oMyBackground.Embedded = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Embedded_IRepD3PlaneXYBackgroundImageInt.htm`*
