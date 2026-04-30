---
title: "IRepSpiderSubObjInt.Type"
description: "Returns the subobject type of a spider axis system in DIAdem REPORT when DIAdem calls the event assigned to the OnSpider for ToolTipEvents property. DIAdem call"
---

# IRepSpiderSubObjInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for SpiderSubObj

Returns the subobject type of a spider axis system in DIAdem REPORT when DIAdem calls the event assigned to the OnSpider for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Signature

```python
obj.Type
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

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eSpiderElementAxis` | 0 | Axis |
| `eSpiderElementAxisNumbers` | 1 | Axis scale labels |
| `eSpiderElementAxisLabel` | 2 | Show/hide |
| `eSpiderElementCurve` | 3 | Curve |
| `eSpiderElementCurveLegend` | 4 | Legend |

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepSpiderSubObjInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
