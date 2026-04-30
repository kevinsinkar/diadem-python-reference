---
title: "IRepToolTipPositionInt"
description: "The ToolTipPositionInt object returns the x-cursor and the y-cursor coordinates as page coordinates in DIAdem REPORT when DIAdem calls the event assigned to the"
---

# IRepToolTipPositionInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ToolTipPositionInt

The ToolTipPositionInt object returns the x-cursor and the y-cursor coordinates as page coordinates in DIAdem REPORT when DIAdem calls the event assigned to the OnAxisSystem2D for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object. Use the methods ConvertPageXPositionToXAxisValue and ConvertPageYPositionToYAxisValue to convert the page coordinates into coordinates of a 2D axis system.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptooltippositionint-x/">X</a> | <a href="../../properties/ireptooltippositionint-y/">Y</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptooltip2daxiscontextint/">ToolTip2DAxisContext</a>.<a href="../../properties/ireptooltip2daxiscontextint-position/">Position</a> | <a href="../ireptooltip2dtablecontextint/">ToolTip2DTableContext</a>.<a href="../../properties/ireptooltip2dtablecontextint-position/">Position</a> | <a href="../ireptooltip3daxiscontextint/">ToolTip3DAxisContext</a>.<a href="../../properties/ireptooltip3daxiscontextint-position/">Position</a> | <a href="../ireptooltip3dtablecontextint/">ToolTip3DTableContext</a>.<a href="../../properties/ireptooltip3dtablecontextint-position/">Position</a> | <a href="../ireptooltiparrowcontextint/">ToolTipArrowContext</a>.<a href="../../properties/ireptooltiparrowcontextint-position/">Position</a> | <a href="../ireptooltipcirclecontextint/">ToolTipCircleContext</a>.<a href="../../properties/ireptooltipcirclecontextint-position/">Position</a> | <a href="../ireptooltipcommentcontextint/">ToolTipCommentContext</a>.<a href="../../properties/ireptooltipcommentcontextint-position/">Position</a> | <a href="../ireptooltipformuladisplaycontextint/">ToolTipFormulaDisplayContext</a>.<a href="../../properties/ireptooltipformuladisplaycontextint-position/">Position</a> | <a href="../ireptooltipframecontextint/">ToolTipFrameContext</a>.<a href="../../properties/ireptooltipframecontextint-position/">Position</a> | <a href="../ireptooltipimagecontextint/">ToolTipImageContext</a>.<a href="../../properties/ireptooltipimagecontextint-position/">Position</a> | <a href="../ireptooltippiechartcontextint/">ToolTipPieChartContext</a>.<a href="../../properties/ireptooltippiechartcontextint-position/">Position</a> | <a href="../ireptooltippolarcontextint/">ToolTipPolarContext</a>.<a href="../../properties/ireptooltippolarcontextint-position/">Position</a> | <a href="../ireptooltipspidercontextint/">ToolTipSpiderContext</a>.<a href="../../properties/ireptooltipspidercontextint-position/">Position</a> | <a href="../ireptooltiptextcontextint/">ToolTipTextContext</a>.<a href="../../properties/ireptooltiptextcontextint-position/">Position</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepToolTipPositionInt.htm`*
