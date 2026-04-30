---
title: "IRepShadowInt"
description: "The Shadow object provides the shadow properties of a Rectangle or Circle type object in DIAdem REPORT."
---

# IRepShadowInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Shadow

The Shadow object provides the shadow properties of a Rectangle or Circle type object in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyFrame = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFrame,"MyFrame")
oMyBackgroundColor = oMyFrame.BackgroundColor
oMyBackgroundColor.SetPredefinedColor(dd.eColorIndexRed )
oMyPosition = oMyFrame.Position.ByCoordinate
oMyPosition.X1 = 10
oMyPosition.X2 = 40
oMyPosition.Y1 = 50
oMyPosition.Y2 = 80
oMyShadow = oMyFrame.Shadow
oMyShadow.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyShadow.Direction = dd.eShadowDirectionLeftBottom
oMyShadow.OffsetX = 1
oMyShadow.OffsetY = 2
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepshadowint-color/">Color</a> | <a href="../../properties/irepshadowint-direction/">Direction</a> | <a href="../../properties/irepshadowint-offsetx/">OffsetX</a> | <a href="../../properties/irepshadowint-offsety/">OffsetY</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepfreeframeint/">Frame</a>.<a href="../../properties/irepfreeframeint-shadow/">Shadow</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepShadowInt.htm`*
