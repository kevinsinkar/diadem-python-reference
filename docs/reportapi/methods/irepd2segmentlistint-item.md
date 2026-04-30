---
title: "IRepD2SegmentListInt.Item"
description: "Returns the background segment associated with a specific index in a 2D axis system in DIAdem REPORT."
---

# IRepD2SegmentListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for 2DBackgroundSegments

Returns the background segment associated with a specific index in a 2D axis system in DIAdem REPORT.

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
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "examples\\data\\Segment.tdm","TDM","")
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNewCurve")
oMySgementList = oMy2DaxisSystem.Settings.BackgroundSegments
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMySgementList.Add()
print(oMySgementList.Count)
oMySgementList(1).XChannel.Reference = "[1]/[3]"
oMySgementList(1).YChannel.Reference = "[1]/[4]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepD2SegmentListInt.htm`*
