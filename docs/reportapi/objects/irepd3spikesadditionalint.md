---
title: "IRepD3SpikesAdditionalInt"
description: "The 3DAdditionalSpikes object provides the properties of the additional spikes display in 3D axis systems in DIAdem REPORT."
---

# IRepD3SpikesAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAdditionalSpikes

The 3DAdditionalSpikes object provides the properties of the additional spikes display in 3D axis systems in DIAdem REPORT.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySpike = oMyShape.Extensions.Spike
oMySpike.Visible = True
oMySpike.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySpike.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3spikesadditionalint-color/">Color</a> | <a href="../../properties/irepd3spikesadditionalint-interval/">Interval</a> | <a href="../../properties/irepd3spikesadditionalint-linetype/">LineType</a> | <a href="../../properties/irepd3spikesadditionalint-visible/">Visible</a> | <a href="../../properties/irepd3spikesadditionalint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjlineextensionsint/">3DLineExtensions</a>.<a href="../../properties/irepd3shapeobjlineextensionsint-spike/">Spike</a> | <a href="../irepd3shapeobjsurfaceextensionsint/">3DSurfaceExtensions</a>.<a href="../../properties/irepd3shapeobjsurfaceextensionsint-spike/">Spike</a> | <a href="../irepd3shapeobjwaterfallextensionsint/">3DWaterfallExtensions</a>.<a href="../../properties/irepd3shapeobjwaterfallextensionsint-spike/">Spike</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3SpikesAdditionalInt.htm`*
