---
title: "ITDMDataFinderSettings"
description: "The DataFinderSettings object provides a DataFinder configuration. You use the DataFinderSettings object to create and to delete search areas, and folders that "
---

# ITDMDataFinderSettings

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: DataFinderSettings

The DataFinderSettings object provides a DataFinder configuration. You use the DataFinderSettings object to create and to delete search areas, and folders that are to be excluded from the search, to optimize custom properties, and to import and export DataFinder configurations. You only can use the DataFinderSettings object for the My DataFinder DataFinder.

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyDataFinderSettings = oMyDataFinder.GetSettings()
oMyPropertyList = oMyDataFinder.GetIndexedProperties(dd.eSearchChannelGroup)
if oMyPropertyList.Exists("Test_Name") :
    if oMyPropertyList.Item("Test_Name").DataType == dd.DataTypeOptiUnknown :
        oMyDataFinderSettings.OptimizeCustomProperty(dd.eSearchChannelGroup, "Test_Name", dd.DataTypeString)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmdatafindersettings-autocommit/">AutoCommit</a> | <a href="../../properties/itdmdatafindersettings-indexerschedule/">IndexerSchedule</a> | <a href="../../properties/itdmdatafindersettings-searchareas/">SearchAreas</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmdatafindersettings-commit/">Commit</a> | <a href="../../methods/itdmdatafindersettings-exportconfiguration/">ExportConfiguration</a> | <a href="../../methods/itdmdatafindersettings-importconfiguration/">ImportConfiguration</a> | <a href="../../methods/itdmdatafindersettings-optimizecustomproperty/">OptimizeCustomProperty</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itdmdatafinder/">DataFinder</a>.<a href="../../methods/itdmdatafinder-getsettings/">GetSettings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMDataFinderSettings.htm`*
