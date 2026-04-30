---
title: "IRepSolidLineInt"
description: "The SolidLine object provides the properties of a line in DIAdem REPORT."
---

# IRepSolidLineInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SolidLine

The SolidLine object provides the properties of a line in DIAdem REPORT.

## Python example

```python
oMyBorderLine = dd.Report.Settings.Page.BorderLine
oMyBorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyBorderLine.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsolidlineint-color/">Color</a> | <a href="../../properties/irepsolidlineint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axissettingsint/">2DAxisSettings</a>.<a href="../../properties/irepd2axissettingsint-axisline/">AxisLine</a> | <a href="../irepd2shapeobjcoordinatesettingsint/">2DCoordinateSettings</a>.<a href="../../properties/irepd2shapeobjcoordinatesettingsint-markerborderline/">MarkerBorderLine</a> | <a href="../irepd3axisxint/">3DAxisX</a>.<a href="../../properties/irepd3axisxint-line/">Line</a> | <a href="../irepd3axisyint/">3DAxisY</a>.<a href="../../properties/irepd3axisyint-line/">Line</a> | <a href="../irepd3axiszint/">3DAxisZ</a>.<a href="../../properties/irepd3axiszint-line/">Line</a> | <a href="../ireppagedefaultsettingsint/">PageDefaultSettings</a>.<a href="../../properties/ireppagedefaultsettingsint-borderline/">BorderLine</a> | <a href="../irepspideraxisint/">SpiderAxis</a>.<a href="../../properties/irepspideraxisint-line/">Line</a> | <a href="../irepspidergridint/">SpiderGrid</a>.<a href="../../properties/irepspidergridint-line/">Line</a> | <a href="../irepspidergridint/">SpiderGrid</a>.<a href="../../properties/irepspidergridint-minitickline/">MiniTickLine</a> | <a href="../irepspidersettingsint/">SpiderSettings</a>.<a href="../../properties/irepspidersettingsint-borderline/">BorderLine</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSolidLineInt.htm`*
