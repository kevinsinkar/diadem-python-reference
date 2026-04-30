---
title: "IRepD3PlaneYZBackgroundImageInt.Scaling"
description: "Specifies the scaling of the background graphic of the yz-plane in a 3D axis system in DIAdem REPORT."
---

# IRepD3PlaneYZBackgroundImageInt.Scaling

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Scaling for 3DPlaneYZBackgroundImage

Specifies the scaling of the background graphic of the yz-plane in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Scaling
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
oMyBackground = oMySettings.PlaneYZ.BackgroundImage
oMyBackground.FileName = "Example1.png"
oMyScaling = oMyBackground.Scaling
oMyScaling.Enable = True
oMyScaling.YBegin = 0.2
oMyScaling.YEnd = 0.8
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

*Source: `ReportApi/properties/Report_property_Scaling_IRepD3PlaneYZBackgroundImageInt.htm`*
