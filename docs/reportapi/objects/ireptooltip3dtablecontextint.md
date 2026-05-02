---
title: "IRepToolTip3DTableContextInt"
description: "The ToolTip3DTableContext object provides information on a 3D table in DIAdem REPORT when DIAdem calls the event assigned to the OnTable3D for ToolTipEvents pro"
---

# IRepToolTip3DTableContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ToolTip3DTableContext

The ToolTip3DTableContext object provides information on a 3D table in DIAdem REPORT when DIAdem calls the event assigned to the OnTable3D for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Data.Root.Clear()
DataFileLoad(DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DTable = dd.Report.ActiveSheet.Objects.Add(eReportObject3DTable,"My2DTable")
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

# This event will be raised if the mouse is moved AND the shift key pressed
dd.Report.Events.ToolTip.OnTable3D = "MyToolTipEvent"
dd.Report.Refresh()
```

```python
def MyToolTipEvent(Context,ToolTipText):
    oSubObject = Context.SubObject
    ToolTipText = "Sheet: " + Context.Sheet.Name + "\r\n" + "Sub object" + "\r\n" + "Name: " + oSubObject.Name + "\r\n" + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
    ToolTipText = ToolTipText + "\r\n" + "X position: " + Context.Position.X + "\r\n" + "Y position: " + Context.Position.Y
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptooltip3dtablecontextint-position/">Position</a> | <a href="../../properties/ireptooltip3dtablecontextint-sheet/">Sheet</a> | <a href="../../properties/ireptooltip3dtablecontextint-subobject/">SubObject</a> | <a href="../../properties/ireptooltip3dtablecontextint-table3d/">Table3D</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepToolTip3DTableContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
