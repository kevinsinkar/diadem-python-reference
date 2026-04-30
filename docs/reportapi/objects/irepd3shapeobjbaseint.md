---
title: "IRepD3ShapeObjBaseInt"
description: "The 3DShapeObject object provides the properties of the curve in a 3D axis system in DIAdem REPORT. The 3DShapeObject object corresponds to one of the following"
---

# IRepD3ShapeObjBaseInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DShapeObject

The 3DShapeObject object provides the properties of the curve in a 3D axis system in DIAdem REPORT. The 3DShapeObject object corresponds to one of the following objects: 3DBars (IRepD3ShapeObjBarsInt) Bars 3DCharacteristicDiagram (IRepD3ShapeObjCharacteristicDiagramInt) Characteristic diagram 3DCoordinate (IRepD3ShapeObjCoordinateInt) Coordinate 3DIsolines (IRepD3ShapeObjIsolinesInt) Isolines 3DLine (IRepD3ShapeObjLineInt) 3D curve 3DMatrix2D (IRepD3ShapeObj2DMatrixInt) 2D matrix 3DPoints (IRepD3ShapeObjPointsInt) Points 3DSpikes (IRepD3ShapeObjSpikeInt) Spikes 3DSurface (IRepD3ShapeObjSurfaceInt) Surface 3DVector (IRepD3ShapeObjVectorInt) Vector 3DWaterfall (IRepD3ShapeObjWaterfallInt) Waterfall

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
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3curveint/">3DCurve</a>.<a href="../../properties/irepd3curveint-shape/">Shape</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjBaseInt.htm`*
