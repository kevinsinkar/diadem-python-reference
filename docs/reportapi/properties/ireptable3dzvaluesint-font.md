---
title: "IRepTable3DZValuesInt.Font"
description: "Specifies the font of the z-values in a 3D table in DIAdem REPORT."
---

# IRepTable3DZValuesInt.Font

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Font for 3DTableZValues

Specifies the font of the z-values in a 3D table in DIAdem REPORT.

## Signature

```python
return_value = obj.Font
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DTable,"My2DTable")
oMyPosition = oMy3DTable.Position.ByBorder
oMyPosition.Top = 20
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 20
oMyX = oMy3DTable.X
oMyY = oMy3DTable.Y
oMyZ = oMy3DTable.Z
oMySettings = oMy3DTable.Settings
oMySettings.UseAutoFontSize = False
oMyX.Channel.Reference = "[2]/[1]"
oMyX.Font.Size = 2
oMyX.Font.Name = "Times Roman"()
oMyX.Format = "d.dd"
oMyY.Channel.Reference = "[2]/[2]"
oMyY.Font.Size = 2
oMyY.Font.Name = "Arial"
oMyY.Format = "d.dd"
oMyZ.Channel.Reference = "[2]/[3]"
oMyZ.Font.Size = 2
oMyZ.Font.Name = "Times Roman"()
oMyZ.Format = "d.dd"
oMyX.Header.TitleSize = 70
oMyX.Header.Font.Name = "Times Roman"()
oMyY.Header.TitleSize = 70
oMyY.Header.Font.Name = "Arial"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Font_IRepTable3DZValuesInt.htm`*
