---
title: "IRepFreeFrameInt"
description: "The Frame object provides a rectangle in DIAdem REPORT."
---

# IRepFreeFrameInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Frame

The Frame object provides a rectangle in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyFrame = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFrame,"MyFrame")
oMyFrame.ForceSquare = True
oMyBackgroundColor = oMyFrame.BackgroundColor
oMyBackgroundColor.SetPredefinedColor(dd.eColorIndexRed )
oMyBackgroundColor.Transparency = 50

oMyFrame.Position.ByCoordinate.X1 = 10
oMyFrame.Position.ByCoordinate.X2 = 40
oMyFrame.Position.ByCoordinate.Y1 = 50
oMyFrame.Position.ByCoordinate.Y2 = 80

oMyBorderLineColor = oMyFrame.BorderLine.Color
oMyBorderLineColor.SetPredefinedColor(dd.eColorIndexGreen)
oMyFrame.BorderLine.LineType = dd.eLineTypeDotted
oMyFrame.BorderLine.Width = dd.eLineWidth0140

oMyShadowColor = oMyFrame.Shadow.Color
oMyShadowColor.SetPredefinedColor(dd.eColorIndexBlue)
oMyFrame.Shadow.Direction = dd.eShadowDirectionLeftBottom
oMyFrame.Shadow.OffsetX = 1
oMyFrame.Shadow.OffsetY = 2

oMyFrame.ExportToImage("D:\\MyFrame",dd.eImageExportTypePNG)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepfreeframeint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/irepfreeframeint-borderline/">BorderLine</a> | <a href="../../properties/irepfreeframeint-forcesquare/">ForceSquare</a> | <a href="../../properties/irepfreeframeint-index/">Index</a> | <a href="../../properties/irepfreeframeint-isselected/">IsSelected</a> | <a href="../../properties/irepfreeframeint-name/">Name</a> | <a href="../../properties/irepfreeframeint-objecttype/">ObjectType</a> | <a href="../../properties/irepfreeframeint-position/">Position</a> | <a href="../../properties/irepfreeframeint-shadow/">Shadow</a> | <a href="../../properties/irepfreeframeint-tagstored/">TagStored</a> | <a href="../../properties/irepfreeframeint-tagtemporary/">TagTemporary</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepfreeframeint-exporttoimage/">ExportToImage</a> | <a href="../../methods/irepfreeframeint-select/">Select</a> | <a href="../../methods/irepfreeframeint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptooltipframecontextint/">ToolTipFrameContext</a>.<a href="../../properties/ireptooltipframecontextint-frame/">Frame</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepFreeFrameInt.htm`*
