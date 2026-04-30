---
title: "IRepD2AxisSubObjInt.Type"
description: "Returns a subobject type of a 2D axis system in DIAdem REPORT when DIAdem calls the event assigned to the OnAxisSystem2D for ToolTipEvents property. DIAdem call"
---

# IRepD2AxisSubObjInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for D2SubObj

Returns a subobject type of a 2D axis system in DIAdem REPORT when DIAdem calls the event assigned to the OnAxisSystem2D for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Signature

```python
obj.Type
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
dd.Data.Root.Clear()
DataFileLoad(DataReadPath + "Report_Data.tdm","TDM","")

oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(e2DShapeLine, "My2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[6]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[6]/[4]"

# This event will be raised if the mouse is moved AND the shift key pressed
dd.Report.Events.ToolTip.OnAxisSystem2D = "MyToolTipEvent"
dd.Report.Refresh()
```

```python
def MyToolTipEvent(Context,ToolTipText):
    if Context.SubObject.Type = e2DElementCurve:
        oSystem = Context.AxisSystem2D

        # Find curve, x and y-axis to convert the coordinate to value
        oXAxis = oSystem.XAxis
        oCurve = oSystem.Curves2D.Item(Context.SubObject.Name)
        oYAxis = oSystem.YAxisList.Item(oCurve.YAxisReference)

        # Convert cursor position to axis coordinates
        x = oXAxis.ConvertPageXPositionToXAxisValue(Context.Position.X)
        y = oYAxis.ConvertPageYPositionToYAxisValue(Context.Position.Y)

        # Find nearest point on curve
        oPoint = oCurve.FindNearestValue(x,y)

        # Build tooltip text
        ToolTipText =  ToolTipText + VBCrLf + "Point (" + oPoint.Index + ")" + VBCrLf + "X = " + RTT(oPoint.X) + VBCrLf + "Y = " + Str(oPoint.Y)
        # Add assignment value which categorizes the value as a string value based on value limits
        oChannel = dd.Data.GetChannel(oCurve.Shape.YChannel.Reference)
        ToolTipText =  ToolTipText + VBCrLf + "Assignment value: " + oChannel.Values(oPoint.Index)
    else:
        oSubObject = Context.SubObject
        ToolTipText = "Sheet: " + Context.Sheet.Name + VBCrLf + "Sub object" + VBCrLf + "Name: " + oSubObject.Name + VBCrLf + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepD2AxisSubObjInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
