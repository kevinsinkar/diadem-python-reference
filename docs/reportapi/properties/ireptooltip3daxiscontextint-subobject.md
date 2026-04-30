---
title: "IRepToolTip3DAxisContextInt.SubObject"
description: "Returns a subobject type of a 3D axis system in DIAdem REPORT when DIAdem calls the event assigned to the OnAxisSystem3D for ToolTipEvents property. DIAdem call"
---

# IRepToolTip3DAxisContextInt.SubObject

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SubObject for ToolTip3DAxisContext

Returns a subobject type of a 3D axis system in DIAdem REPORT when DIAdem calls the event assigned to the OnAxisSystem3D for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

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
dd.Report.Events.ToolTip.OnAxisSystem3D = "MyToolTipEvent"
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

*Source: `ReportApi/properties/Report_property_SubObject_IRepToolTip3DAxisContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
