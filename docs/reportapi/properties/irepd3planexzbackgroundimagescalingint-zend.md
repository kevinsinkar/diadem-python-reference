---
title: "IRepD3PlaneXZBackgroundImageScalingInt.ZEnd"
description: "Specifies the end value in z-direction for scaling the background graphic of the xz-plane in a 3D axis system in DIAdem REPORT."
---

# IRepD3PlaneXZBackgroundImageScalingInt.ZEnd

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ZEnd for 3DPlaneXZBackgroundImageScaling

Specifies the end value in z-direction for scaling the background graphic of the xz-plane in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.ZEnd
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
oMyBackground = oMySettings.PlaneXZ.BackgroundImage
oMyBackground.FileName = "Example1.png"
oMyScaling = oMyBackground.Scaling
oMyScaling.Enable = True
oMyScaling.XBegin = 0.2
oMyScaling.XEnd = 0.8
oMyScaling.ZBegin = -0.5
oMyScaling.ZEnd = 0
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ZEnd_IRepD3PlaneXZBackgroundImageScalingInt.htm`*
