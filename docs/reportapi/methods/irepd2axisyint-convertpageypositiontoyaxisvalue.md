---
title: "IRepD2AxisYInt.ConvertPageYPositionToYAxisValue"
description: "Converts a y-page coordinate into a y-axis coordinate in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisYInt.ConvertPageYPositionToYAxisValue

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ConvertPageYPositionToYAxisValue for 2DAxisY

Converts a y-page coordinate into a y-axis coordinate in a 2D axis system in DIAdem REPORT.

## Signature

```python
iConvertPageYPositionToYAxisValue = Object.ConvertPageYPositionToYAxisValue(Value)
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")

oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "My2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[6]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[6]/[4]"

#This event will be raised if the mouse is moved AND the shift key pressed
dd.Report.Events.ToolTip.OnAxisSystem2D = "MyToolTipEvent"
dd.Report.Refresh()
```

```python
def MyToolTipEvent(Context,ToolTipText):
    if Context.SubObject.Type == dd.e2DElementCurve :
        oSystem = Context.AxisSystem2D

#Find curve, x and y-axis to convert the coordinate to value
        oXAxis = oSystem.XAxis
        oCurve = oSystem.Curves2D.Item(Context.SubObject.Name)
        oYAxis = oSystem.YAxisList.Item(oCurve.YAxisReference)

#Convert cursor position to axis coordinates
        x = oXAxis.ConvertPageXPositionToXAxisValue(Context.Position.X)
        y = oYAxis.ConvertPageYPositionToYAxisValue(Context.Position.Y)

#Find nearest point on curve
        oPoint = oCurve.FindNearestValue(x,y)

#Build tooltip text
        ToolTipText =  ToolTipText + "\r\n" + "Point (" + oPoint.Index + ")" + "\r\n" + "X = " + dd.RTT(oPoint.X) + "\r\n" + "Y = " + dd.Str(oPoint.Y)
#Add assignment value which categorizes the value as a string value based on value limits
        oChannel = dd.Data.GetChannel(oCurve.Shape.YChannel.Reference)
        ToolTipText =  ToolTipText + "\r\n" + "Assignment value: " + oChannel.Values(oPoint.Index)
    else:
        oSubObject = Context.SubObject
        ToolTipText = "Sheet: " + Context.Sheet.Name + "\r\n" + "Sub object" + "\r\n" + "Name: " +  oSubObject.Name + "\r\n" + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ConvertPageYPositionToYAxisValue_IRepD2AxisYInt.htm`*
