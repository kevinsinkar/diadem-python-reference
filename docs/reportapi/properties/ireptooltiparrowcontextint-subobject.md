---
title: "IRepToolTipArrowContextInt.SubObject"
description: "Returns the subobject of an arrow in DIAdem REPORT when DIAdem calls the event assigned to the OnArrow for ToolTipEvents property. DIAdem calls this event if yo"
---

# IRepToolTipArrowContextInt.SubObject

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SubObject for ToolTipArrowContext

Returns the subobject of an arrow in DIAdem REPORT when DIAdem calls the event assigned to the OnArrow for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Signature

```python
return_value = obj.SubObject
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note  </strong>To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.NewLayout()
oMyArrow = dd.Report.ActiveSheet.Objects.Add(eReportObjectArrow,"MyArrow")
oMyArrow.ArrowHeadAtBegin = eArrowHeadPoint
oMyArrow.ArrowHeadAtEnd = eArrowHeadStandardArrow
oMyArrowPosition = oMyArrow.Position.ByCoordinate
oMyArrowPosition.X1 = 10
oMyArrowPosition.X2 = 40
oMyArrowPosition.Y1 = 30
oMyArrowPosition.Y2 = 90

# This event will be raised if the mouse is moved AND the shift key pressed
dd.Report.Events.ToolTip.OnArrow = "MyToolTipEvent"
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

*Source: `ReportApi/properties/Report_property_SubObject_IRepToolTipArrowContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
