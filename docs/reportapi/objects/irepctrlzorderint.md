---
title: "IRepCtrlZOrderInt"
description: "The ZOrder object provides the object order in DIAdem REPORT."
---

# IRepCtrlZOrderInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ZOrder

The ZOrder object provides the object order in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyCircle = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")
oMyCircle.BackgroundColor.SetPredefinedColor(dd.ePredefinedColorBlue)
oMyFrame = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFrame,"MyFrame")
oMyFrame.BackgroundColor.SetPredefinedColor(dd.ePredefinedColorRed)
oMyFrame.Position.ZOrder.Move(-1)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepctrlzorderint-order/">Order</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepctrlzorderint-move/">Move</a> | <a href="../../methods/irepctrlzorderint-movetobackground/">MoveToBackground</a> | <a href="../../methods/irepctrlzorderint-movetoforeground/">MoveToForeground</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppositionint/">ObjectPosition</a>.<a href="../../properties/ireppositionint-zorder/">ZOrder</a> | <a href="../ireppositionxyint/">ObjectPositionXY</a>.<a href="../../properties/ireppositionxyint-zorder/">ZOrder</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCtrlZOrderInt.htm`*
