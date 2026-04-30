---
title: "IRepPaletteColorInt.Color"
description: "Specifies the palette color for the 2D table display in DIAdem REPORT."
---

# IRepPaletteColorInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for TablePaletteColor

Specifies the palette color for the 2D table display in DIAdem REPORT.

## Signature

```python
return_value = obj.Color
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        oMyPalette = oMyReportObj.Settings.Palette
        oMyPalette.Count = 10
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of palette colors: " + oMyPalette.Count)
        for i in range( 1, oMyPalette.Count+1):
            sOutput = sOutput + "Palette color " + i + ": "+ oMyPalette.Item(i).Color.ColorIndex + "\r\n"
        dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepPaletteColorInt.htm`*
