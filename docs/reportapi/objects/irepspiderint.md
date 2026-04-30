---
title: "IRepSpiderInt"
description: "The Spider object provides a spider axis system in DIAdem REPORT."
---

# IRepSpiderInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Spider

The Spider object provides a spider axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepspiderint-categorysettings/">CategorySettings</a> | <a href="../../properties/irepspiderint-curvelegend/">CurveLegend</a> | <a href="../../properties/irepspiderint-curvesspider/">CurvesSpider</a> | <a href="../../properties/irepspiderint-index/">Index</a> | <a href="#" data-unresolved="1">IsSelected</a> | <a href="../../properties/irepspiderint-name/">Name</a> | <a href="../../properties/irepspiderint-objecttype/">ObjectType</a> | <a href="../../properties/irepspiderint-position/">Position</a> | <a href="#" data-unresolved="1">SelectedElements</a> | <a href="../../properties/irepspiderint-settings/">Settings</a> | <a href="../../properties/irepspiderint-tagstored/">TagStored</a> | <a href="../../properties/irepspiderint-tagtemporary/">TagTemporary</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepspiderint-exporttoimage/">ExportToImage</a> | <a href="../../methods/irepspiderint-select/">Select</a> | <a href="../../methods/irepspiderint-showpropertiesdlg/">ShowPropertiesDlg</a> | <a href="../../methods/irepspiderint-updatescaling/">UpdateScaling</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptooltipspidercontextint/">ToolTipSpiderContext</a>.<a href="../../properties/ireptooltipspidercontextint-spider/">Spider</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderInt.htm`*
