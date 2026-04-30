---
title: "3DCurves"
description: "Collection of all 3DCurve objects in DIAdem REPORT. Use the 3DCurves object to delete or to create new curves in 3D axis systems."
---

# 3DCurves

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: 3DCurves

Collection of all 3DCurve objects in DIAdem REPORT. Use the 3DCurves object to delete or to create new curves in 3D axis systems.

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
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3curvelistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepd3curvelistint-add/">Add</a> | <a href="../../methods/irepd3curvelistint-changeshape/">ChangeShape</a> | <a href="../../methods/irepd3curvelistint-copy/">Copy</a> | <a href="../../methods/irepd3curvelistint-exists/">Exists</a> | <a href="../../methods/irepd3curvelistint-item/">Item</a> | <a href="../../methods/irepd3curvelistint-move/">Move</a> | <a href="../../methods/irepd3curvelistint-remove/">Remove</a> | <a href="../../methods/irepd3curvelistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepd3axisint/">3DAxisSystem</a>.<a href="../../properties/irepd3axisint-curves3d/">Curves3D</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3CurveListInt.htm`*
