---
title: "IRepPolarSubObjInt.Type"
description: "Returns the subobject type of a polar axis system in DIAdem REPORT when DIAdem calls the event assigned to the OnPolarSystem for ToolTipEvents property. DIAdem "
---

# IRepPolarSubObjInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for PolarSubObj

Returns the subobject type of a polar axis system in DIAdem REPORT when DIAdem calls the event assigned to the OnPolarSystem for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Signature

```python
obj.Type
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePolarElementRadialAxis` | 0 | Radial axis |
| `ePolarElementRadialAxisNumbers` | 1 | Radial axis scale |
| `ePolarElementSectorNumbers` | 2 | Circle scale |
| `ePolarElementRadialAxisLabel` | 3 | Radial axis label |
| `ePolarElementCurve` | 4 | Curve |
| `ePolarElementCurveLegend` | 5 | Legend |

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

*Source: `ReportApi/properties/Report_property_Type_IRepPolarSubObjInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
