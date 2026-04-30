---
title: "ITDMDataFinder.ResultsProperties"
description: "Returns the results of a column-oriented search without user interface in a DataFinder."
---

# ITDMDataFinder.ResultsProperties

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ResultsProperties for DataFinder

Returns the results of a column-oriented search without user interface in a DataFinder.

## Signature

```python
return_value = obj.ResultsProperties
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  The <a href="../itdmresultsproperties-maxcount/">MaxCount</a> property specifies the maximum number of elements that a search returns to the search results. The <a href="../itdmresultsproperties-isincomplete/">IsIncomplete</a> property specifies whether the search results contain all the search results elements.<br attr="ext"/>
</td></tr></table>
</div>

## Python example

```python
dd.Data.Root.Clear()

oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyQuery.ReturnType = dd.eSearchChannel
oMyConditions = oMyQuery.Conditions
oMyConditions.Add(dd.eSearchChannel,"maximum",">=","10")
oMyConditions.Logic = "C1"

oMyResultsColumns = oMyDataFinder.CreateResultsColumns()
oMyResultsColumns.RemoveAll()
oMyResultsColumns.Add(dd.eSearchChannelGroup, "name")
oMyResultsColumns.Add(dd.eSearchFile, "fileName")
oMyResultsColumns.Add(dd.eSearchFile, "folder")
oMyResultsColumns.Add(dd.eSearchChannel, "maximum")

oMyDataFinder.SearchProperties(oMyQuery, oMyResultsColumns)
oMyResultsProps = oMyDataFinder.ResultsProperties
dd.MsgBoxDisp("Results properties incomplete? " + oMyResultsProps.IsIncomplete)

dd.Navigator.LoadProperty(oMyResultsProps)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ResultsProperties_ITDMDataFinder.htm`*
