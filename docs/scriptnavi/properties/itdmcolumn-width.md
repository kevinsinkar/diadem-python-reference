---
title: "ITDMColumn.Width"
description: "Specifies the width of a column in the search results list of a DataFinder or of a data store, in dialog box units. You cannot change the width of the first col"
---

# ITDMColumn.Width

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Width for Column

Specifies the width of a column in the search results list of a DataFinder or of a data store, in dialog box units. You cannot change the width of the first column of the search results list. Therefore the index count starts in the second column.

## Signature

```python
obj.Width
```

## Python example

```python
oMyCurrDataProvider = dd.Navigator.Display.CurrDataFinder
oMyQueryForm = oMyCurrDataProvider.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType = dd.eSearchChannel
oMyConditions = oMyQueryForm.Conditions
#Setting query conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","TR_M17_QT_*")
oMyConditions.Add(dd.eSearchChannelGroup,"Test_Status","=","fail")
#Searching
oMyQueryForm.Search()
oMyResults = oMyCurrDataProvider.ResultsList.ResultsElements
#Defining width of results columns
oMyResultsColumns = oMyCurrDataProvider.ResultsList.Columns
oMyResultsColumns(1).Width = 120
#Loading results into Data Portal
dd.Navigator.LoadData(oMyResults)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Width_ITDMColumn.htm`*
