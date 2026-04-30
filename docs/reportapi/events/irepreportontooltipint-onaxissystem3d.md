---
title: "IRepReportOnToolTipInt.OnAxisSystem3D"
description: "Is triggered in DIAdem REPORT when you press the shift key and move the mouse over a 3D axis system. The event starts the user command that you assigned to the "
---

# IRepReportOnToolTipInt.OnAxisSystem3D

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnAxisSystem3D for ToolTipEvents

Is triggered in DIAdem REPORT when you press the shift key and move the mouse over a 3D axis system. The event starts the user command that you assigned to the OnAxisSystem3D for ToolTipEvents property. The user command receives two parameters. The first parameter corresponds to a ToolTip3DAxisContext object and provides information about the 3D axis system in DIAdem REPORT. The second parameter is a text and corresponds with the tooltip for display. Refer to Working with Events in DIAdem for further information on events in DIAdem.

## Signature

```python
obj.OnAxisSystem3D
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
dd.Data.Root.Clear()
DataFileLoad(DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObject3DAxisSystem,"My3DAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(e3DShapeSurface, "MyNew3DCurve")
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMy3DCurve.Shape.DataStructure = e3DDataStructureMatrix

# This event will be raised if the mouse is moved AND the shift key pressed
AddUserCommandToEvent("dd.Report.Events.ToolTip.OnAxisSystem3D", "MyToolTipEvent")
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

*Source: `ReportApi/events/Report_event_OnAxisSystem3D_IRepReportOnToolTipInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
