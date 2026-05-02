---
title: "IRepReportOnToolTipInt"
description: "The ToolTipEvents object provides the events when you press the shift key and move the mouse over a REPORT object."
---

# IRepReportOnToolTipInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ToolTipEvents

The ToolTipEvents object provides the events when you press the shift key and move the mouse over a REPORT object.

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
    if Context.SubObject.Type == e2DElementCurve:
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
        ToolTipText =  ToolTipText + "\r\n" + "Point (" + oPoint.Index + ")" + "\r\n" + "X = " + RTT(oPoint.X) + "\r\n" + "Y = " + Str(oPoint.Y)
        # Add assignment value which categorizes the value as a string value based on value limits
        oChannel = dd.Data.GetChannel(oCurve.Shape.YChannel.Reference)
        ToolTipText =  ToolTipText + "\r\n" + "Assignment value: " + oChannel.Values(oPoint.Index)
    else:
        oSubObject = Context.SubObject
        ToolTipText = "Sheet: " + Context.Sheet.Name + "\r\n" + "Sub object" + "\r\n" + "Name: " + oSubObject.Name + "\r\n" + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepreportontooltipint-onarrow/">OnArrow</a> | <a href="../../properties/irepreportontooltipint-onaxissystem2d/">OnAxisSystem2D</a> | <a href="../../properties/irepreportontooltipint-onaxissystem3d/">OnAxisSystem3D</a> | <a href="../../properties/irepreportontooltipint-oncircle/">OnCircle</a> | <a href="../../properties/irepreportontooltipint-oncomment/">OnComment</a> | <a href="../../properties/irepreportontooltipint-onformuladisplay/">OnFormulaDisplay</a> | <a href="../../properties/irepreportontooltipint-onframe/">OnFrame</a> | <a href="../../properties/irepreportontooltipint-onimage/">OnImage</a> | <a href="../../properties/irepreportontooltipint-onpiechart/">OnPieChart</a> | <a href="../../properties/irepreportontooltipint-onpolarsystem/">OnPolarSystem</a> | <a href="../../properties/irepreportontooltipint-onspider/">OnSpider</a> | <a href="../../properties/irepreportontooltipint-ontable2d/">OnTable2D</a> | <a href="../../properties/irepreportontooltipint-ontable3d/">OnTable3D</a> | <a href="../../properties/irepreportontooltipint-ontext/">OnText</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepreporteventsint/">Events</a>.<a href="../../properties/irepreporteventsint-tooltip/">ToolTip</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepReportOnToolTipInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
