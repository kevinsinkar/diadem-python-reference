---
title: "IRepFrameSubObjInt.Name"
description: "Returns the name of the subobject of a rectangle in DIAdem REPORT when DIAdem calls the event assigned to the OnFrame for ToolTipEvents property. DIAdem calls t"
---

# IRepFrameSubObjInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for FrameSubObj

Returns the name of the subobject of a rectangle in DIAdem REPORT when DIAdem calls the event assigned to the OnFrame for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Signature

```python
obj.Name
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
oMyFrame = dd.Report.ActiveSheet.Objects.Add(eReportObjectFrame,"MyFrame")
oMyFrame.ForceSquare = True
oMyFrame.Position.ByCoordinate.X1 = 10
oMyFrame.Position.ByCoordinate.X2 = 40
oMyFrame.Position.ByCoordinate.Y1 = 50
oMyFrame.Position.ByCoordinate.Y2 = 80

# This event will be raised if the mouse is moved AND the shift key pressed
dd.Report.Events.ToolTip.OnFrame = "MyToolTipEvent"
dd.Report.Refresh()
```

```python
def MyToolTipEvent(Context,ToolTipText):
    oSubObject = Context.SubObject
    ToolTipText = "Sheet: " + Context.Sheet.Name + VBCrLf + "Sub object" + VBCrLf + "Name: " + oSubObject.Name + VBCrLf + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
    ToolTipText = ToolTipText + VBCrLf + "X position: " + Context.Position.X + VBCrLf + "Y position: " + Context.Position.Y
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Name_IRepFrameSubObjInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
