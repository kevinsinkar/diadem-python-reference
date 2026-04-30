---
title: "ITDMResultsDisplaySettings"
description: "The ResultsListSettings object provides the settings of the search results list in a DataFinder or in a data store."
---

# ITDMResultsDisplaySettings

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: ResultsListSettings

The ResultsListSettings object provides the settings of the search results list in a DataFinder or in a data store.

## Python example

```python
dd.Navigator.Display.OpenDataFinder("My DataFinder")
oMyCurrDataProvider = dd.Navigator.Display.CurrDataFinder
oMyQueryForm = oMyCurrDataProvider.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType = dd.eSearchFile
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","Brake*")
oMyResultsList = oMyCurrDataProvider.ResultsList
oMySettings = oMyResultsList.Settings
oMySettings.ColumnHeaderDisplayMode = dd.eResultsHdrModeProperty
oMySettings.DetermineColumnsAutomatically = True
oMySettings.MaxCount = 100
oMyQueryForm.Search()
dd.MsgBoxDisp(oMyResultsList.ResultsElements.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmresultsdisplaysettings-columnheaderdisplaymode/">ColumnHeaderDisplayMode</a> | <a href="../../properties/itdmresultsdisplaysettings-columns/">Columns</a> | <a href="../../properties/itdmresultsdisplaysettings-determinecolumnsautomatically/">DetermineColumnsAutomatically</a> | <a href="../../properties/itdmresultsdisplaysettings-maxcount/">MaxCount</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmresultsdisplaysettings-resetcolumnwidths/">ResetColumnWidths</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../inavidatastoreresultdisplay/">ResultsList &lt;DataStore&gt;</a>.<a href="../../properties/inavidatastoreresultdisplay-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMResultsDisplaySettings.htm`*
