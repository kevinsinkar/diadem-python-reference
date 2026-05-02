---
title: "IRepToolTipCircleContextInt.Circle"
description: "Returns a circle in DIAdem REPORT when DIAdem calls the event assigned to the OnCircle for ToolTipEvents property. DIAdem calls this event if you press the shif"
---

# IRepToolTipCircleContextInt.Circle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Circle for ToolTipCircleContext

Returns a circle in DIAdem REPORT when DIAdem calls the event assigned to the OnCircle for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Signature

```python
return_value = obj.Circle
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
oMyCircle = dd.Report.ActiveSheet.Objects.Add(eReportObjectCircle,"MyCircle")
oMyCircle.ForceCircle = True
oMyCircle.Position.ByCoordinate.X1 = 10
oMyCircle.Position.ByCoordinate.X2 = 40
oMyCircle.Position.ByCoordinate.Y1 = 50
oMyCircle.Position.ByCoordinate.Y2 = 80

# This event will be raised if the mouse is moved AND the shift key pressed
dd.Report.Events.ToolTip.OnCircle = "MyToolTipEvent"
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

*Source: `ReportApi/properties/Report_property_Circle_IRepToolTipCircleContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
