---
title: "IRepTextSimpleInt"
description: "The Text object provides a text in DIAdem REPORT."
---

# IRepTextSimpleInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Text

The Text object provides a text in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "@@CurrDate@@"
oMyText.Font.Color.SetPredefinedColor(dd.ePredefinedColorBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptextsimpleint-font/">Font</a> | <a href="../../properties/ireptextsimpleint-index/">Index</a> | <a href="../../properties/ireptextsimpleint-isselected/">IsSelected</a> | <a href="../../properties/ireptextsimpleint-name/">Name</a> | <a href="../../properties/ireptextsimpleint-objecttype/">ObjectType</a> | <a href="../../properties/ireptextsimpleint-positionxy/">PositionXY</a> | <a href="../../properties/ireptextsimpleint-tagstored/">TagStored</a> | <a href="../../properties/ireptextsimpleint-tagtemporary/">TagTemporary</a> | <a href="../../properties/ireptextsimpleint-text/">Text</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireptextsimpleint-exporttoimage/">ExportToImage</a> | <a href="../../methods/ireptextsimpleint-select/">Select</a> | <a href="../../methods/ireptextsimpleint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptextsimpledropcontextint/">TextDropContext</a>.<a href="../../properties/ireptextsimpledropcontextint-text/">Text</a> | <a href="../ireptooltiptextcontextint/">ToolTipTextContext</a>.<a href="../../properties/ireptooltiptextcontextint-text/">Text</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTextSimpleInt.htm`*
