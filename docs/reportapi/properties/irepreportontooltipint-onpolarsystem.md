---
title: "IRepReportOnToolTipInt.OnPolarSystem"
description: "Specifies the user command which DIAdem REPORT executes when you press the shift key and move the mouse over a polar axis system. The user command receives two "
---

# IRepReportOnToolTipInt.OnPolarSystem

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnPolarSystem for ToolTipEvents

Specifies the user command which DIAdem REPORT executes when you press the shift key and move the mouse over a polar axis system. The user command receives two parameters. The first parameter corresponds to a ToolTipPolarContext object and provides information about the polar axis system in DIAdem REPORT. The second parameter is a text and corresponds with the tooltip for display.

## Signature

```python
obj.OnPolarSystem
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
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObjectPolarSystem,"MyPolarSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(ePolarShapeLine, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.Line.Color.SetPredefinedColor(eColorIndexBlue)

# This event will be raised if the mouse is moved AND the shift key pressed
dd.Report.Events.ToolTip.OnPolarSystem = "MyToolTipEvent"
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

*Source: `ReportApi/properties/Report_property_OnPolarSystem_IRepReportOnToolTipInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
