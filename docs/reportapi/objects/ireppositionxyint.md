---
title: "IRepPositionXYInt"
description: "The ObjectPositionXY object provides the position of a text in DIAdem REPORT."
---

# IRepPositionXYInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ObjectPositionXY

The ObjectPositionXY object provides the position of a text in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "This is a text"
oMyPosition = oMyText.PositionXY
oMyPosition.RelativePosition = dd.eRelativePositionRightTop
oMyPosition.X = 10
oMyPosition.Y = 20
oMyPosition.Angle = 45
oMyFont = oMyText.Font
oMyFont.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFont.Name = "Tahoma"
oMyFont.Size = 10
oMyFont.Border = True
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppositionxyint-angle/">Angle</a> | <a href="../../properties/ireppositionxyint-relativeposition/">RelativePosition</a> | <a href="../../properties/ireppositionxyint-x/">X</a> | <a href="../../properties/ireppositionxyint-y/">Y</a> | <a href="../../properties/ireppositionxyint-zorder/">ZOrder</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptextsimpleint/">Text</a>.<a href="../../properties/ireptextsimpleint-positionxy/">PositionXY</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPositionXYInt.htm`*
