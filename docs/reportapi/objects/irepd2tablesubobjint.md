---
title: "IRepD2TableSubObjInt"
description: "The D2TableSubObj object provides information on a subobject of a 2D table in DIAdem REPORT when DIAdem calls the event assigned to the OnTable2D for ToolTipEve"
---

# IRepD2TableSubObjInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: D2TableSubObj

The D2TableSubObj object provides information on a subobject of a 2D table in DIAdem REPORT when DIAdem calls the event assigned to the OnTable2D for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyColumn = oMy2DTable.Columns.Add(e2DTableColumnChannel)
oMyColumn.Channel.Reference = "[1]/[2]"
oMyColumn.Settings.Alignment = eTableAlignmentDecimalPoint
oMyColumn.Settings.Format = "d.dddd"

# This event will be raised if the mouse is moved AND the shift key pressed
dd.Report.Events.ToolTip.OnTable2D = "MyToolTipEvent"
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
<p><a href="../../properties/irepd2tablesubobjint-name/">Name</a> | <a href="../../properties/irepd2tablesubobjint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptooltip2dtablecontextint/">ToolTip2DTableContext</a>.<a href="../../properties/ireptooltip2dtablecontextint-subobject/">SubObject</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2TableSubObjInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
