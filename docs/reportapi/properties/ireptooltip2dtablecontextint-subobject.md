---
title: "IRepToolTip2DTableContextInt.SubObject"
description: "Returns a subobject type of a 2D table in DIAdem REPORT when DIAdem calls the event associated with the OnTable2D for ToolTipEvents property. DIAdem calls this "
---

# IRepToolTip2DTableContextInt.SubObject

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SubObject for ToolTip2DTableContext

Returns a subobject type of a 2D table in DIAdem REPORT when DIAdem calls the event associated with the OnTable2D for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Signature

```python
return_value = obj.SubObject
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SubObject_IRepToolTip2DTableContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
