---
title: "IRepPolarCurveInt.UseCurveExpansion"
description: "Specifies whether DIAdem REPORT enables the curve expansion when displaying polar curves."
---

# IRepPolarCurveInt.UseCurveExpansion

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseCurveExpansion for PolarCurve

Specifies whether DIAdem REPORT enables the curve expansion when displaying polar curves.

## Signature

```python
obj.UseCurveExpansion
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "TR_M17_QT_32-1.tdm","TDM","")
dd.Report.NewLayout()
oMyReportSettings = dd.Report.Settings
oMyReportSettings.CurveExpansion.Enable = True
oMyReportSettings.CurveExpansion.AttributeList.Enable = True
oMyPolarSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarSystem")
oMyPos = oMyPolarSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyPolarCurve = oMyPolarSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyPolarCurve")
oMyPolarCurve.Shape.XChannel.Reference = ""
oMyPolarCurve.Shape.YChannel.Reference = "Temp_A"
oMyPolarCurve.UseCurveExpansion = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseCurveExpansion_IRepPolarCurveInt.htm`*
