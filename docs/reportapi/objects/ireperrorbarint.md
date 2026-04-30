---
title: "IRepErrorBarInt"
description: "The ErrorBar object provides the properties of the x and y error bars in a 2D axis system in DIAdem REPORT."
---

# IRepErrorBarInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ErrorBar

The ErrorBar object provides the properties of the x and y error bars in a 2D axis system in DIAdem REPORT.

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
oMyErrorBars = oMyCurve.Shape.Extensions.ErrorBars
oMyErrorBars.Line.LineType = dd.eLineTypeSolid
oMyErrorBars.YErrorBar.Type = dd.eErrorbarPositiveAndNegative
oMyErrorBars.YErrorBar.PercentageErrorValue = 10
oMyErrorBars.EndCap.Type = dd.eErrorbarDisplaySpike
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireperrorbarint-absoluteerrorvalue/">AbsoluteErrorValue</a> | <a href="../../properties/ireperrorbarint-errorchannelnegative/">ErrorChannelNegative</a> | <a href="../../properties/ireperrorbarint-errorchannelpositive/">ErrorChannelPositive</a> | <a href="../../properties/ireperrorbarint-errortype/">ErrorType</a> | <a href="../../properties/ireperrorbarint-percentageerrorvalue/">PercentageErrorValue</a> | <a href="../../properties/ireperrorbarint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2errorbarsadditionalint/">2DAdditionalErrorBars</a>.<a href="../../properties/irepd2errorbarsadditionalint-xerrorbar/">XErrorBar</a> | <a href="../irepd2errorbarsadditionalint/">2DAdditionalErrorBars</a>.<a href="../../properties/irepd2errorbarsadditionalint-yerrorbar/">YErrorBar</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepErrorBarInt.htm`*
