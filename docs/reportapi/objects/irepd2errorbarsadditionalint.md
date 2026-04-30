---
title: "IRepD2ErrorBarsAdditionalInt"
description: "The 2DAdditionalErrorBars object provides the properties of an error bar in a 2D axis system in DIAdem REPORT."
---

# IRepD2ErrorBarsAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAdditionalErrorBars

The 2DAdditionalErrorBars object provides the properties of an error bar in a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.Extensions.ErrorBars.XErrorBar.Type = dd.eErrorbarPositiveAndNegative
oMyShape.Extensions.ErrorBars.XErrorBar.PercentageErrorValue = 10
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2errorbarsadditionalint-endcap/">EndCap</a> | <a href="../../properties/irepd2errorbarsadditionalint-line/">Line</a> | <a href="../../properties/irepd2errorbarsadditionalint-xerrorbar/">XErrorBar</a> | <a href="../../properties/irepd2errorbarsadditionalint-yerrorbar/">YErrorBar</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjlineandpointsextensionsint/">2DLineAndPointsExtensions</a>.<a href="../../properties/irepd2shapeobjlineandpointsextensionsint-errorbars/">ErrorBars</a> | <a href="../irepd2shapeobjlineextensionsint/">2DLineExtensions</a>.<a href="../../properties/irepd2shapeobjlineextensionsint-errorbars/">ErrorBars</a> | <a href="../irepd2shapeobjspecialcombinationextensionsint/">2DSpecialCombinationExtensions</a>.<a href="../../properties/irepd2shapeobjspecialcombinationextensionsint-errorbars/">ErrorBars</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ErrorBarsAdditionalInt.htm`*
