---
title: "IRepArrowInt"
description: "The Arrow object provides a line or an arrow in DIAdem REPORT."
---

# IRepArrowInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Arrow

The Arrow object provides a line or an arrow in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyArrow = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectArrow,"MyArrow")

oMyArrow.ArrowHeadAtBegin = dd.eArrowHeadPoint
oMyArrow.ArrowHeadAtEnd = dd.eArrowHeadStandardArrow

oMyArrowPosition = oMyArrow.Position.ByCoordinate
oMyArrowPosition.X1 = 10
oMyArrowPosition.X2 = 40
oMyArrowPosition.Y1 = 30
oMyArrowPosition.Y2 = 90

oMyArrowLine = oMyArrow.Line
oMyArrowLine.LineType = dd.eLineTypeDotted
oMyArrowLine.Width = dd.eLineWidth0200

oMyArrowLineColor = oMyArrowLine.Color
oMyArrowLineColor.SetPredefinedColor(dd.eColorIndexGreen)

oMyArrow.ExportToImage(dd.LayoutWritePath + "MyNewArrow", dd.eImageExportTypePNG)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireparrowint-arrowheadatbegin/">ArrowHeadAtBegin</a> | <a href="../../properties/ireparrowint-arrowheadatend/">ArrowHeadAtEnd</a> | <a href="../../properties/ireparrowint-index/">Index</a> | <a href="../../properties/ireparrowint-isselected/">IsSelected</a> | <a href="../../properties/ireparrowint-line/">Line</a> | <a href="../../properties/ireparrowint-name/">Name</a> | <a href="../../properties/ireparrowint-objecttype/">ObjectType</a> | <a href="../../properties/ireparrowint-position/">Position</a> | <a href="../../properties/ireparrowint-tagstored/">TagStored</a> | <a href="../../properties/ireparrowint-tagtemporary/">TagTemporary</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireparrowint-exporttoimage/">ExportToImage</a> | <a href="../../methods/ireparrowint-select/">Select</a> | <a href="../../methods/ireparrowint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptooltiparrowcontextint/">ToolTipArrowContext</a>.<a href="../../properties/ireptooltiparrowcontextint-arrow/">Arrow</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepArrowInt.htm`*
