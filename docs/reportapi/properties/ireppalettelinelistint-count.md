---
title: "IRepPaletteLineListInt.Count"
description: "Changes the number of palette colors for the curve display in a 2D axis system in DIAdem REPORT or returns this value."
---

# IRepPaletteLineListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for PaletteLines

Changes the number of palette colors for the curve display in a 2D axis system in DIAdem REPORT or returns this value.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMyCurves = oMyReportObj.Curves2D
        for oMyCurve in oMyCurves:
            dd.MsgBoxDisp("Object name: " + oMyCurve.Name + "\r\n" + "Number of isolines: " + oMyCurve.Shape.Settings.Palette.Lines.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepPaletteLineListInt.htm`*
