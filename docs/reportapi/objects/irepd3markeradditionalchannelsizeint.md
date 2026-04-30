---
title: "IRepD3MarkerAdditionalChannelSizeInt"
description: "The 3DAdditionalMarkerChannelSize object provides the properties of the curve markers of a 3D axis system in DIAdem REPORT."
---

# IRepD3MarkerAdditionalChannelSizeInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAdditionalMarkerChannelSize

The 3DAdditionalMarkerChannelSize object provides the properties of the curve markers of a 3D axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeLine, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[3]/[1]"
oMyShape.YChannel.Reference = "[3]/[2]"
oMyShape.ZChannel.Reference = "[3]/[3]"
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.dd"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 8
oMyLabel.Position.Type = dd.e3DLabelPositionAtPoint
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyMarker = oMyShape.Extensions.Marker
oMyMarker.Type = dd.eMarkerCircle
oMyMarker.Size = 2
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3markeradditionalchannelsizeint-channel/">Channel</a> | <a href="../../properties/irepd3markeradditionalchannelsizeint-filling/">Filling</a> | <a href="../../properties/irepd3markeradditionalchannelsizeint-line/">Line</a> | <a href="../../properties/irepd3markeradditionalchannelsizeint-minimumdisplaysize/">MinimumDisplaySize</a> | <a href="../../properties/irepd3markeradditionalchannelsizeint-size/">Size</a> | <a href="../../properties/irepd3markeradditionalchannelsizeint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjlineextensionsint/">3DLineExtensions</a>.<a href="../../properties/irepd3shapeobjlineextensionsint-marker/">Marker</a> | <a href="../irepd3shapeobjpointssettingsint/">3DPointsSettings</a>.<a href="../../properties/irepd3shapeobjpointssettingsint-marker/">Marker</a> | <a href="../irepd3shapeobjspikeextensionsint/">3DSpikesExtensions</a>.<a href="../../properties/irepd3shapeobjspikeextensionsint-marker/">Marker</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3MarkerAdditionalChannelSizeInt.htm`*
