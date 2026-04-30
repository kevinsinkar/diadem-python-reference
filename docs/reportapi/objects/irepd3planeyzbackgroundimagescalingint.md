---
title: "IRepD3PlaneYZBackgroundImageScalingInt"
description: "The 3DPlaneYZBackgroundImageScaling object provides the scaling properties of a background graphic of the yz-plane in a 3D axis system, in DIAdem REPORT."
---

# IRepD3PlaneYZBackgroundImageScalingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DPlaneYZBackgroundImageScaling

The 3DPlaneYZBackgroundImageScaling object provides the scaling properties of a background graphic of the yz-plane in a 3D axis system, in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3planeyzbackgroundimagescalingint-enable/">Enable</a> | <a href="../../properties/irepd3planeyzbackgroundimagescalingint-ybegin/">YBegin</a> | <a href="../../properties/irepd3planeyzbackgroundimagescalingint-yend/">YEnd</a> | <a href="../../properties/irepd3planeyzbackgroundimagescalingint-zbegin/">ZBegin</a> | <a href="../../properties/irepd3planeyzbackgroundimagescalingint-zend/">ZEnd</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3planeyzbackgroundimageint/">3DPlaneYZBackgroundImage</a>.<a href="../../properties/irepd3planeyzbackgroundimageint-scaling/">Scaling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3PlaneYZBackgroundImageScalingInt.htm`*
