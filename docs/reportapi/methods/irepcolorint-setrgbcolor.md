---
title: "IRepColorInt.SetRGBColor"
description: "Assigns a color to an object in DIAdem REPORT. The method also specifies the Color object properties which are necessary to display a color."
---

# IRepColorInt.SetRGBColor

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: SetRGBColor for Color

Assigns a color to an object in DIAdem REPORT. The method also specifies the Color object properties which are necessary to display a color.

## Signature

```python
obj.SetRGBColor(RGB)
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DAxisSystem.Settings.UseIndividualAxisStyle = True
oMyXLine = oMy2DAxisSystem.XAxis.Line
oMyXLine.Color.SetRGBColor(dd.RGB(255,0,0))
oMyXLine.UseCurveColor = False
oMyXLine.Width = dd.eLineWidth0100
oMyYLine = oMy2DAxisSystem.YAxis.Line
oMyYLine.Color.SetRGBColor(dd.RGB(0, 0, 255))
oMyYLine.UseCurveColor = False
oMyYLine.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_SetRGBColor_IRepColorInt.htm`*
