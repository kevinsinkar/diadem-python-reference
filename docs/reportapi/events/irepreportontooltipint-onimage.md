---
title: "IRepReportOnToolTipInt.OnImage"
description: "Is triggered in DIAdem REPORT when you press the shift key and move the mouse over an image. The event starts the user command that you assigned to the OnImage "
---

# IRepReportOnToolTipInt.OnImage

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnImage for ToolTipEvents

Is triggered in DIAdem REPORT when you press the shift key and move the mouse over an image. The event starts the user command that you assigned to the OnImage for ToolTipEvents property. The user command receives two parameters. The first parameter corresponds to a ToolTipImageContext object and provides information about the image in DIAdem REPORT. The second parameter is a text and corresponds with the tooltip for display. Refer to Working with Events in DIAdem for further information on events in DIAdem.

## Signature

```python
obj.OnImage
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
oMyImage = dd.Report.ActiveSheet.Objects.Add(eReportObjectImage, "MyImage")
oMyPos = oMyImage.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 60
oMyPos.Y1 = 20
oMyPos.Y2 = 60
oMyImage.FileName = MediaLibrPath + "Example1.png"
oMyImage.BackgroundColor.SetPredefinedColor(eColorIndexNone)

# This event will be raised if the mouse is moved AND the shift key pressed
dd.AddUserCommandToEvent("dd.Report.Events.ToolTip.OnImage", "MyToolTipEvent")
dd.Report.Refresh()
```

```python
def MyToolTipEvent(Context,ToolTipText):
    oSubObject = Context.SubObject
    ToolTipText = "Sheet: " + Context.Sheet.Name + "\r\n" + "Sub object" + "\r\n" + "Name: " + oSubObject.Name + "\r\n" + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
    ToolTipText = ToolTipText + "\r\n" + "X position: " + Context.Position.X + "\r\n" + "Y position: " + Context.Position.Y
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/events/Report_event_OnImage_IRepReportOnToolTipInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
