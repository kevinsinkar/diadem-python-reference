---
title: "IRepSpiderShapeObjLineInt.Channel"
description: "Specifies in a curve in the display type Line in a spider axis system the channel whose values DIAdem REPORT displays."
---

# IRepSpiderShapeObjLineInt.Channel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Channel for SpiderLine

Specifies in a curve in the display type Line in a spider axis system the channel whose values DIAdem REPORT displays.

## Signature

```python
return_value = obj.Channel
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Channel_IRepSpiderShapeObjLineInt.htm`*
