---
title: "IRepToolTipSpiderContextInt"
description: "The ToolTipSpiderContext object provides information on a 2D spider axis system in DIAdem REPORT when DIAdem calls the event assigned to the OnSpider for ToolTi"
---

# IRepToolTipSpiderContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ToolTipSpiderContext

The ToolTipSpiderContext object provides information on a 2D spider axis system in DIAdem REPORT when DIAdem calls the event assigned to the OnSpider for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

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
dd.Report.Events.ToolTip.OnSpider = "MyToolTipEvent"
dd.Report.Refresh()
```

```python
def MyToolTipEvent(Context,ToolTipText):
    oSubObject = Context.SubObject
    ToolTipText = "Sheet: " + Context.Sheet.Name + VBCrLf + "-Sub object-" + VBCrLf + "Name: " + oSubObject.Name + VBCrLf + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
    ToolTipText = ToolTipText + VBCrLf + "X position: " + Context.Position.X + VBCrLf + "Y position: " + Context.Position.Y
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/ireptooltipspidercontextint-position/">Position</a> | <a href="../../properties/ireptooltipspidercontextint-sheet/">Sheet</a> | <a href="../../properties/ireptooltipspidercontextint-spider/">Spider</a> | <a href="../../properties/ireptooltipspidercontextint-subobject/">SubObject</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/ireptooltipspidercontextint-position/">Position</a> | <a href="../../properties/ireptooltipspidercontextint-sheet/">Sheet</a> | <a href="../../properties/ireptooltipspidercontextint-spider/">Spider</a> | <a href="../../properties/ireptooltipspidercontextint-subobject/">SubObject</a></p>
</div>
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepToolTipSpiderContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
