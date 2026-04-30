---
title: "IToBirdsEyeViewChartInt.YEnd"
description: "Returns the end of the value range of the y-axis in a bird's eye view display in DIAdem VIEW."
---

# IToBirdsEyeViewChartInt.YEnd

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: YEnd for BirdsEyeView

Returns the end of the value range of the y-axis in a bird's eye view display in DIAdem VIEW.

## Signature

```python
obj.YEnd
```

## Python example

```python
if dd.View.ActiveSheet.ActiveArea.DisplayObjType == "BirdsEyeView" :
    oMyChart = dd.View.ActiveSheet.ActiveArea.DisplayObj
    dd.LogfileWrite("XBegin: " + dd.Str(oMyChart.XBegin) + "\r\n" + "XEnd: " + dd.Str(oMyChart.XEnd) + "\r\n" +"YBegin: " + dd.Str(oMyChart.YBegin) + "\r\n" + "YEnd: " + dd.Str(oMyChart.YEnd))
else:
    dd.MsgBoxDisp("No BirdsEyeView area")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2> </h2>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_YEnd_IToBirdsEyeViewChartInt.htm`*
