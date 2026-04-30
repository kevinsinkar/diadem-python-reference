---
title: "INavigatorSettings"
description: "The Settings object provides access to general settings in DIAdem NAVIGATOR."
---

# INavigatorSettings

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Settings <Navigator>

The Settings object provides access to general settings in DIAdem NAVIGATOR.

## Python example

```python
oMyStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyPropertyImportSet = dd.Navigator.Settings.CreatePropertyImportSet(oMyStore)
oMyPropertyImportSet.NamingSchema = dd.eNamingSchemaPropertyName
oMyPropertyImportSet.InheritanceMode = dd.eInheritanceNone
dd.Navigator.Settings.SavePropertyImportSet("C:\\MyPropImportSet.tdl", oMyPropertyImportSet)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/inavigatorsettings-registereddataplugins/">RegisteredDataPlugins</a> | <a href="../../properties/inavigatorsettings-registereddatastores/">RegisteredDataStores</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/inavigatorsettings-createbrowsesettings/">CreateBrowseSettings</a> | <a href="../../methods/inavigatorsettings-createcontextparameterset/">CreateContextParameterSet</a> | <a href="../../methods/inavigatorsettings-createdatapluginparameter/">CreateDataPluginParameter</a> | <a href="../../methods/inavigatorsettings-createimportparameter/">CreateImportParameter</a> | <a href="../../methods/inavigatorsettings-createpropertyimportset/">CreatePropertyImportSet</a> | <a href="../../methods/inavigatorsettings-createupdatesource/">CreateUpdateSource</a> | <a href="../../methods/inavigatorsettings-createvaluemapper/">CreateValueMapper</a> | <a href="../../methods/inavigatorsettings-loadbrowsesettings/">LoadBrowseSettings</a> | <a href="../../methods/inavigatorsettings-loadcontextparameterset/">LoadContextParameterSet</a> | <a href="../../methods/inavigatorsettings-loadpropertyimportset/">LoadPropertyImportSet</a> | <a href="../../methods/inavigatorsettings-loadvaluemapper/">LoadValueMapper</a> | <a href="../../methods/inavigatorsettings-registerdataplugin/">RegisterDataPlugin</a> | <a href="../../methods/inavigatorsettings-registerdataprovider/">RegisterDataProvider</a> | <a href="../../methods/inavigatorsettings-savebrowsesettings/">SaveBrowseSettings</a> | <a href="../../methods/inavigatorsettings-savecontextparameterset/">SaveContextParameterSet</a> | <a href="../../methods/inavigatorsettings-savepropertyimportset/">SavePropertyImportSet</a> | <a href="../../methods/inavigatorsettings-savevaluemapper/">SaveValueMapper</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../inavigator/">Navigator</a>.<a href="../../properties/inavigator-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_INavigatorSettings.htm`*
