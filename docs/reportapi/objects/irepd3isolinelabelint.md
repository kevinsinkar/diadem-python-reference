---
title: "IRepD3IsolineLabelInt"
description: "The 3DIsolineLabel object provides the properties of the labels for the additional isolines of a 3D axis system in the display modes Surface or Characteristic d"
---

# IRepD3IsolineLabelInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DIsolineLabel

The 3DIsolineLabel object provides the properties of the labels for the additional isolines of a 3D axis system in the display modes Surface or Characteristic diagram in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCharacteristicDiagram, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMy3DAxisSystem.Settings
oMySettings.RotationAngleXY = 90
oMySettings.RotationAngleZ = 270
oMyLabel = oMyShape.Extensions.Isoline.Label
oMyLabel.Visible = True
oMyLabel.UseCurveColor = False
oMyLabel.RepetitionMode = dd.e3DLabelRepetitionSurfaceLength
oMyLabel.RepetitionPercent = 10
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3isolinelabelint-angle/">Angle</a> | <a href="../../properties/irepd3isolinelabelint-font/">Font</a> | <a href="../../properties/irepd3isolinelabelint-format/">Format</a> | <a href="../../properties/irepd3isolinelabelint-referenceline1/">ReferenceLine1</a> | <a href="../../properties/irepd3isolinelabelint-referenceline2/">ReferenceLine2</a> | <a href="../../properties/irepd3isolinelabelint-referencelinedefinition/">ReferenceLineDefinition</a> | <a href="../../properties/irepd3isolinelabelint-relativeposition/">RelativePosition</a> | <a href="../../properties/irepd3isolinelabelint-repetitionmode/">RepetitionMode</a> | <a href="../../properties/irepd3isolinelabelint-repetitionpercent/">RepetitionPercent</a> | <a href="../../properties/irepd3isolinelabelint-repetitionvalue/">RepetitionValue</a> | <a href="../../properties/irepd3isolinelabelint-showatbegin/">ShowAtBegin</a> | <a href="../../properties/irepd3isolinelabelint-showatend/">ShowAtEnd</a> | <a href="../../properties/irepd3isolinelabelint-usecurvecolor/">UseCurveColor</a> | <a href="../../properties/irepd3isolinelabelint-visible/">Visible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3characteristicdiagramisolineadditionalint/">3DAdditionalCharacteristicDiagramIsoline</a>.<a href="../../properties/irepd3characteristicdiagramisolineadditionalint-label/">Label</a> | <a href="../irepd3surfaceisolineadditionalint/">3DAdditionalSurfaceIsoline</a>.<a href="../../properties/irepd3surfaceisolineadditionalint-label/">Label</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3IsolineLabelInt.htm`*
