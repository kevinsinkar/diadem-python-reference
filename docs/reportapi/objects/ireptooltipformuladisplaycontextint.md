---
title: "IRepToolTipFormulaDisplayContextInt"
description: "The ToolTipFormulaDisplayContext object provides information about a formula in DIAdem REPORT when DIAdem calls the event assigned to the OnFormulaDisplay for T"
---

# IRepToolTipFormulaDisplayContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ToolTipFormulaDisplayContext

The ToolTipFormulaDisplayContext object provides information about a formula in DIAdem REPORT when DIAdem calls the event assigned to the OnFormulaDisplay for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.NewLayout
oMyFormula = dd.Report.ActiveSheet.Objects.Add(eReportObjectFormulaDisplay ,"MyFormular")
oMyPosFormula = oMyFormula.Position.ByCoordinate
oMyFormula.Text = "a^2+b^2=c^2"
oMyPosFormula.X1 = 20
oMyPosFormula.X2 = 40
oMyPosFormula.Y1 = 20
oMyPosFormula.Y2 = 35

# This event will be raised if the mouse is moved AND the shift key pressed
dd.Report.Events.ToolTip.OnFormulaDisplay = "MyToolTipEvent"
dd.Report.Refresh()
```

```python
def MyToolTipEvent(Context,ToolTipText):
    oSubObject = Context.SubObject
    ToolTipText = "Sheet: " + Context.Sheet.Name + "\r\n" + "Sub object" + "\r\n" + "Name: " + oSubObject.Name + "\r\n" + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
    ToolTipText = ToolTipText + "\r\n" + "X position: " + Context.Position.X + "\r\n" + "Y position: " + Context.Position.Y
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptooltipformuladisplaycontextint-formuladisplay/">FormulaDisplay</a> | <a href="../../properties/ireptooltipformuladisplaycontextint-position/">Position</a> | <a href="../../properties/ireptooltipformuladisplaycontextint-sheet/">Sheet</a> | <a href="../../properties/ireptooltipformuladisplaycontextint-subobject/">SubObject</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepToolTipFormulaDisplayContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
