---
title: "IRepImageInt"
description: "The Image object provides the properties of a graphic in DIAdem REPORT."
---

# IRepImageInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Image

The Image object provides the properties of a graphic in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyImage = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectImage, "MyImage")
oMyPos = oMyImage.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 60
oMyPos.Y1 = 20
oMyPos.Y2 = 60
oMyImage.FileName = dd.MediaLibrPath + "Example1.png"
oMyImage.BackgroundColor.SetPredefinedColor(dd.eColorIndexNone)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepimageint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/irepimageint-embedded/">Embedded</a> | <a href="../../properties/irepimageint-filename/">FileName</a> | <a href="../../properties/irepimageint-fullpath/">FullPath</a> | <a href="../../properties/irepimageint-index/">Index</a> | <a href="../../properties/irepimageint-isselected/">IsSelected</a> | <a href="../../properties/irepimageint-name/">Name</a> | <a href="../../properties/irepimageint-objecttype/">ObjectType</a> | <a href="../../properties/irepimageint-originalratio/">OriginalRatio</a> | <a href="../../properties/irepimageint-position/">Position</a> | <a href="../../properties/irepimageint-relativeposition/">RelativePosition</a> | <a href="../../properties/irepimageint-tagstored/">TagStored</a> | <a href="../../properties/irepimageint-tagtemporary/">TagTemporary</a> | <a href="../../properties/irepimageint-useoriginalratio/">UseOriginalRatio</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepimageint-exporttoimage/">ExportToImage</a> | <a href="../../methods/irepimageint-select/">Select</a> | <a href="../../methods/irepimageint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptooltipimagecontextint/">ToolTipImageContext</a>.<a href="../../properties/ireptooltipimagecontextint-image/">Image</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepImageInt.htm`*
