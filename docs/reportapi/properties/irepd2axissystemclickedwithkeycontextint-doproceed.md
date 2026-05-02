---
title: "IRepD2AxisSystemClickedWithKeyContextInt.DoProceed"
description: "Specifies whether DIAdem also transfers the D2AxisSystemClickedWithKeyContext object to the following events. If the value is TRUE , DIAdem also transfers the D"
---

# IRepD2AxisSystemClickedWithKeyContextInt.DoProceed

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DoProceed for D2AxisSystemClickedWithKeyContext

Specifies whether DIAdem also transfers the D2AxisSystemClickedWithKeyContext object to the following events. If the value is TRUE , DIAdem also transfers the D2AxisSystemClickedWithKeyContext object to the following events.

## Signature

```python
obj.DoProceed
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

# This event will be raised if you click a 2D axis system while you press a keyboard key
dd.Report.Events.ClickedWithKey.OnAxisSystem2D = "MyClickEvent"
dd.Report.Refresh()
```

```python
def MyClickEvent(Context):
    Context.DoProceed = False  # True
    # Check the key
    if Chr(Context.KeyValue) == "C" or Chr(Context.KeyValue) == "c":
        Context.DoProceed = True
        if Context.SubObject.Type == e2DElementCurve:
            oSystem = Context.AxisSystem2D

            # Convert cursor position to axis coordinates
            oXAxis = oSystem.XAxis
            oCurve = oSystem.Curves2D.Item(Context.SubObject.Name)
            oYAxis = oSystem.YAxisList.Item(oCurve.YAxisReference)

            # Map Cursor point to Axis Values
            x = oXAxis.ConvertPageXPositionToXAxisValue(Context.Position.X)
            y = oYAxis.ConvertPageYPositionToYAxisValue(Context.Position.Y)

            # Find nearest point on curve
            oPoint = oCurve.FindNearestValue(x,y)

            # Build message text
            sgMessage =  "Point (" + oPoint.Index + ")" + "\r\n" + "X = " + RTT(oPoint.X) + "\r\n" + "Y = " + Str(oPoint.Y)
            oChannel = dd.Data.GetChannel(oCurve.Shape.YChannel.Reference)
            sgMessage =  sgMessage + "\r\n" + "Assignment value: " + oChannel.Values(oPoint.Index)
        else:
            oSubObject = Context.SubObject
            sgMessage = "Sheet: " + Context.Sheet.Name + "\r\n" + "Sub object" + "\r\n" + "Name: " + oSubObject.Name + "\r\n" + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
        MsgBoxDisp(sgMessage, None, None, None,5,True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DoProceed_IRepD2AxisSystemClickedWithKeyContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
