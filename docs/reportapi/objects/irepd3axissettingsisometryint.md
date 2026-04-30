---
title: "IRepD3AxisSettingsIsometryInt"
description: "The 3DAxisSettingsIsometry object provides the properties for isometric axis adjustment of a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisSettingsIsometryInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAxisSettingsIsometry

The 3DAxisSettingsIsometry object provides the properties for isometric axis adjustment of a 3D axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
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
oMyIsometry = oMy3DAxisSystem.Settings.Isometry
oMyIsometry.Type = dd.e3DAxisIsometryXY
oMyIsometry.Length = 50
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3axissettingsisometryint-fitintoarea/">FitIntoArea</a> | <a href="../../properties/irepd3axissettingsisometryint-length/">Length</a> | <a href="../../properties/irepd3axissettingsisometryint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3axissettingsint/">3DAxisSettings</a>.<a href="../../properties/irepd3axissettingsint-isometry/">Isometry</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3AxisSettingsIsometryInt.htm`*
