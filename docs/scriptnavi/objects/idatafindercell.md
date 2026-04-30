---
title: "IDataFinderCell"
description: "In a DataFinder the Cell object provides a cell of the search results list."
---

# IDataFinderCell

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Cell <DataFinder>

In a DataFinder the Cell object provides a cell of the search results list.

## Python example

```python
oMyCurrDataProvider = dd.Navigator.Display.CurrDataFinder
oMyQueryForm = oMyCurrDataProvider.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType = dd.eSearchFile
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","Brake*")
oMyQueryForm.Search()
dd.WndShow("NAVIGATOR", "SHOW")
dd.InterActionOn("Select one cell in the search results")
dd.WndShow("SCRIPT", "SHOW")
oMyResultsList = oMyCurrDataProvider.ResultsList
oMyCell = oMyResultsList.FocusedCell
dd.MsgBoxDisp(oMyCell.Element.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idatafindercell-column/">Column</a> | <a href="../../properties/idatafindercell-element/">Element</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/cellsselection/">CellsSelection</a>.<a href="../../methods/itdmresultsdisplaycellsselection-item/">Item</a> | <a href="../inavidatafinderresultdisplay/">ResultsList &lt;DataFinder&gt;</a>.<a href="../../properties/inavidatafinderresultdisplay-focusedcell/">FocusedCell</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IDataFinderCell.htm`*
