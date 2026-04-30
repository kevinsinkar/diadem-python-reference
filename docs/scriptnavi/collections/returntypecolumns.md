---
title: "ReturnTypeColumns"
description: "Collection of the columns which the DIAdem NAVIGATOR displays in the search results list of a search for files ( eSearchFile ), for channel groups ( eSearchChan"
---

# ReturnTypeColumns

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: ReturnTypeColumns

Collection of the columns which the DIAdem NAVIGATOR displays in the search results list of a search for files ( eSearchFile ), for channel groups ( eSearchChannelgroup ), or for channels ( eSearchChannel ).

## Python example

```python
oMyReturnTypeColumn = dd.Navigator.Display.CurrDataFinder.ResultsList.Settings.Columns
print(oMyReturnTypeColumn.Item(dd.eSearchChannel).Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmreturntypecolumns-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmreturntypecolumns-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itdmresultsdisplaysettings/">ResultsListSettings</a>.<a href="../../properties/itdmresultsdisplaysettings-columns/">Columns</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMReturnTypeColumns.htm`*
