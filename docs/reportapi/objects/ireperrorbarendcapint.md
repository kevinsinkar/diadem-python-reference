---
title: "IRepErrorBarEndCapInt"
description: "The ErrorBarEndCap object provides the properties of the error bars in a 2D axis system in DIAdem REPORT."
---

# IRepErrorBarEndCapInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ErrorBarEndCap

The ErrorBarEndCap object provides the properties of the error bars in a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[6]/[1]"
oMyCurve.Shape.YChannel.Reference = "[6]/[2]"
oMyCurve.Shape.Extensions.ErrorBars.YErrorBar.Type = dd.eErrorbarPositiveAndNegative
oMyCurve.Shape.Extensions.ErrorBars.YErrorBar.PercentageErrorValue = 10
oMyCurve.Shape.Extensions.ErrorBars.EndCap.Type = dd.eErrorbarDisplaySpike
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireperrorbarendcapint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2errorbarsadditionalint/">2DAdditionalErrorBars</a>.<a href="../../properties/irepd2errorbarsadditionalint-endcap/">EndCap</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepErrorBarEndCapInt.htm`*
