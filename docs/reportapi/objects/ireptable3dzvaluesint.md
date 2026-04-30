---
title: "IRepTable3DZValuesInt"
description: "The 3DTableZValues object provides the properties of the z-values in a 3D table in DIAdem REPORT."
---

# IRepTable3DZValuesInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DTableZValues

The 3DTableZValues object provides the properties of the z-values in a 3D table in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
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
oMyX.Format = "d.dd"
oMyY.Channel.Reference = "[2]/[2]"
oMyY.Font.Size = 2
oMyY.Format = "d.dd"
oMyZ.Channel.Reference = "[2]/[3]"
oMyZ.Font.Size = 2
oMyZ.Format = "d.dd"
oMyX.Header.TitleSize = 70
oMyY.Header.TitleSize = 70
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable3dzvaluesint-alignment/">Alignment</a> | <a href="../../properties/ireptable3dzvaluesint-angle/">Angle</a> | <a href="../../properties/ireptable3dzvaluesint-channel/">Channel</a> | <a href="../../properties/ireptable3dzvaluesint-font/">Font</a> | <a href="../../properties/ireptable3dzvaluesint-format/">Format</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable3dint/">3DTable</a>.<a href="../../properties/ireptable3dint-z/">Z</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable3DZValuesInt.htm`*
