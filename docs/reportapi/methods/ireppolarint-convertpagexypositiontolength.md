---
title: "IRepPolarInt.ConvertPageXYPositionToLength"
description: "Converts in a polar axis system in DIAdem REPORT a page coordinate into a radius."
---

# IRepPolarInt.ConvertPageXYPositionToLength

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ConvertPageXYPositionToLength for PolarSystem

Converts in a polar axis system in DIAdem REPORT a page coordinate into a radius.

## Signature

```python
iConvertPageXYPositionToLength = Object.ConvertPageXYPositionToLength(X, Y)
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
        oSystem = Context.AxisSystemPolar

        # Map cursor point to length and angle
        Lenght = oSystem.ConvertPageXYPositionToLength(Context.Position.X, Context.Position.Y)
        Angle  = oSystem.ConvertPageXYPositionToAngle(Context.Position.X, Context.Position.Y)

        # Build message text
        sgMessage =  "Lenght: " + VBTab + Lenght + VBCrLf + "Angle: " + VBTab + Angle
        MsgBoxDisp(sgMessage,,,,5,True)
```

---

*Source: `ReportApi/methods/Report_method_ConvertPageXYPositionToLength_IRepPolarInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
