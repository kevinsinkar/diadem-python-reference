---
title: "IToContourCurveInt.TripletDistribution"
description: "Specifies the distribution of data triplets for contour displays in DIAdem VIEW."
---

# IToContourCurveInt.TripletDistribution

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: TripletDistribution for ContourCurve

Specifies the distribution of data triplets for contour displays in DIAdem VIEW.

## Signature

```python
obj.TripletDistribution
```

## Python example

```python
dd.View.Sheets(1).Areas.Removeall()
dd.View.Sheets(1).Areas(1).DisplayObjType = "Contour"
oMyObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyContour = oMyObj.CurvesContour.AddContour("[1]/[1]","[1]/[2]","[1]/[3]")
oMyContour.Structure = "Triplet"
oMyContour.TripletDistribution = "PartialLoads"
oMyContour.PartialLoadTolerance = 5
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_TripletDistribution_IToContourCurveInt.htm`*
