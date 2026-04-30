---
title: "IRepD2SpecialCombAdditionalStylesInt"
description: "The 2DAdditionalStyles object provides the additional display type properties of a 2D axis system in the Special combination display mode in DIAdem REPORT."
---

# IRepD2SpecialCombAdditionalStylesInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAdditionalStyles

The 2DAdditionalStyles object provides the additional display type properties of a 2D axis system in the Special combination display mode in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyAdditionalStyles = oMyShape.Extensions.AdditionalStyles
oMyAdditionalStyles.Type = dd.e2DAdditionalStyleSpikes
oMyAdditionalStyles.Line.Color.SetPredefinedColor(dd.eColorIndexRed)
oMyAdditionalStyles.Line.Width = dd.eLineWidth0025
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2specialcombadditionalstylesint-filling/">Filling</a> | <a href="../../properties/irepd2specialcombadditionalstylesint-line/">Line</a> | <a href="../../properties/irepd2specialcombadditionalstylesint-offset/">Offset</a> | <a href="../../properties/irepd2specialcombadditionalstylesint-type/">Type</a> | <a href="../../properties/irepd2specialcombadditionalstylesint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjspecialcombinationextensionsint/">2DSpecialCombinationExtensions</a>.<a href="../../properties/irepd2shapeobjspecialcombinationextensionsint-additionalstyles/">AdditionalStyles</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2SpecialCombAdditionalStylesInt.htm`*
