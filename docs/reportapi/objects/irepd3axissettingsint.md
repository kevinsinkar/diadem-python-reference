---
title: "IRepD3AxisSettingsInt"
description: "The 3DAxisSettings object provides the properties of a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAxisSettings

The 3DAxisSettings object provides the properties of a 3D axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeMatrix2D, "MyNew3DCurve")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMy3DAxisSystem.Settings
oMySettings.RotationAngleXY = 90
oMySettings.RotationAngleZ = 270
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3axissettingsint-enableinteractiverotation/">EnableInteractiveRotation</a> | <a href="../../properties/irepd3axissettingsint-isometry/">Isometry</a> | <a href="../../properties/irepd3axissettingsint-planexy/">PlaneXY</a> | <a href="../../properties/irepd3axissettingsint-planexz/">PlaneXZ</a> | <a href="../../properties/irepd3axissettingsint-planeyz/">PlaneYZ</a> | <a href="../../properties/irepd3axissettingsint-rotationanglexy/">RotationAngleXY</a> | <a href="../../properties/irepd3axissettingsint-rotationanglez/">RotationAngleZ</a> | <a href="../../properties/irepd3axissettingsint-usecurvetransformation/">UseCurveTransformation</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3axisint/">3DAxisSystem</a>.<a href="../../properties/irepd3axisint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3AxisSettingsInt.htm`*
