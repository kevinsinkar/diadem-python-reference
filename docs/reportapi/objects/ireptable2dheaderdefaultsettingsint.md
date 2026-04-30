---
title: "IRepTable2DHeaderDefaultSettingsInt"
description: "The 2DTableHeaderDefaultSettings object provides the global properties of the headers and footers in a 2D table in DIAdem REPORT."
---

# IRepTable2DHeaderDefaultSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableHeaderFooterDefaultSettings

The 2DTableHeaderDefaultSettings object provides the global properties of the headers and footers in a 2D table in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyHeaderSettings = oMy2DTable.Settings.Header
oMyHeaderSettings.Height = 20
oMyHeaderSettings.Title1 = "@@ChnName(CurrChnNo)@@"
oMyHeaderSettings.Title2 = "@@ChnDim(CurrChnNo)@@"
oMyHeaderSettings.Font.Size = 4
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dheaderdefaultsettingsint-alignment/">Alignment</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-angle/">Angle</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-font/">Font</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-height/">Height</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-showgridlines/">ShowGridLines</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-showonlyonlastsubsheet/">ShowOnlyOnLastSubSheet</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-title1/">Title1</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-title2/">Title2</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-title3/">Title3</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-titledefinition1/">TitleDefinition1</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-titledefinition2/">TitleDefinition2</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-titledefinition3/">TitleDefinition3</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-useautofontsize/">UseAutoFontSize</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-usetextclipping/">UseTextClipping</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-usewordwrap/">UseWordWrap</a> | <a href="../../properties/ireptable2dheaderdefaultsettingsint-visible/">Visible</a> </p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable2dsettingsint/">2DTableSettings</a>.<a href="../../properties/ireptable2dsettingsint-footer/">Footer</a> | <a href="../ireptable2dsettingsint/">2DTableSettings</a>.<a href="../../properties/ireptable2dsettingsint-header/">Header</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DHeaderDefaultSettingsInt.htm`*
