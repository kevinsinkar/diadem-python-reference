---
title: "IRepCircleInt"
description: "The Circle object provides a circle in DIAdem REPORT."
---

# IRepCircleInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Circle

The Circle object provides a circle in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyCircle = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")

oMyCircle.ForceCircle = True

oMyBackgroundColor = oMyCircle.BackgroundColor
oMyBackgroundColor.SetPredefinedColor(dd.eColorIndexRed )
oMyBackgroundColor.Transparency = 50

oMyCircle.Position.ByCoordinate.X1 = 10
oMyCircle.Position.ByCoordinate.X2 = 40
oMyCircle.Position.ByCoordinate.Y1 = 50
oMyCircle.Position.ByCoordinate.Y2 = 80

oMyBorderLineColor = oMyCircle.BorderLine.Color
oMyBorderLineColor.SetPredefinedColor(dd.eColorIndexGreen)
oMyCircle.BorderLine.LineType = dd.eLineTypeDotted
oMyCircle.BorderLine.Width = dd.eLineWidth0140

dd.Report.Settings.ImageExport.PNG.BitsPerPixel = dd.ePNGBitsPerPixelRGB24
dd.Report.Settings.ImageExport.PNG.Height = 300
dd.Report.Settings.ImageExport.PNG.UseRatio = True
oMyCircle.ExportToImage(dd.LayoutWritePath + "MyCircle", dd.eImageExportTypePNG)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcircleint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/irepcircleint-borderline/">BorderLine</a> | <a href="../../properties/irepcircleint-forcecircle/">ForceCircle</a> | <a href="../../properties/irepcircleint-index/">Index</a> | <a href="../../properties/irepcircleint-isselected/">IsSelected</a> | <a href="../../properties/irepcircleint-name/">Name</a> | <a href="../../properties/irepcircleint-objecttype/">ObjectType</a> | <a href="../../properties/irepcircleint-position/">Position</a> | <a href="../../properties/irepcircleint-tagstored/">TagStored</a> | <a href="../../properties/irepcircleint-tagtemporary/">TagTemporary</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepcircleint-exporttoimage/">ExportToImage</a> | <a href="../../methods/irepcircleint-select/">Select</a> | <a href="../../methods/irepcircleint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptooltipcirclecontextint/">ToolTipCircleContext</a>.<a href="../../properties/ireptooltipcirclecontextint-circle/">Circle</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCircleInt.htm`*
