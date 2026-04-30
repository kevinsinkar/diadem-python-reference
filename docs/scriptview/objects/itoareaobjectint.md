---
title: "IToAreaObjectInt"
description: "The Area object provides an area in DIAdem VIEW. The Area object also provides access to the object that is displayed in the area. Split an existing Area object"
---

# IToAreaObjectInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Area

The Area object provides an area in DIAdem VIEW. The Area object also provides access to the object that is displayed in the area. Split an existing Area object to create new Area objects.

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.Name = "MySheet"
oMyArea = oMySheet.ActiveArea
oMyNewArea = oMyArea.SplitRight("NewArea", 0.5)
oMyNewArea.Active = True
oMyNewArea.DisplayObjType = "CurveChart2D"
oMyChart = oMyNewArea.DisplayObj
oMyCurve = oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itoareaobjectint-active/">Active</a> | <a href="../../properties/itoareaobjectint-bottommargin/">BottomMargin</a> | <a href="../../properties/itoareaobjectint-displayobj/">DisplayObj</a> | <a href="../../properties/itoareaobjectint-displayobjtype/">DisplayObjType</a> | <a href="../../properties/itoareaobjectint-index/">Index</a> | <a href="../../properties/itoareaobjectint-leftmargin/">LeftMargin</a> | <a href="../../properties/itoareaobjectint-name/">Name</a> | <a href="../../properties/itoareaobjectint-rightmargin/">RightMargin</a> | <a href="../../properties/itoareaobjectint-sheet/">Sheet</a> | <a href="../../properties/itoareaobjectint-tagstored/">TagStored</a> | <a href="../../properties/itoareaobjectint-tagtemporary/">TagTemporary</a> | <a href="../../properties/itoareaobjectint-topmargin/">TopMargin</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itoareaobjectint-getsize/">GetSize</a> | <a href="../../methods/itoareaobjectint-splitbottom/">SplitBottom</a> | <a href="../../methods/itoareaobjectint-splitleft/">SplitLeft</a> | <a href="../../methods/itoareaobjectint-splitright/">SplitRight</a> | <a href="../../methods/itoareaobjectint-splittop/">SplitTop</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="./">Area</a>.<a href="../../methods/itoareaobjectint-splitbottom/">SplitBottom</a> | <a href="./">Area</a>.<a href="../../methods/itoareaobjectint-splitleft/">SplitLeft</a> | <a href="./">Area</a>.<a href="../../methods/itoareaobjectint-splitright/">SplitRight</a> | <a href="./">Area</a>.<a href="../../methods/itoareaobjectint-splittop/">SplitTop</a> | <a href="../../collections/areas/">Areas</a>.<a href="../../methods/itoareaobjectscontint-copy/">Copy</a> | <a href="../../collections/areas/">Areas</a>.<a href="../../methods/itoareaobjectscontint-item/">Item</a> | <a href="../../collections/areas/">Areas</a>.<a href="../../methods/itoareaobjectscontint-move/">Move</a> | <a href="../itobirdseyeviewchartint/">BirdsEyeView</a>.<a href="../../properties/itobirdseyeviewchartint-area/">Area</a> | <a href="../itobodechartint/">Bode</a>.<a href="../../properties/itobodechartint-area/">Area</a> | <a href="../itocascadechartint/">Cascade</a>.<a href="../../properties/itocascadechartint-area/">Area</a> | <a href="../itochanneltableint/">ChannelTable</a>.<a href="../../properties/itochanneltableint-area/">Area</a> | <a href="../itocontourchartint/">Contour</a>.<a href="../../properties/itocontourchartint-area/">Area</a> | <a href="../ito2dchartint/">CurveChart2D</a>.<a href="../../properties/ito2dchartint-area/">Area</a> | <a href="../itosuddlgint/">Dialog</a>.<a href="../../properties/itosuddlgint-area/">Area</a> | <a href="../itodisplayobj/">DisplayObj</a>.<a href="../../properties/itodisplayobj-area/">Area</a> | <a href="../itodropeventcontext/">DropEventContext</a>.<a href="../../properties/itodropeventcontext-area/">Area</a> | <a href="../itomapdisplayint/">Map</a>.<a href="../../properties/itomapdisplayint-area/">Area</a> | <a href="../itoorbitchartint/">Orbit</a>.<a href="../../properties/itoorbitchartint-area/">Area</a> | <a href="../itopictureint/">Picture</a>.<a href="../../properties/itopictureint-area/">Area</a> | <a href="../itopolarchartint/">Polar</a>.<a href="../../properties/itopolarchartint-area/">Area</a> | <a href="../itopythongraphicint/">PythonGraphic</a>.<a href="../../properties/itopythongraphicint-area/">Area</a> | <a href="../itoshaftcenterlinechartint/">ShaftCenterline</a>.<a href="../../properties/itoshaftcenterlinechartint-area/">Area</a> | <a href="../itosheetint/">Sheet</a>.<a href="../../properties/itosheetint-activearea/">ActiveArea</a> | <a href="../itosheetint/">Sheet</a>.<a href="../../methods/itosheetint-copyarea/">CopyArea</a> | <a href="../itosheetint/">Sheet</a>.<a href="../../properties/itosheetint-currarea/">CurrArea</a> | <a href="../itosheetint/">Sheet</a>.<a href="../../methods/itosheetint-movearea/">MoveArea</a> | <a href="../itotextboxint/">TextBox</a>.<a href="../../properties/itotextboxint-area/">Area</a> | <a href="../itovideoint/">Video</a>.<a href="../../properties/itovideoint-area/">Area</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToAreaObjectInt.htm`*
