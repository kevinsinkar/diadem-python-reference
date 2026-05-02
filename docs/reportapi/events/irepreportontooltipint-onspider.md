---
title: "IRepReportOnToolTipInt.OnSpider"
description: "Is triggered in DIAdem REPORT when you press the shift key and move the mouse over a spider axis system. The event starts the user command that you assigned to "
---

# IRepReportOnToolTipInt.OnSpider

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnSpider for ToolTipEvents

Is triggered in DIAdem REPORT when you press the shift key and move the mouse over a spider axis system. The event starts the user command that you assigned to the OnSpider for ToolTipEvents property. The user command receives two parameters. The first parameter corresponds to a ToolTipSpiderContext object and provides information about the spider axis system in DIAdem REPORT. The second parameter is a text and is the same as displayed on the tooltip. Refer to Working with Events in DIAdem for more information on events in DIAdem.

## Signature

```python
obj.OnTable2D
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note</strong>  To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
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
DataFileLoad("Example.tdm","TDM","")
oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObjectSpider, "MySpiderAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyAxisSystem.CurvesSpider.Add(eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

# This event will be raised if the mouse is moved AND the shift key pressed
AddUserCommandToEvent("dd.Report.Events.ToolTip.OnSpider", "MyToolTipEvent" )
dd.Report.Refresh()
```

```python
def MyToolTipEvent(Context,ToolTipText):
    oSubObject = Context.SubObject
    ToolTipText = "Sheet: " + Context.Sheet.Name + "\r\n" + "-Sub object-" + "\r\n" + "Name: " + oSubObject.Name + "\r\n" + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
    ToolTipText = ToolTipText + "\r\n" + "X position: " + Context.Position.X + "\r\n" + "Y position: " + Context.Position.Y
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/events/Report_event_OnSpider_IRepReportOnToolTipInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
