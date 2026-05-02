---
title: "IRepReportOnToolTipInt.OnText"
description: "Is triggered in DIAdem REPORT when you press the shift key and move the mouse over a text. The event starts the user command that you assigned to the OnText for"
---

# IRepReportOnToolTipInt.OnText

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnText for ToolTipEvents

Is triggered in DIAdem REPORT when you press the shift key and move the mouse over a text. The event starts the user command that you assigned to the OnText for ToolTipEvents property. The first parameter corresponds to a ToolTipTextContext object and provides information about the comment in DIAdem REPORT. The second parameter is a text and corresponds with the tooltip for display. Refer to Working with Events in DIAdem for further information on events in DIAdem.

## Signature

```python
obj.OnText
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
oMyText = dd.Report.ActiveSheet.Objects.Add(eReportObjectText,"MyText")
oMyText.Text = "@@CurrDate@@"
oMyText.Font.Color.SetPredefinedColor(ePredefinedColorBlue)

# This event will be raised if the mouse is moved AND the shift key pressed
AddUserCommandToEvent("dd.Report.Events.ToolTip.OnText", "MyToolTipEvent")
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

*Source: `ReportApi/events/Report_event_OnText_IRepReportOnToolTipInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
