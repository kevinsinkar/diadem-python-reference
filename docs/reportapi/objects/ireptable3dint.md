---
title: "IRepTable3DInt"
description: "The 3DTable object provides a 3D table in DIAdem REPORT."
---

# IRepTable3DInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DTable

The 3DTable object provides a 3D table in DIAdem REPORT.

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
<p><a href="../../properties/ireptable3dint-index/">Index</a> | <a href="../../properties/ireptable3dint-isselected/">IsSelected</a> | <a href="../../properties/ireptable3dint-name/">Name</a> | <a href="../../properties/ireptable3dint-objecttype/">ObjectType</a> | <a href="../../properties/ireptable3dint-position/">Position</a> | <a href="../../properties/ireptable3dint-selectedelements/">SelectedElements</a> | <a href="../../properties/ireptable3dint-settings/">Settings</a> | <a href="../../properties/ireptable3dint-tagstored/">TagStored</a> | <a href="../../properties/ireptable3dint-tagtemporary/">TagTemporary</a> | <a href="../../properties/ireptable3dint-x/">X</a> | <a href="../../properties/ireptable3dint-y/">Y</a> | <a href="../../properties/ireptable3dint-z/">Z</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireptable3dint-exporttoimage/">ExportToImage</a> | <a href="../../methods/ireptable3dint-select/">Select</a> | <a href="../../methods/ireptable3dint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable3ddropcontextint/">3DTableDropContext</a>.<a href="../../properties/ireptable3ddropcontextint-table/">Table</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptooltip3dtablecontextint/">ToolTip3DTableContext</a>.<a href="../../properties/ireptooltip3dtablecontextint-table3d/">Table3D</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable3DInt.htm`*
