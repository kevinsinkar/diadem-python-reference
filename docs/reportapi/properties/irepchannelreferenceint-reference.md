---
title: "IRepChannelReferenceInt.Reference"
description: "Specifies the channel reference in DIAdem REPORT. Assign an empty string to a channel reference so that you do not need to assign a channel."
---

# IRepChannelReferenceInt.Reference

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Reference for ChannelReference

Specifies the channel reference in DIAdem REPORT. Assign an empty string to a channel reference so that you do not need to assign a channel.

## Signature

```python
obj.Reference
```

## Python example

```python
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Reference_IRepChannelReferenceInt.htm`*
