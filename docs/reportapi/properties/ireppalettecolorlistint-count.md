---
title: "IRepPaletteColorListInt.Count"
description: "Changes the number of palette colors in a 2D table in DIAdem REPORT or returns this value."
---

# IRepPaletteColorListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for TablePaletteColors

Changes the number of palette colors in a 2D table in DIAdem REPORT or returns this value.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        oMyReportObj.Settings.Palette.Count = 10
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of palette colors: " + oMyReportObj.Settings.Palette.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepPaletteColorListInt.htm`*
