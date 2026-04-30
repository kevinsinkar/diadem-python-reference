---
title: "ITo2DChartInt.Segments"
description: "Returns the collection of segments in a 2D axis system in DIAdem VIEW."
---

# ITo2DChartInt.Segments

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Segments for CurveChart2D

Returns the collection of segments in a 2D axis system in DIAdem VIEW.

## Signature

```python
return_value = obj.Segments
```

## Python example

```python
for oMySegment in dd.View.ActiveSheet.ActiveArea.DisplayObj.Segments:
    dd.MsgBoxDisp("X-Channel:" + oMySegment.XChannelName + "\r\n" + "Y-Channel:" + oMySegment.YChannelName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Segments_ITo2DChartInt.htm`*
