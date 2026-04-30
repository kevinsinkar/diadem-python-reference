---
title: "IToContourCurveInt.PartialLoadTolerance"
description: "Specifies the maximum deviation of the x-value in the partial load as a percentage of the complete x-area. Points whose x-values lie outside the tolerance belon"
---

# IToContourCurveInt.PartialLoadTolerance

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: PartialLoadTolerance for ContourCurve

Specifies the maximum deviation of the x-value in the partial load as a percentage of the complete x-area. Points whose x-values lie outside the tolerance belong to a further partial load. If a partial load has fewer than three points, DIAdem terminates the display.

## Signature

```python
obj.PartialLoadTolerance
```

## Python example

```python
dd.View.Sheets(1).Areas.Removeall()
dd.View.Sheets(1).Areas(1).DisplayObjType = "Contour"
oMyObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyContour = oMyObj.CurvesContour.AddContour("[4]/[1]","[4]/[2]","[4]/[3]")
oMyContour.Structure = "Triplet"
oMyContour.TripletDistribution = "PartialLoads"
oMyContour.PartialLoadTolerance = 5
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_PartialLoadTolerance_IToContourCurveInt.htm`*
