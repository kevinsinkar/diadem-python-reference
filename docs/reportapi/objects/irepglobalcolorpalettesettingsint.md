---
title: "IRepGlobalColorPaletteSettingsInt"
description: "The GlobalColorPaletteSettings object provides the properties of a global color legend in DIAdem REPORT."
---

# IRepGlobalColorPaletteSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: GlobalColorPaletteSettings

The GlobalColorPaletteSettings object provides the properties of a global color legend in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")

dd.Report.NewLayout()
oMyGlobalColorPaletteLine = dd.Report.Settings.GlobalColorPalette1.LineStyle
oMyGlobalColorPaletteLine.Width = dd.eLineWidth0100
oMyGlobalColorPaletteLine.LineType = dd.eLineTypeDashed1
oMyGlobalColorPaletteLine.Interval = 5

oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.Settings.Line.Color.ColorIndex = dd.eColorIndexGlobalColorPalette1
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepglobalcolorpalettesettingsint-colorhslfirst/">ColorHSLFirst</a> | <a href="../../properties/irepglobalcolorpalettesettingsint-colorhsllast/">ColorHSLLast</a> | <a href="../../properties/irepglobalcolorpalettesettingsint-count/">Count</a> | <a href="../../properties/irepglobalcolorpalettesettingsint-linestyle/">LineStyle</a> | <a href="../../properties/irepglobalcolorpalettesettingsint-scalemode/">ScaleMode</a> | <a href="../../properties/irepglobalcolorpalettesettingsint-scalevaluebegin/">ScaleValueBegin</a> | <a href="../../properties/irepglobalcolorpalettesettingsint-scalevalueend/">ScaleValueEnd</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsettingsint/">Settings</a>.<a href="../../properties/irepsettingsint-globalcolorpalette1/">GlobalColorPalette1</a> | <a href="../irepsettingsint/">Settings</a>.<a href="../../properties/irepsettingsint-globalcolorpalette2/">GlobalColorPalette2</a> | <a href="../irepsettingsint/">Settings</a>.<a href="../../properties/irepsettingsint-globalcolorpalette3/">GlobalColorPalette3</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepGlobalColorPaletteSettingsInt.htm`*
