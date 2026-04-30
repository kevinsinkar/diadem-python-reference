---
title: "IRepChannelReferenceListInt.Item"
description: "Returns in DIAdem REPORT in a 2D axis system in the display mode Stacked Bars or Grouped Bars the y-channel of a specific name of index."
---

# IRepChannelReferenceListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for Channels

Returns in DIAdem REPORT in a 2D axis system in the display mode Stacked Bars or Grouped Bars the y-channel of a specific name of index.

## Signature

```python
return_value = obj.Item(Index)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")

oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")

oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeStackedBars, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = ""
oMy2DCurve.Shape.YChannels.Add("[4]/[1]")
oMy2DCurve.Shape.YChannels.Add("[4]/[2]")
oMy2DCurve.Shape.YChannels.Add("[4]/[3]")

for I in range( 1, oMy2DCurve.Shape.YChannels.Count+1):
    MyChannels = MyChannels + "\r\n" + "Channel Reference " + I + ": " + oMy2DCurve.Shape.YChannels.Item(I).Reference

print(MyChannels)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepChannelReferenceListInt.htm`*
