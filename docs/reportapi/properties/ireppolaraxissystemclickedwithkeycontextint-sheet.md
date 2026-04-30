---
title: "IRepPolarAxisSystemClickedWithKeyContextInt.Sheet"
description: "Specifies the worksheet in DIAdem REPORT when you call the event you assigned to the OnAxisSystemPolar for ClickedWithKeyEvents property. DIAdem calls this even"
---

# IRepPolarAxisSystemClickedWithKeyContextInt.Sheet

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Sheet for PolarAxisSystemClickedWithKeyContext

Specifies the worksheet in DIAdem REPORT when you call the event you assigned to the OnAxisSystemPolar for ClickedWithKeyEvents property. DIAdem calls this event when you click a polar axis system while pressing a key. For this event DIAdem does not support keys such as <Alt>, <Ctrl>, and <Shift>. Use the methods ConvertPageXPositionToXAxisValue , and ConvertPageYPositionToYAxisValue to convert the page coordinates of a polar axis system.

## Signature

```python
return_value = obj.Sheet
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note  </strong>To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
DataFileLoad(DataReadPath + "Report_Data.tdm","TDM","")

oMyPolarSystem = dd.Report.ActiveSheet.Objects.Add(eReportObjectPolarSystem, "MyPolarSystem")
oMyPos = oMyPolarSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyPolarCurve = oMyPolarSystem.CurvesPolar.Add(ePolarShapeLine, "MyPolarCurve")
oMyPolarCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyPolarCurve.Shape.YChannel.Reference = "[5]/[4]"

# This event will be raised if you click a 2D axis system while you press a keyboard key
dd.Report.Events.ClickedWithKey.OnAxisSystemPolar = "MyClickEvent"
dd.Report.Refresh()
```

```python
def MyClickEvent(Context):
    Context.DoProceed = False'True
    # Check the key
    if Chr(Context.KeyValue) = "C" or Chr(Context.KeyValue) = "c":
        Context.DoProceed = True
        if Context.SubObject.Type = ePolarElementMain:
            oSystem = Context.AxisSystemPolar

            # Map cursor point to length and angle
            Lenght = oSystem.ConvertPageXYPositionToLength(Context.Position.X, Context.Position.Y)
            Angle  = oSystem.ConvertPageXYPositionToAngle(Context.Position.X, Context.Position.Y)

            # Build message text
            sgMessage =  "Lenght: " + VBTab + Lenght + VBCrLf + "Angle: " + VBTab + Angle
        else:
            oSubObject = Context.SubObject
            sgMessage = "Sheet: " + Context.Sheet.Name + VBCrLf + "Sub object" + VBCrLf + "Name: " + oSubObject.Name + VBCrLf + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
        MsgBoxDisp(sgMessage,,,,5,True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Sheet_IRepPolarAxisSystemClickedWithKeyContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
