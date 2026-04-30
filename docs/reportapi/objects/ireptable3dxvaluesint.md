---
title: "IRepTable3DXValuesInt"
description: "The 3DTableXValues object provides the properties of the x-values in a 3D table in DIAdem REPORT."
---

# IRepTable3DXValuesInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DTableXValues

The 3DTableXValues object provides the properties of the x-values in a 3D table in DIAdem REPORT.

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
oMyY.Header.TitleSize = 50
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable3dxvaluesint-alignment/">Alignment</a> | <a href="../../properties/ireptable3dxvaluesint-angle/">Angle</a> | <a href="../../properties/ireptable3dxvaluesint-channel/">Channel</a> | <a href="../../properties/ireptable3dxvaluesint-font/">Font</a> | <a href="../../properties/ireptable3dxvaluesint-format/">Format</a> | <a href="../../properties/ireptable3dxvaluesint-header/">Header</a> | <a href="../../properties/ireptable3dxvaluesint-indexbegin/">IndexBegin</a> | <a href="../../properties/ireptable3dxvaluesint-indexend/">IndexEnd</a> | <a href="../../properties/ireptable3dxvaluesint-indexincrement/">IndexIncrement</a> | <a href="../../properties/ireptable3dxvaluesint-useautoindex/">UseAutoIndex</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable3dint/">3DTable</a>.<a href="../../properties/ireptable3dint-x/">X</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable3DXValuesInt.htm`*
