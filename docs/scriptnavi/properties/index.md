---
title: "Properties (NAVIGATOR / Data Portal / Data Finder)"
---

# Properties

377 properties from `ScriptNavi.chm`.

| Name | Summary |
| --- | --- |
| [`ICommonExportParameter.DataPluginName`](icommonexportparameter-datapluginname.md) | Specifies the name of the DataPlugin when configuring the export of data with a selected DataPlugin. |
| [`ICSVExportParameter.DataPluginName`](icsvexportparameter-datapluginname.md) | Specifies the name of the DataPlugin to be configured, when data is exported with the CSV_Export DataPlugin. |
| [`ICSVExportParameter.DecimalSign`](icsvexportparameter-decimalsign.md) | Specifies which decimal symbol DIAdem uses for the exported file, when data is exported with the CSV_Export DataPlugin. The decimal sign must be different to the delimiter character. |
| [`ICSVExportParameter.Delimiter`](icsvexportparameter-delimiter.md) | Specifies which character DIAdem uses as separator for the data of the exported file, when data is exported with the CSV_Export DataPlugin. The delimiter character must be different to the decimal sign. |
| [`ICSVExportParameter.Encoding`](icsvexportparameter-encoding.md) | Specifies which coding DIAdem uses for the data of the exported file, when data is exported with the CSV_Export DataPlugin. |
| [`ICSVExportParameter.StringSign`](icsvexportparameter-stringsign.md) | Specifies the characters that enclose text in the exported file when data is exported with the CSV_Export DataPlugin. You can use any character, but you can specify only one character. |
| [`ICSVExportParameter.TimeFormat`](icsvexportparameter-timeformat.md) | Specifies which Date/time format DIAdem uses for the data of the exported file, when data is exported with the CSV_Export DataPlugin. You can use all Date/time formats available in DIAdem. |
| [`IDataFinderCell.Column`](idatafindercell-column.md) | Specifies in the search results list of a DataFinder a column with properties. |
| [`IDataFinderCell.Element`](idatafindercell-element.md) | Returns the element which is associated to a cell, in the search results list of a DataFinder. |
| [`IDataFinderDisplay.Browser`](idatafinderdisplay-browser.md) | Returns the file browser of the DIAdem NAVIGATOR interface, in a DataFinder. |
| [`IDataFinderDisplay.DataFinderVersion`](idatafinderdisplay-datafinderversion.md) | Specifies the version number of the DataFinder as text. |
| [`IDataFinderDisplay.DataFinderVersionNumber`](idatafinderdisplay-datafinderversionnumber.md) | Specifies the version number of the DataFinder as a double value. |
| [`IDataFinderDisplay.Name`](idatafinderdisplay-name.md) | Specifies the name of the DataFinder currently open. |
| [`IDataFinderDisplay.QueryForm`](idatafinderdisplay-queryform.md) | Returns the search input area of a DataFinder. |
| [`IDataFinderDisplay.ResultsList`](idatafinderdisplay-resultslist.md) | Returns the search results list of a search, in a DataFinder. |
| [`IDataFinderQuery.ReturnType`](idatafinderquery-returntype.md) | Specifies the return type of the search results in a search without the user interface in a DataFinder. |
| [`IDataFinderResultsDisplayElementsSelection.Count`](idatafinderresultsdisplayelementsselection-count.md) | Specifies the number of rows selected in a search results list of a DataFinder. |
| [`IDataPluginParameter.DataPluginName`](idatapluginparameter-datapluginname.md) | During the configuration of a DataPlugin, specifies the name of the DataPlugin for which the object was created. |
| [`IDataStoreBaseQuery.ReturnType`](idatastorebasequery-returntype.md) | Specifies the return type of the search results of a search without the user interface in a data store. |
| [`IDataStoreCell.Column`](idatastorecell-column.md) | Specifies in the search results list of a data store a column with properties. |
| [`IDataStoreCell.Element`](idatastorecell-element.md) | Returns the element which is associated to a cell, in the search results list of a data store. |
| [`IDataStoreDisplay.Browser`](idatastoredisplay-browser.md) | Returns the file browser of the DIAdem NAVIGATOR interface in a data store. |
| [`IDataStoreDisplay.IsQuerySupported`](idatastoredisplay-isquerysupported.md) | Specifies whether you can search for data in a data store. |
| [`IDataStoreDisplay.Name`](idatastoredisplay-name.md) | Specifies the name of the data store currently open. |
| [`IDataStoreDisplay.Plugin`](idatastoredisplay-plugin.md) | Specifies the DataPlugin with which DIADem opened a data store. |
| [`IDataStoreDisplay.PropertyImportSet`](idatastoredisplay-propertyimportset.md) | Returns the Loading Configuration of the data store open in DIAdem NAVIGATOR. |
| [`IDataStoreDisplay.QueryForm`](idatastoredisplay-queryform.md) | Returns the search input area of a data store. |
| [`IDataStoreDisplay.ResultsList`](idatastoredisplay-resultslist.md) | Returns the search results of a search in a data store. |
| [`IDataStoreResultsDisplayElementsSelection.Count`](idatastoreresultsdisplayelementsselection-count.md) | Specifies the number of rows selected in a search results list of a data store. |
| [`IDataStoreTextQuery.ReturnType`](idatastoretextquery-returntype.md) | Specifies the search results type of a search in a data store. You can only run a quick search in a data store if you access a DataFinder instance which is declared as an ASAM ODS server. The search results of a quick search in a data store is always a test type. |
| [`IDataStoreTextQuery.Text`](idatastoretextquery-text.md) | Specifies the search text for the quick search in a data store. You can only run a quick search in a data store if you access a DataFinder instance which is declared as an ASAM ODS server. |
| [`IDisplay.CurrDataFinder`](idisplay-currdatafinder.md) | Returns the current DataFinder. To do so a DataFinder must be open in DIAdem NAVIGATOR. |
| [`IDisplay.CurrDataStore`](idisplay-currdatastore.md) | Returns the current data store. To do so a data store must be open in DIAdem NAVIGATOR. |
| [`IEntityValueMappings.Count`](ientityvaluemappings-count.md) | Returns the number of possible levels on which you can define the mappings for properties, when mapping the values of a property in the data preparation. A level can be a file (eSearchFile), a channel group (eSearchChannelGroup), or a channel (eSearchChannel). The number of levels is always 3. |
| [`IEvents.OnAllowSearch`](ievents-onallowsearch.md) | Specifies the name of the user command that DIAdem executes before executing a search. The user command receives a parameter. This parameter specifies whether DIAdem executes the search after executing the user command (TRUE) or not (FALSE). |
| [`IEvents.OnContextMenuPointSelected`](ievents-oncontextmenupointselected.md) | Specifies the name of the user command that DIAdem executes when you select a context menu item in DIAdem NAVIGATOR. |
| [`IEvents.OnDataProviderClosing`](ievents-ondataproviderclosing.md) | Specifies the name of the user command that DIAdem executes after closing a DataFinder or a data store. |
| [`IEvents.OnDataProviderOpened`](ievents-ondataprovideropened.md) | Specifies the name of the user command that DIAdem executes after opening a DataFinder or a data store. |
| [`IEvents.OnDataStoreLoading`](ievents-ondatastoreloading.md) | Specifies the name of the user command that DIAdem executes before loading data from a data store. |
| [`IEvents.OnDataStoreSaving`](ievents-ondatastoresaving.md) | Specifies the name of the user command that DIAdem executes after saving a data store. |
| [`IEvents.OnFileLoading`](ievents-onfileloading.md) | Specifies the name of the user command that DIAdem executes before loading data from a file. |
| [`IEvents.OnInteractionLoaded`](ievents-oninteractionloaded.md) | Specifies the name of the user command that DIAdem executes after executing a command which was called when data was dragged and dropped into the Data Portal. |
| [`IEvents.OnInteractionLoading`](ievents-oninteractionloading.md) | Specifies the name of the user command that DIAdem executes before executing a command which was called when data was dragged and dropped into the Data Portal. |
| [`IEvents.OnLoaded`](ievents-onloaded.md) | Specifies the name of the user command that DIAdem executes after loading data. |
| [`IEvents.OnSearched`](ievents-onsearched.md) | Specifies the name of the user command that DIAdem executes after executing a search. |
| [`IEvents.OnShowingContextMenu`](ievents-onshowingcontextmenu.md) | Specifies the name of the user command that DIAdem executes when you open a context menu in DIAdem NAVIGATOR. |
| [`IImportParameterSet.AppendCheckGroupName`](iimportparameterset-appendcheckgroupname.md) | Specifies how DIAdem deals with group names when appending external data to the data in the Data Portal. |
| [`IImportParameterSet.BulkDataLoadingMode`](iimportparameterset-bulkdataloadingmode.md) | Specifies the time when DIAdem loads the mass data of the files, whose metadata was previously loaded with a load command, into the Data Portal. |
| [`IImportParameterSet.ChannelRelationMode`](iimportparameterset-channelrelationmode.md) | Specifies whether DIAdem retains the channel reference between the x-channels to the y-channels when importing data. |
| [`IImportParameterSet.ImportMode`](iimportparameterset-importmode.md) | Specifies whether a load command loads, registers, appends or expands the data. |
| [`IImportParameterSet.LoadReturnMode`](iimportparameterset-loadreturnmode.md) | Specifies with which elements a load command fills the returned elements list. |
| [`IImportParameterSet.PropertyHandling`](iimportparameterset-propertyhandling.md) | Contains the configuration of properties when loading data in DIAdem. |
| [`INaviDataFinderBrowser.FocusedElement`](inavidatafinderbrowser-focusedelement.md) | Specifies in the file browser of a DataFinder the element that has the focus. |
| [`INaviDataFinderBrowser.IsActive`](inavidatafinderbrowser-isactive.md) | Specifies whether the file browser is active in a DataFinder. |
| [`INaviDataFinderBrowser.OnlyShowSearchAreas`](inavidatafinderbrowser-onlyshowsearchareas.md) | Specifies in the file browser of a DataFinder whether only search areas or additionally the local file system is displayed. |
| [`INaviDataFinderBrowser.SelectedElements`](inavidatafinderbrowser-selectedelements.md) | Specifies in the file browser of a DataFinder the currently selected elements. |
| [`INaviDataFinderQueryForm.Conditions`](inavidatafinderqueryform-conditions.md) | Specifies the Search parameters for an advanced search in the interface of a DataFinder. |
| [`INaviDataFinderQueryForm.Mode`](inavidatafinderqueryform-mode.md) | Specifies whether DIAdem displays in a DataFinder the quick search or the advanced search for properties. By default DIAdem uses the quick search. |
| [`INaviDataFinderQueryForm.ResultsMode`](inavidatafinderqueryform-resultsmode.md) | Specifies whether you search for elements or execute a column-oriented search for properties on the DataFinder interface. |
| [`INaviDataFinderQueryForm.ReturnType`](inavidatafinderqueryform-returntype.md) | Specifies the search results type in a search in the interface of a DataFinder. Possible types are files ( eSearchFile ), channel groups ( eSearchChannelGroup ), and channels ( eSearchChannel ). |
| [`INaviDataFinderQueryForm.Text`](inavidatafinderqueryform-text.md) | Specifies the search text of the DataFinder quick search. |
| [`INaviDataFinderQueryForm.ValueMaxCount`](inavidatafinderqueryform-valuemaxcount.md) | Specifies the maximum number of indexed values that DIAdem displays in the search input area of a DataFinder. |
| [`INaviDataFinderResultDisplay.CellsSelection`](inavidatafinderresultdisplay-cellsselection.md) | Specifies in the results list of a DataFinder the cells currently selected. |
| [`INaviDataFinderResultDisplay.Columns`](inavidatafinderresultdisplay-columns.md) | Specifies in the search results list of a DataFinder all the columns with properties except the column Search Results . If you run an advanced search, DIAdem automatically adds columns with the properties that you searched for. Select Configure Search Results List from the context menu of the search results list to manually add further columns with properties. You only can remove columns which were added manually. |
| [`INaviDataFinderResultDisplay.ColumnsSelection`](inavidatafinderresultdisplay-columnsselection.md) | Specifies in the results list of a DataFinder the columns currently selected. |
| [`INaviDataFinderResultDisplay.Elements`](inavidatafinderresultdisplay-elements.md) | Use the new properties ResultsElements and ResultsProperties instead of the property Elements . |
| [`INaviDataFinderResultDisplay.ElementsSelection`](inavidatafinderresultdisplay-elementsselection.md) | Returns the elements which you have currently selected, in the search results list of a DataFinder. |
| [`INaviDataFinderResultDisplay.FocusedCell`](inavidatafinderresultdisplay-focusedcell.md) | Returns the cell with the focus in the search results, in a DataFinder. |
| [`INaviDataFinderResultDisplay.IsActive`](inavidatafinderresultdisplay-isactive.md) | Specifies whether the search results list is active in a DataFinder. |
| [`INaviDataFinderResultDisplay.ResultsElements`](inavidatafinderresultdisplay-resultselements.md) | Returns a collection of the currently displayed search results in a DataFinder interface search. |
| [`INaviDataFinderResultDisplay.ResultsProperties`](inavidatafinderresultdisplay-resultsproperties.md) | Specifies the search result of a column-oriented interface search in a DataFinder. |
| [`INaviDataFinderResultDisplay.Selection`](inavidatafinderresultdisplay-selection.md) | Specifies the elements, cells, or columns currently selected in the search results list of a DataFinder. |
| [`INaviDataFinderResultDisplay.Settings`](inavidatafinderresultdisplay-settings.md) | Specifies the settings of the search results list in a DataFinder. |
| [`INaviDataStoreBrowser.EnableDropData`](inavidatastorebrowser-enabledropdata.md) | Enables you to drop data from the Data Portal into data stores to save data. Note If you drag and droop data from the Data Portal into the data browser, DIAdem executes the event OnDataStoreSaving . With this event you can determine, for example, which element is selected in the Data Portal and on which file the focus in the data browser is before you save data. |
| [`INaviDataStoreBrowser.FocusedElement`](inavidatastorebrowser-focusedelement.md) | Specifies in the data browser of a data store the element that has the focus. |
| [`INaviDataStoreBrowser.IsActive`](inavidatastorebrowser-isactive.md) | Specifies whether the data browser is active in a data store. |
| [`INaviDataStoreBrowser.SelectedElements`](inavidatastorebrowser-selectedelements.md) | Specifies the selected elements in the file browser of a data store. |
| [`INaviDataStoreQueryForm.Conditions`](inavidatastorequeryform-conditions.md) | Specifies the search parameters for a search in the interface of a data store. |
| [`INaviDataStoreQueryForm.IsFilterActive`](inavidatastorequeryform-isfilteractive.md) | Specifies whether a Filter is set in the search input area of a data store. Use the filter to limit the view of the data store in the data browser to specified elements. |
| [`INaviDataStoreQueryForm.Mode`](inavidatastorequeryform-mode.md) | Specifies whether DIAdem displays in a data store the quick search or the advanced search for properties. By default DIAdem uses the advanced search to search for elements. You can only execute a quick search in a data store if you access a DataFinder instance which is declared as an ASAM ODS server. |
| [`INaviDataStoreQueryForm.ResultsMode`](inavidatastorequeryform-resultsmode.md) | Specifies whether you search for data elements or execute a column-oriented search for properties on the data store interface. If you search for elements ( ResultsMode = eResultsModeElements) , DIAdem returns the search results in the property ResultsList . ResultsElements . If you execute a column oriented search ( ResultsMode = eResultsModeProperties ), DIAdem returns the search results in the property ResultsList . ResultsProperties . |
| [`INaviDataStoreQueryForm.ReturnType`](inavidatastorequeryform-returntype.md) | Specifies the search results type in a search in the interface of a data store. |
| [`INaviDataStoreQueryForm.Text`](inavidatastorequeryform-text.md) | Specifies the search text for the quick search in a data store. You can only run a quick search in a data store if you access a DataFinder instance which is declared as an ASAM ODS server. |
| [`INaviDataStoreQueryForm.ValueMaxCount`](inavidatastorequeryform-valuemaxcount.md) | Specifies the maximum number of indexed values that DIAdem displays in the search input area of a data store. |
| [`INaviDataStoreResultDisplay.CellsSelection`](inavidatastoreresultdisplay-cellsselection.md) | Specifies in the results list of a data store the cells currently selected. |
| [`INaviDataStoreResultDisplay.Columns`](inavidatastoreresultdisplay-columns.md) | Specifies in the search results list of a data store all the columns with properties except the column Results List. DIAdem automatically displays additional columns with the properties that you searched for. Select Configure Search Results List from the context menu of the search results list to manually add further columns with properties. You only can remove columns which were added manually. |
| [`INaviDataStoreResultDisplay.ColumnsSelection`](inavidatastoreresultdisplay-columnsselection.md) | Specifies in the results list of a data store the columns currently selected. |
| [`INaviDataStoreResultDisplay.Elements`](inavidatastoreresultdisplay-elements.md) | Use the new property ResultsElements instead of the Elements property. |
| [`INaviDataStoreResultDisplay.ElementsSelection`](inavidatastoreresultdisplay-elementsselection.md) | Returns the elements which are currently selected in the search results list of a data store. |
| [`INaviDataStoreResultDisplay.FocusedCell`](inavidatastoreresultdisplay-focusedcell.md) | Returns the cell with the focus in the search results, in a data store. |
| [`INaviDataStoreResultDisplay.IsActive`](inavidatastoreresultdisplay-isactive.md) | Specifies whether the search results list is active in a data store. |
| [`INaviDataStoreResultDisplay.ResultsElements`](inavidatastoreresultdisplay-resultselements.md) | Returns in an interface search of a data store a collection of the currently displayed search results. |
| [`INaviDataStoreResultDisplay.ResultsProperties`](inavidatastoreresultdisplay-resultsproperties.md) | Specifies the search result of a column-oriented interface search in a data store. If you search for elements ( ResultsMode = eResultsModeElements) , DIAdem returns the search results in the property ResultsList . ResultsElements . If you execute a column oriented search ( ResultsMode = eResultsModeProperties ), DIAdem returns the search results in the property ResultsList . ResultsProperties . |
| [`INaviDataStoreResultDisplay.Selection`](inavidatastoreresultdisplay-selection.md) | Specifies the elements, cells, or columns currently selected in the search results list of a data store. |
| [`INaviDataStoreResultDisplay.Settings`](inavidatastoreresultdisplay-settings.md) | Specifies the settings of the search results list in a data store. |
| [`INavigator.Display`](inavigator-display.md) | Contains methods and properties which refer to the search with a DataFinder or a data store on the DIAdem NAVIGATOR interface. |
| [`INavigator.Events`](inavigator-events.md) | Returns the object which contains the names of the user commands for events, in DIAdem NAVIGATOR. |
| [`INavigator.Settings`](inavigator-settings.md) | Provides general DIAdem NAVIGATOR settings, for example, the methods for loading, creating, and saving a Loading Configuration . |
| [`INavigatorSettings.RegisteredDataPlugins`](inavigatorsettings-registereddataplugins.md) | Specifies the DataPlugins registered on your computer in DIAdem NAVIGATOR. |
| [`INavigatorSettings.RegisteredDataStores`](inavigatorsettings-registereddatastores.md) | Specifies the data stores registered on your computer. |
| [`IPropertyHandling.AutoUpdateChnCharacteristics`](ipropertyhandling-autoupdatechncharacteristics.md) | Specifies whether or not DIAdem calculates the characteristic values, when loading data automatically according to specific criteria. Per default DIAdem does not automatically calculate the characteristic values. If the loaded data did not contain characteristic values and DIAdem does not calculate characteristic values, this data is then missing in the data set. |
| [`IPropertyHandling.ImportSet`](ipropertyhandling-importset.md) | Accepts a Loading Configuration for an ASAM data store. The load configuration specifies, which properties of an ASAM data store DIAdem imports when also loading the mass data into the Data Portal. |
| [`IPropertyHandling.InheritanceMode`](ipropertyhandling-inheritancemode.md) | Specifies whether DIAdem also transfers the properties of elements from superordinate levels to the element in the Data Portal when loading data from a DataFinder or an ASAM data store. |
| [`IPropertyHandling.InheritanceSeparator`](ipropertyhandling-inheritanceseparator.md) | Specifies whether DIAdem uses the underscore or the tilde as the separator for the inheritance of properties. |
| [`IPropertyHandling.NameMappingFile`](ipropertyhandling-namemappingfile.md) | Specifies the name of a Technical Property Identifier Mapping file ( *.TPIM ). You are using TPIM files to replace the property identifiers. |
| [`IPropertyHandling.NamingSchema`](ipropertyhandling-namingschema.md) | Specifies the name pattern of properties after the properties are loaded into the Data Portal. If you load data from a DataFinder or an ASAM data store into the Data Portal, DIAdem names the properties in the Data Portal according to these rules. |
| [`IPropertyHandling.ValueMappingFile`](ipropertyhandling-valuemappingfile.md) | Specifies the name of a Technical Property Value Mapping file ( *.TPVM ). You are using TPVM files to replace the property values. |
| [`IPropertyImportProperties.Count`](ipropertyimportproperties-count.md) | Specifies the number of elements of the Loading Configuration of Data Stores . An element consists of a property and the property type. |
| [`IPropertyImportProperty.Property`](ipropertyimportproperty-property.md) | Specifies a property containing a Loading Configuration for a data source. |
| [`IPropertyImportProperty.Type`](ipropertyimportproperty-type.md) | Specifies the property type of a Loading Configuration of Data Stores . The names of the types depend on the data model on which the data store is based. |
| [`IPropertyImportSet.InheritanceMode`](ipropertyimportset-inheritancemode.md) | Specifies for the Loading Configuration of an ASAM data store the inheritance type of the properties, which DIAdem uses when loading data from data stores into the Data Portal. |
| [`IPropertyImportSet.InheritanceSeparator`](ipropertyimportset-inheritanceseparator.md) | Specifies for the Loading Configuration of an ASAM data store the inheritance separators of the properties, which DIAdem uses when loading data from data stores into the Data Portal. |
| [`IPropertyImportSet.isModified`](ipropertyimportset-ismodified.md) | Specifies whether the Loading configuration of a data store was changed. |
| [`IPropertyImportSet.NamingSchema`](ipropertyimportset-namingschema.md) | Specifies for the Loading configuration of an ASAM data store, the naming of the properties which DIAdem loads from a data store into the Data Portal. |
| [`IPropertyImportSet.Properties`](ipropertyimportset-properties.md) | Returns the properties that a Loading Configuration contains for a data source. When loading data from this data source, DIAdem loads only the properties specified here. |
| [`IRegisteredDataPlugin.Description`](iregistereddataplugin-description.md) | Specifies the description of a DataPlugin registered on your computer. |
| [`IRegisteredDataPlugin.FileExtensionList`](iregistereddataplugin-fileextensionlist.md) | Specifies the list with the filename extensions of the files which you can load with a registered DataPlugin. You can specify the list of filename extensions only for file-based DataPlugins. Use the IsFileBased method to determine whether a DataPlugin is file-based. |
| [`IRegisteredDataPlugin.IsFastLoadingSupported`](iregistereddataplugin-isfastloadingsupported.md) | Specifies whether a DataPlugin supports fast loading. |
| [`IRegisteredDataPlugin.IsFileBased`](iregistereddataplugin-isfilebased.md) | Specifies whether you can use a DataPlugin registered on your computer to load files. |
| [`IRegisteredDataPlugin.IsLoadingSupported`](iregistereddataplugin-isloadingsupported.md) | Specifies whether a DataPlugin supports reading data. |
| [`IRegisteredDataPlugin.IsProtected`](iregistereddataplugin-isprotected.md) | Specifies whether a DataPlugin registered on your computer is protected. You cannot change or delete protected DataPlugins. |
| [`IRegisteredDataPlugin.IsQuerySupported`](iregistereddataplugin-isquerysupported.md) | Specifies whether a DataPlugin can process queries. |
| [`IRegisteredDataPlugin.IsRegisterSupported`](iregistereddataplugin-isregistersupported.md) | Specifies whether a DataPlugin supports data registration. |
| [`IRegisteredDataPlugin.IsSavingSupported`](iregistereddataplugin-issavingsupported.md) | Specifies whether a DataPlugin supports saving data in a file. |
| [`IRegisteredDataPlugin.IsSelectiveLoadingSupported`](iregistereddataplugin-isselectiveloadingsupported.md) | Specifies whether a DataPlugin supports selective data loading. |
| [`IRegisteredDataPlugin.IsTdmModel`](iregistereddataplugin-istdmmodel.md) | Specifies whether a DataPlugin registered on your computer is based on the TDM data model and therefore provides TDM data. |
| [`IRegisteredDataPlugin.ModelName`](iregistereddataplugin-modelname.md) | Specifies the name of the data model on which a DataPlugin is based. |
| [`IRegisteredDataPlugin.Name`](iregistereddataplugin-name.md) | Specifies the name of a DataPlugin registered on your computer. |
| [`IRegisteredDataPlugin.Type`](iregistereddataplugin-type.md) | Specifies the type of a DataPlugin registered on your computer. |
| [`IRegisteredDataPlugin.Version`](iregistereddataplugin-version.md) | Specifies the version number of a DataPlugin registered on your computer. |
| [`IRegisteredDataPluginCollection.Count`](iregistereddataplugincollection-count.md) | Specifies the number of DataPlugins registered on your computer. |
| [`IRegisteredDataStore.DataPluginName`](iregistereddatastore-datapluginname.md) | Specifies the name of a DataPlugin. |
| [`IRegisteredDataStore.Name`](iregistereddatastore-name.md) | Specifies the name of a connection definition of a data store on your computer. |
| [`IRegisteredDataStore.Parameter`](iregistereddatastore-parameter.md) | Specifies the parameters of a connection to a data store as a string. |
| [`IRegisteredDataStoreCollection.Count`](iregistereddatastorecollection-count.md) | Specifies the number of data stores registered on your computer. |
| [`ISUSIChannel.ChannelGroup`](isusichannel-channelgroup.md) | Returns the channel group of a channel in a DataFinder. |
| [`ISUSIChannel.Name`](isusichannel-name.md) | Specifies in a DataFinder the name of a channel. |
| [`ISUSIChannel.Properties`](isusichannel-properties.md) | Returns the properties of a channel in a DataFinder. |
| [`ISUSIChannelGroup.Channels`](isusichannelgroup-channels.md) | Returns the channels of a channel group in a DataFinder. |
| [`ISUSIChannelGroup.Name`](isusichannelgroup-name.md) | Specifies in a DataFinder the name of a channel group. |
| [`ISUSIChannelGroup.Properties`](isusichannelgroup-properties.md) | Returns the properties of a channel group in a DataFinder. |
| [`ISUSIChannelGroup.Root`](isusichannelgroup-root.md) | Returns the file of a channel group in a DataFinder. |
| [`ISUSIChannelGroups.Count`](isusichannelgroups-count.md) | Specifies in a DataFinder the number of channel groups of a ChannelGroups collection. |
| [`ISUSIChannels.Count`](isusichannels-count.md) | Specifies in a DataFinder the number of channels of a Channels collection. The Channels collection contains all channels of a channel group. |
| [`ISUSIElement.Name`](isusielement-name.md) | Specifies in a DataFinder the name of an element. |
| [`ISUSIElement.Properties`](isusielement-properties.md) | Returns the properties of an element in a DataFinder. |
| [`ISUSIElements.Count`](isusielements-count.md) | Specifies in a DataFinder the number of elements of an Elements collection. |
| [`ISUSIElements.IsIncomplete`](isusielements-isincomplete.md) | Specifies whether the search results list of a DataFinder contains all the elements of the search results. If the IsIncomplete property has the value TRUE , the search has more results than the MaxCount property specifies. |
| [`ISUSIElements.MaxCount`](isusielements-maxcount.md) | Specifies in a DataFinder the maximum number of elements that a search returns to the search results list. |
| [`ISUSIProperties.Count`](isusiproperties-count.md) | Specifies in a DataFinder the number of properties of a Properties collection. |
| [`ISUSIProperty.DataType`](isusiproperty-datatype.md) | Specifies in a DataFinder the data type of a property. |
| [`ISUSIProperty.Default`](isusiproperty-default.md) | Specifies in a DataFinder whether a property is a default property or a custom property. The Default property returns the value TRUE if the property is a default property. |
| [`ISUSIProperty.DisplayName`](isusiproperty-displayname.md) | Specifies in a DataFinder the display name of a property . The display name is the property name that DIAdem displays on the user interface. |
| [`ISUSIProperty.Hidden`](isusiproperty-hidden.md) | Specifies whether DIAdem displays a property on the interface by default. In DIAdem you can hide only the register properties. These properties remain in the associated collections so that you can still access these properties in a script. |
| [`ISUSIProperty.Name`](isusiproperty-name.md) | Specifies in a DataFinder the name of a property . |
| [`ISUSIProperty.Value`](isusiproperty-value.md) | Specifies in a DataFinder the value of a file property , a channel group property, or a channel property. |
| [`ISUSIRoot.ChannelGroups`](isusiroot-channelgroups.md) | Returns the channel groups of a file in a DataFinder. |
| [`ISUSIRoot.Name`](isusiroot-name.md) | Specifies in a DataFinder the name of a file. |
| [`ISUSIRoot.Properties`](isusiroot-properties.md) | Returns the properties of a file in a DataFinder. |
| [`ITDMBrowseEntity.ChildEntity`](itdmbrowseentity-childentity.md) | Specifies in the browse path of a data store the entity located below a given entity. |
| [`ITDMBrowseEntity.ChildPath`](itdmbrowseentity-childpath.md) | Specifies in the browse path of a data store the reference to the subordinate entity. |
| [`ITDMBrowseEntity.EntityType`](itdmbrowseentity-entitytype.md) | Specifies in the browse path of a data store the type of an entity. |
| [`ITDMBrowseEntity.ParentEntity`](itdmbrowseentity-parententity.md) | Specifies in the browse path of a data store the entity located above a given entity. |
| [`ITDMBrowseEntity.ParentPath`](itdmbrowseentity-parentpath.md) | Specifies in the browse path of a data store the reference to the superordinate entity. |
| [`ITDMBrowseSettings.RootElements`](itdmbrowsesettings-rootelements.md) | Returns the elements that correspond to the root level of the browse path in a data store. |
| [`ITDMBrowseSettings.RootEntity`](itdmbrowsesettings-rootentity.md) | Specifies in a data store the top entity of a browse path . |
| [`ITDMCell.Column`](itdmcell-column.md) | Specifies in the search results list of a DataFinder or a data store a column with properties. |
| [`ITDMColumn.DataType`](itdmcolumn-datatype.md) | Specifies the data type of a properties column in the search results. Note DIAdem automatically specifies the data type of base properties and optimized custom properties. Use the Add method to specify the data type of non-optimized custom properties. |
| [`ITDMColumn.Property`](itdmcolumn-property.md) | Specifies in a DataFinder or in a data store a property from a column of the search results list. |
| [`ITDMColumn.Type`](itdmcolumn-type.md) | Specifies the type of a column in the search results list of a DataFinder or of a data store. |
| [`ITDMColumn.Width`](itdmcolumn-width.md) | Specifies the width of a column in the search results list of a DataFinder or of a data store, in dialog box units. You cannot change the width of the first column of the search results list. Therefore the index count starts in the second column. |
| [`ITDMColumns.Count`](itdmcolumns-count.md) | Specifies in a DataFinder or a data store the number of columns in the results list. |
| [`ITDMContextParameter.DataType`](itdmcontextparameter-datatype.md) | Specifies the data type of a context parameter. |
| [`ITDMContextParameter.Name`](itdmcontextparameter-name.md) | Specifies the name of a context parameter. |
| [`ITDMContextParameter.Value`](itdmcontextparameter-value.md) | Specifies the value of a context parameter. |
| [`ITDMContextParameters.Count`](itdmcontextparameters-count.md) | Specifies the number of context parameters in a ContextParameters collection. |
| [`ITDMContextParameterSet.Name`](itdmcontextparameterset-name.md) | Specifies the name of a context parameters set. |
| [`ITDMContextParameterSet.Parameters`](itdmcontextparameterset-parameters.md) | Specifies the collection of context parameters in a context parameter set. |
| [`ITDMDataFinder.Indexer`](itdmdatafinder-indexer.md) | Provides the methods which you use to reindex files and folders, in a DataFinder. You cannot use the indexer object for DataFinders located on another host. |
| [`ITDMDataFinder.Name`](itdmdatafinder-name.md) | Specifies the name of the DataFinder where you execute a search without the interface. |
| [`ITDMDataFinder.Results`](itdmdatafinder-results.md) | Use the new properties ResultsElements and ResultsProperties instead of the property Results . |
| [`ITDMDataFinder.ResultsElements`](itdmdatafinder-resultselements.md) | Returns in a DataFinder the search results of a search without user interface for elements. |
| [`ITDMDataFinder.ResultsProperties`](itdmdatafinder-resultsproperties.md) | Returns the results of a column-oriented search without user interface in a DataFinder. |
| [`ITDMDataFinder.ValueMaxCount`](itdmdatafinder-valuemaxcount.md) | Specifies the maximum length of the list of indexed values when a DataFinder is being searched without the interface. |
| [`ITDMDataFinder.Version`](itdmdatafinder-version.md) | Returns the version number of the DataFinder as text. |
| [`ITDMDataFinder.VersionNumber`](itdmdatafinder-versionnumber.md) | Returns the version number of the DataFinder as a double value. |
| [`ITDMDataFinderAdvancedQuery.Conditions`](itdmdatafinderadvancedquery-conditions.md) | Specifies the search parameters for a search without the interface in a DataFinder. |
| [`ITDMDataFinderAdvancedQuery.ReturnType`](itdmdatafinderadvancedquery-returntype.md) | Specifies the search results type in an advanced search in a DataFinder. |
| [`ITDMDataFinderCondition.Name`](itdmdatafindercondition-name.md) | Specifies in a DataFinder the name of a search condition, for example, C1 or C2 . |
| [`ITDMDataFinderCondition.Operator`](itdmdatafindercondition-operator.md) | Specifies the operator that DIAdem uses in a DataFinder for a search condition. |
| [`ITDMDataFinderCondition.OrderBy`](itdmdatafindercondition-orderby.md) | Specifies the Sorting order of the search results when searching with the DataFinder. |
| [`ITDMDataFinderCondition.Property`](itdmdatafindercondition-property.md) | Specifies in a DataFinder the property of a search condition. |
| [`ITDMDataFinderCondition.Size`](itdmdatafindercondition-size.md) | Returns in a search in a DataFinder the number of values in a search condition that are connected with OR. |
| [`ITDMDataFinderCondition.Type`](itdmdatafindercondition-type.md) | Specifies whether DIAdem searches in properties of a file, a group, or a channel, in a DataFinder. |
| [`ITDMDataFinderCondition.Value`](itdmdatafindercondition-value.md) | Specifies the value which DIAdem searches for in an advanced search in a DataFinder. |
| [`ITDMDataFinderCondition.Values`](itdmdatafindercondition-values.md) | Specifies in a DataFinder a vector with values of a search condition. The size of the vector depends on the Size property. |
| [`ITDMDataFinderConditions.Count`](itdmdatafinderconditions-count.md) | Specifies in a DataFinder the number of search parameters of an advanced search. |
| [`ITDMDataFinderConditions.Logic`](itdmdatafinderconditions-logic.md) | Returns the logical operations of search conditions of a DataFinder in the search input area. You can connect search conditions with AND and OR. Use parentheses to specify the order of the evaluation. |
| [`ITDMDataFinderExcludeFolder.LocalPath`](itdmdatafinderexcludefolder-localpath.md) | Specifies the path to a folder that is excluded from a search in a search area, in a DataFinder configuration. |
| [`ITDMDataFinderExcludeFolder.Name`](itdmdatafinderexcludefolder-name.md) | Specifies in a DataFinder configuration the alias of a folder that is excluded from the search in a search area. |
| [`ITDMDataFinderExcludeFolders.Count`](itdmdatafinderexcludefolders-count.md) | Specifies the number of folders that are excluded from the search in a search area, in a DataFinder configuration. |
| [`ITDMDataFinderIndexer.Status`](itdmdatafinderindexer-status.md) | Specifies in a DataFinder the status of the indexer. |
| [`ITDMDataFinderIndexerSchedule.Interval`](itdmdatafinderindexerschedule-interval.md) | Specifies the intervals at which the DataFinder repeats the indexing of the search areas, in a DataFinder configuration. |
| [`ITDMDataFinderIndexerSchedule.StartTime`](itdmdatafinderindexerschedule-starttime.md) | Specifies the time at which the DataFinder indexes the search areas, in a DataFinder configuration. Use the Interval property to specify the interval at which the DataFinder indexes. If you specify a weekly interval, you must also specify the weekday. Otherwise, you specify only the time. You can use this method only on the computer on which the DataFinder is active. |
| [`ITDMDataFinderIndexerSchedule.Weekday`](itdmdatafinderindexerschedule-weekday.md) | Specifies the weekday on which the DataFinder indexes the search areas, in a DataFinder configuration. You can assign a value to the Weekday property only if the DataFinder indexes the search areas every week. |
| [`ITDMDataFinderSearchArea.ClientPath`](itdmdatafindersearcharea-clientpath.md) | Specifies in a DataFinder configuration the path that the client uses to access a search area. |
| [`ITDMDataFinderSearchArea.ExcludeFolders`](itdmdatafindersearcharea-excludefolders.md) | Returns a collection of the folders in a search area that the DataFinder excludes from a search, in a DataFinder configuration. |
| [`ITDMDataFinderSearchArea.LocalPath`](itdmdatafindersearcharea-localpath.md) | Specifies the path to a search area in a DataFinder configuration. |
| [`ITDMDataFinderSearchArea.Name`](itdmdatafindersearcharea-name.md) | Specifies the alias of a search area in a DataFinder configuration. |
| [`ITDMDataFinderSearchAreas.Count`](itdmdatafindersearchareas-count.md) | Specifies the number of search areas in a DataFinder configuration. |
| [`ITDMDataFinderSettings.AutoCommit`](itdmdatafindersettings-autocommit.md) | Specifies whether the DataFinder accepts configuration changes immediately or whether the DataFinder first saves the changes. If you assign the value TRUE to the AutoCommit property, the DataFinder changes the configuration directly. If you assign the value FALSE to the AutoCommit property, you must first execute the Commit method before the DataFinder makes the changes. |
| [`ITDMDataFinderSettings.IndexerSchedule`](itdmdatafindersettings-indexerschedule.md) | Returns the settings for the indexer schedule in a DataFinder configuration. |
| [`ITDMDataFinderSettings.SearchAreas`](itdmdatafindersettings-searchareas.md) | Returns a collection of all search areas, in a DataFinder configuration. Note Use the SearchAreas property only for the configuration of the My DataFinder DataFinder. To configure a data indexing instance in SystemLink TDM, use the SystemLink TDM HTTP API. For a description of the SystemLink TDM HTTP API, see the SystemLink Help. |
| [`ITDMDataFinderStatistics.AnalyzedFiles`](itdmdatafinderstatistics-analyzedfiles.md) | Specifies the number of all the files indexed in the search areas, of which the file information was indexed, regardless of whether the associated DataPlugins can also read the channel information and the group information of the files. |
| [`ITDMDataFinderStatistics.IndexedChannels`](itdmdatafinderstatistics-indexedchannels.md) | Displays the number of channels which the DataFinder has indexed. |
| [`ITDMDataFinderStatistics.IndexedFiles`](itdmdatafinderstatistics-indexedfiles.md) | Specifies the number of indexed files whose associated DataPlugins can read in the group information and the channel information as well as the file information. |
| [`ITDMDataFinderStatistics.IndexedGroups`](itdmdatafinderstatistics-indexedgroups.md) | Displays the number of channel groups which the DataFinder has indexed. |
| [`ITDMDataFinderStatistics.IndexingComplete`](itdmdatafinderstatistics-indexingcomplete.md) | Displays whether the DataFinder has executed the indexing of the search area completely at least once. |
| [`ITDMDataFinderStatistics.IndexSize`](itdmdatafinderstatistics-indexsize.md) | Displays the size in kilobyte (kB) of the index which the DataFinder generated when indexing the search area. |
| [`ITDMDataFinderStatistics.LastCompleteIndexing`](itdmdatafinderstatistics-lastcompleteindexing.md) | Displays the date and time of the last complete indexing of the search area by the DataFinder. |
| [`ITDMDataFinderTextQuery.ReturnType`](itdmdatafindertextquery-returntype.md) | Specifies the search results type of a search in a data store. The search result of a quick search in a DataFinder is always a file type. |
| [`ITDMDataFinderTextQuery.Text`](itdmdatafindertextquery-text.md) | Specifies in a DataFinder the search text for the quick search. |
| [`ITDMDataStore.Model`](itdmdatastore-model.md) | Specifies the data model of the currently open data store. |
| [`ITDMDataStore.Name`](itdmdatastore-name.md) | Specifies the name of the data store currently open. |
| [`ITDMDataStore.Parameters`](itdmdatastore-parameters.md) | Specifies in a data store an XML string with the parameters which open the data store. |
| [`ITDMDataStore.PluginName`](itdmdatastore-pluginname.md) | Specifies the name of the DataPlugin with which DIAdem has opened a data store. |
| [`ITDMDataStore.Results`](itdmdatastore-results.md) | Use the new property ResultsElements instead of the Results property. |
| [`ITDMDataStore.ResultsElements`](itdmdatastore-resultselements.md) | Returns the search results of a search without user interface for elements in a data store. |
| [`ITDMDataStore.ResultsProperties`](itdmdatastore-resultsproperties.md) | Returns the results of a column-oriented search without the user interface in a data store. |
| [`ITDMDataStore.RootElements`](itdmdatastore-rootelements.md) | Returns the topmost data elements in a data store. |
| [`ITDMDataStoreAdvancedQuery.Conditions`](itdmdatastoreadvancedquery-conditions.md) | Specifies the search parameters for a search without the interface in a data store. |
| [`ITDMDataStoreAdvancedQuery.ReturnType`](itdmdatastoreadvancedquery-returntype.md) | Specifies the search results type in an advanced search in a data store. |
| [`ITDMDataStoreCondition.Name`](itdmdatastorecondition-name.md) | Specifies the name of a search condition in the search input area of a data store, for example, C1 or C2. |
| [`ITDMDataStoreCondition.Operator`](itdmdatastorecondition-operator.md) | Specifies the operator that DIAdem uses in a data store for a search condition. |
| [`ITDMDataStoreCondition.Property`](itdmdatastorecondition-property.md) | Specifies in a data store the property of a search condition. |
| [`ITDMDataStoreCondition.Size`](itdmdatastorecondition-size.md) | Returns in a search in a data store the number of values in a search condition that are connected with OR. |
| [`ITDMDataStoreCondition.Type`](itdmdatastorecondition-type.md) | Specifies the search condition type in a data store. The column Level contains the type of the search condition on the interface of the search input area. You can use the types TestBed , Test , Measurement , and MeaQuantity . |
| [`ITDMDataStoreCondition.Value`](itdmdatastorecondition-value.md) | Specifies the value that DIAdem searches for in a data store. |
| [`ITDMDataStoreCondition.Values`](itdmdatastorecondition-values.md) | Specifies in a data store a vector with values of a search condition. The size of the vector depends on the Size property. |
| [`ITDMDataStoreConditions.Count`](itdmdatastoreconditions-count.md) | Specifies in a data store the number of search conditions of a search. |
| [`ITDMDataStoreConditions.Logic`](itdmdatastoreconditions-logic.md) | Returns the logical operations of search conditions of a data store in the search input area. You can connect search conditions with AND and OR. Use parentheses to specify the order of evaluation. |
| [`ITDMDataStoreModel.Entities`](itdmdatastoremodel-entities.md) | Returns a collection of all the entities of a data store. |
| [`ITDMDataStoreModel.Enumerations`](itdmdatastoremodel-enumerations.md) | Specifies the enumerations in the model of a data store. |
| [`ITDMEnumerationItem.Definition`](itdmenumerationitem-definition.md) | Specifies the definition of an element in an enumeration in the model of a data store. |
| [`ITDMEnumerationItem.Value`](itdmenumerationitem-value.md) | Specifies the value of an element in an enumeration in the model of a data store. |
| [`ITDMEnumerationItems.Count`](itdmenumerationitems-count.md) | Specifies the number of elements in an enumeration in the model of a data store. |
| [`ITDMFreeDataFinderElementList.Count`](itdmfreedatafinderelementlist-count.md) | Returns in the DIAdem NAVIGATOR script interface the number of elements of a FreeElementList collection. |
| [`ITDMFreeStoreElementList.Count`](itdmfreestoreelementlist-count.md) | Returns in the DIAdem NAVIGATOR script interface the number of elements of a data store's FreeElementList collection. |
| [`ITDMIndexedProperties.Count`](itdmindexedproperties-count.md) | Specifies in a DataFinder the number of indexed properties and custom properties of files, of groups, and of channels. |
| [`ITDMIndexedProperty.DataType`](itdmindexedproperty-datatype.md) | Specifies in a DataFinder the data type of a property or a custom property. |
| [`ITDMIndexedProperty.Default`](itdmindexedproperty-default.md) | Specifies in a DataFinder whether a property is a default property or a custom property. The Default property returns the value TRUE if the property is a default property. |
| [`ITDMIndexedProperty.DisplayName`](itdmindexedproperty-displayname.md) | Specifies in a DataFinder the display name of a Property or custom property. |
| [`ITDMIndexedProperty.Name`](itdmindexedproperty-name.md) | Specifies in a DataFinder the name of an indexed property or a custom property. |
| [`ITDMIndexedValueLimits.Max`](itdmindexedvaluelimits-max.md) | Specifies in a DataFinder the largest indexed value of a property. |
| [`ITDMIndexedValueLimits.Min`](itdmindexedvaluelimits-min.md) | Specifies in a DataFinder the smallest indexed value of a property. |
| [`ITDMIndexedValueList.Count`](itdmindexedvaluelist-count.md) | Specifies in a DataFinder the number of indexed values of a text property or of an optimized custom property which is a text type. |
| [`ITDMIndexedValueList.IsIncomplete`](itdmindexedvaluelist-isincomplete.md) | Specifies in a DataFinder whether the list of indexed values returned by the ValueList object is complete. |
| [`ITDMIndexedValueList.Values`](itdmindexedvaluelist-values.md) | Specifies in a DataFinder the value with the specified index from the value list of an indexed property or an optimized custom property. |
| [`ITDMModelEntities.Count`](itdmmodelentities-count.md) | Specifies in a data store the number of data model entities. |
| [`ITDMModelEntity.ModelProperties`](itdmmodelentity-modelproperties.md) | Returns in a data store the properties of an entity of the data model. |
| [`ITDMModelEntity.ModelReferences`](itdmmodelentity-modelreferences.md) | Returns the model references of an entity of the data model in a data store. |
| [`ITDMModelEntity.Name`](itdmmodelentity-name.md) | Specifies in a data store the name of an entity. |
| [`ITDMModelEntity.SubTypes`](itdmmodelentity-subtypes.md) | Returns the entities that are derived from the current entity. |
| [`ITDMModelEntity.SuperType`](itdmmodelentity-supertype.md) | Specifies the entity from which the current entity is derived. |
| [`ITDMModelEnumeration.Items`](itdmmodelenumeration-items.md) | Returns an element of a enumeration in the model of a data store. |
| [`ITDMModelEnumeration.Name`](itdmmodelenumeration-name.md) | Returns the name of an element of an enumeration in the model of a data store. |
| [`ITDMModelEnumerationProperty.BaseName`](itdmmodelenumerationproperty-basename.md) | Specifies in the data model of a data store the base name of an enumeration property. |
| [`ITDMModelEnumerationProperty.DataType`](itdmmodelenumerationproperty-datatype.md) | Specifies in a data store the data type of an enumeration property of the data model. |
| [`ITDMModelEnumerationProperty.Enumeration`](itdmmodelenumerationproperty-enumeration.md) | Returns an enumeration property in the data model of a data store. |
| [`ITDMModelEnumerationProperty.MaxOccur`](itdmmodelenumerationproperty-maxoccur.md) | Specifies in a data store the maximum number of values an enumeration property may contain. Note The MinOccur property specifies the minimum number of values a property must contain. If MinOccur , for example, has the value 0 and MaxOccur has the value 1, the property may have a maximum value of 1 or no value. If MinOccur and MaxOccur have the value 1, the property must have exactly one value. If MinOccur has the value 1 and MaxOccur the value MaxInt , the property must have at least one value but can also have any number of values. |
| [`ITDMModelEnumerationProperty.MinOccur`](itdmmodelenumerationproperty-minoccur.md) | Specifies in a data store the minimum number of values an enumeration property must contain. Note The MaxOccur property specifies the maximum number of values a property may contain. If MinOccur , for example, has the value 0 and MaxOccur has the value 1, the property may have a maximum value of 1 or no value. If MinOccur and MaxOccur have the value 1, the property must have exactly one value. If MinOccur has the value 1 and MaxOccur the value MaxInt , the property must have at least one value but can also have any number of values. |
| [`ITDMModelEnumerationProperty.Name`](itdmmodelenumerationproperty-name.md) | Specifies the name of an enumeration property in an entity of the data model. |
| [`ITDMModelEnumerations.Count`](itdmmodelenumerations-count.md) | Specifies the number of enumerations in the model of a data store. |
| [`ITDMModelProperties.Count`](itdmmodelproperties-count.md) | Specifies in a data store the number of properties of a data model entity. |
| [`ITDMModelProperty.BaseName`](itdmmodelproperty-basename.md) | Specifies in the data model of a data store the base name of a property. |
| [`ITDMModelProperty.DataType`](itdmmodelproperty-datatype.md) | Specifies in a data store the data type of a data model property. |
| [`ITDMModelProperty.MaxOccur`](itdmmodelproperty-maxoccur.md) | Specifies in a data store the maximum number of values a property may contain. |
| [`ITDMModelProperty.MinOccur`](itdmmodelproperty-minoccur.md) | Specifies in a data store the minimum number of values a property must contain. |
| [`ITDMModelProperty.Name`](itdmmodelproperty-name.md) | Specifies the name of an entity property of the data model. |
| [`ITDMModelReference.BaseName`](itdmmodelreference-basename.md) | Specifies in a data store the base name of the model reference of an entity. |
| [`ITDMModelReference.EntityType`](itdmmodelreference-entitytype.md) | Returns the type of a model reference, in a data store. |
| [`ITDMModelReference.Inverse`](itdmmodelreference-inverse.md) | Specifies in a data store the inverse reference of a model reference. |
| [`ITDMModelReference.MaxOccur`](itdmmodelreference-maxoccur.md) | Specifies in a data store the maximum number of values an entity may reference for a certain reference. |
| [`ITDMModelReference.MinOccur`](itdmmodelreference-minoccur.md) | Specifies in a data store the minimum number of values the reference of an entity must contain. |
| [`ITDMModelReference.Name`](itdmmodelreference-name.md) | Specifies in a data store the name of the model reference of an entity. |
| [`ITDMModelReferences.Count`](itdmmodelreferences-count.md) | Specifies in a data store the number of references of a data model entity. |
| [`ITDMModelStandardProperty.BaseName`](itdmmodelstandardproperty-basename.md) | Specifies in the data model of a data store the base name of a standard property. |
| [`ITDMModelStandardProperty.DataType`](itdmmodelstandardproperty-datatype.md) | Specifies in a data store the data type of a standard property of the data model. |
| [`ITDMModelStandardProperty.MaxOccur`](itdmmodelstandardproperty-maxoccur.md) | Specifies in a data store the maximum number of values a standard property may contain. Note The MinOccur property specifies the minimum number of values a property must contain. If MinOccur , for example, has the value 0 and MaxOccur has the value 1, the property may have a maximum value of 1 or no value. If MinOccur and MaxOccur have the value 1, the property must have exactly one value. If MinOccur has the value 1 and MaxOccur the value MaxInt , the property must have at least one value but can also have any number of values. |
| [`ITDMModelStandardProperty.MinOccur`](itdmmodelstandardproperty-minoccur.md) | Specifies in a data store the minimum number of values a standard property must contain. Note The MaxOccur property specifies the maximum number of values a property may contain. If MinOccur , for example, has the value 0 and MaxOccur has the value 1, the property may have a maximum value of 1 or no value. If MinOccur and MaxOccur have the value 1, the property must have exactly one value. If MinOccur has the value 1 and MaxOccur the value MaxInt , the property must have at least one value but can also have any number of values. |
| [`ITDMModelStandardProperty.Name`](itdmmodelstandardproperty-name.md) | Specifies the name of a standard property in an entity of the data model. |
| [`ITDMResultsDisplayCellsSelection.Count`](itdmresultsdisplaycellsselection-count.md) | Specifies the number of cells selected in the search results list of a DataFinder or of a data store. |
| [`ITDMResultsDisplayColumnsSelection.Count`](itdmresultsdisplaycolumnsselection-count.md) | Specifies the number of columns selected in a search results list of a DataFinder or a data store. |
| [`ITDMResultsDisplaySettings.ColumnHeaderDisplayMode`](itdmresultsdisplaysettings-columnheaderdisplaymode.md) | Specifies whether DIAdem displays the names of the layers and the associated properties in the column header of the search result list or whether DIAdem hides the layers and only displays the properties. |
| [`ITDMResultsDisplaySettings.Columns`](itdmresultsdisplaysettings-columns.md) | Specifies in a search in DIAdem NAVIGATOR the property columns to be displayed for the different result types. |
| [`ITDMResultsDisplaySettings.DetermineColumnsAutomatically`](itdmresultsdisplaysettings-determinecolumnsautomatically.md) | Specifies whether DIAdem automatically adds columns to the search results in an advanced search, with the properties that you searched for. |
| [`ITDMResultsDisplaySettings.MaxCount`](itdmresultsdisplaysettings-maxcount.md) | Specifies in an interface search in the DataFinder the maximum number of search results the search returns. |
| [`ITDMResultsProperties.Count`](itdmresultsproperties-count.md) | Specifies the number of properties in the search results of a column-oriented search. |
| [`ITDMResultsProperties.IsIncomplete`](itdmresultsproperties-isincomplete.md) | Specifies whether the search results list of a column-oriented search contains all properties. If the IsIncomplete property has the value TRUE , the search has more results than the MaxCount property specifies. You only can use the IsIncomplete property if the ResultsProperties object contains search results. |
| [`ITDMResultsProperties.MaxCount`](itdmresultsproperties-maxcount.md) | Specifies in a column-oriented search the maximum number of search results which DIAdem determines for a specific property. |
| [`ITDMResultsProperties.ResultsCount`](itdmresultsproperties-resultscount.md) | Specifies the number of search results for a particular property in a column-oriented search. |
| [`ITDMResultsProperties.ReturnType`](itdmresultsproperties-returntype.md) | Specifies in a column-oriented search the return type of the property values in the search result. |
| [`ITDMResultsProperty.DataType`](itdmresultsproperty-datatype.md) | Specifies in a column-oriented search the data type of a property in the search results. Note DIAdem automatically specifies the data type of base properties and optimized custom properties. Use the Add method to specify the data type of non-optimized custom properties. |
| [`ITDMResultsProperty.Property`](itdmresultsproperty-property.md) | Specifies in a column-oriented search the name of a property in a column of the search results. |
| [`ITDMResultsProperty.Size`](itdmresultsproperty-size.md) | Specifies how often a property occurs in the search result of a column-oriented search. |
| [`ITDMResultsProperty.Type`](itdmresultsproperty-type.md) | Specifies in a column-oriented search the type of a plane from which the property originates in the search result. Planes can be Root , Group , or Channel types. |
| [`ITDMReturnTypeColumns.Count`](itdmreturntypecolumns-count.md) | Determines the number of columns that DIAdem-NAVIGATOR displays in the search result list of a search in a data store. |
| [`ITDMStoreElement.Children`](itdmstoreelement-children.md) | Returns the subordinate elements of an Element in a data store. |
| [`ITDMStoreElement.DisplayName`](itdmstoreelement-displayname.md) | Specifies in a data store the display name of an element. |
| [`ITDMStoreElement.InstanceKey`](itdmstoreelement-instancekey.md) | Specifies in a data store the instance key of a data element. |
| [`ITDMStoreElement.Name`](itdmstoreelement-name.md) | Specifies in a data store the name of a data element. |
| [`ITDMStoreElement.Parent`](itdmstoreelement-parent.md) | Returns the superordinate element of a data element in a data store. Use the Parent property to navigate from the measurement quantities to the root element. |
| [`ITDMStoreElement.Properties`](itdmstoreelement-properties.md) | Returns the properties of a data element in a data store. |
| [`ITDMStoreElement.References`](itdmstoreelement-references.md) | Returns the references to other data elements in a data store. |
| [`ITDMStoreElement.Type`](itdmstoreelement-type.md) | Specifies in a data store the type of a data element. |
| [`ITDMStoreElementList.Count`](itdmstoreelementlist-count.md) | Specifies in a data store the number of elements of an ElementList collection. |
| [`ITDMStoreElementList.IsIncomplete`](itdmstoreelementlist-isincomplete.md) | Specifies in a data store whether the list of elements which the ElementList object returns is complete. If the IsIncomplete property has the value TRUE , there are more search results than the MaxCount property specifies. You only can use the IsIncomplete property if the ElementList object contains search results. |
| [`ITDMStoreElementList.MaxCount`](itdmstoreelementlist-maxcount.md) | Specifies in a data store the maximum number of elements that the ElementList collection can contain. |
| [`ITDMStoreElements.Count`](itdmstoreelements-count.md) | Specifies in a data store the number of elements of an Elements collection. |
| [`ITDMStoreElementWithBulk.Children`](itdmstoreelementwithbulk-children.md) | Returns the subordinate elements of a data element in a data store. Use the Children property to navigate from the root element to the measurement quantities. |
| [`ITDMStoreElementWithBulk.DataType`](itdmstoreelementwithbulk-datatype.md) | Specifies in a data store the data type of a LocalColumn. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types. |
| [`ITDMStoreElementWithBulk.DisplayName`](itdmstoreelementwithbulk-displayname.md) | Specifies in a data store the display name of a data element. |
| [`ITDMStoreElementWithBulk.Flags`](itdmstoreelementwithbulk-flags.md) | Specifies in a data store a vector with the flags that correspond to Values . Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types. |
| [`ITDMStoreElementWithBulk.InstanceKey`](itdmstoreelementwithbulk-instancekey.md) | Specifies in a data store the instance key of a data element. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types. |
| [`ITDMStoreElementWithBulk.Name`](itdmstoreelementwithbulk-name.md) | Specifies in a data store the name of a data element. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types. |
| [`ITDMStoreElementWithBulk.Parent`](itdmstoreelementwithbulk-parent.md) | Returns the superordinate element of a data element in a data store. Use the Parent property to navigate from the measurement quantities to the root element. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types. |
| [`ITDMStoreElementWithBulk.Properties`](itdmstoreelementwithbulk-properties.md) | Returns the properties of a data element in a data store. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types. |
| [`ITDMStoreElementWithBulk.References`](itdmstoreelementwithbulk-references.md) | Returns the references to other data elements in a data store. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types. |
| [`ITDMStoreElementWithBulk.Size`](itdmstoreelementwithbulk-size.md) | Specifies in a data store the number of values in the value vector of a LocalColumn. DIAdem automatically adjusts the number of values to the number of values of the associated submatrix. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types. |
| [`ITDMStoreElementWithBulk.Type`](itdmstoreelementwithbulk-type.md) | Specifies in a data store the type of a data element. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types. |
| [`ITDMStoreElementWithBulk.Values`](itdmstoreelementwithbulk-values.md) | Specifies in a data store the value vector of a LocalColumn. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types. |
| [`ITDMStoreProperties.Count`](itdmstoreproperties-count.md) | Specifies in a data store the number of properties of a data element. |
| [`ITDMStoreProperties.ListInstanceProperties`](itdmstoreproperties-listinstanceproperties.md) | Specifies in a data store whether the collection of properties of a data element also contains instance properties. If you assign the value TRUE to the ListInstanceProperties property, you can create new instance properties and delete existing instance properties. |
| [`ITDMStoreProperty.BaseName`](itdmstoreproperty-basename.md) | Specifies in a data store the base name of a property. |
| [`ITDMStoreProperty.DataType`](itdmstoreproperty-datatype.md) | Specifies in a data store the data type of a property. |
| [`ITDMStoreProperty.Name`](itdmstoreproperty-name.md) | Specifies in a data store the name of a property. |
| [`ITDMStoreProperty.Size`](itdmstoreproperty-size.md) | Specifies in a data store the number of values of a property. |
| [`ITDMStoreProperty.Value`](itdmstoreproperty-value.md) | Specifies in a data store the value of a property of a data element. |
| [`ITDMStoreProperty.Values`](itdmstoreproperty-values.md) | Specifies in a data store a vector with values of a property. |
| [`ITDMStoreReference.BaseName`](itdmstorereference-basename.md) | Specifies in a data storage the base name of the reference of an Element object. |
| [`ITDMStoreReference.Elements`](itdmstorereference-elements.md) | Specifies in a data store the referenced data elements. |
| [`ITDMStoreReference.Name`](itdmstorereference-name.md) | Specifies in a data store the name of a reference of a data element. |
| [`ITDMStoreReferences.Count`](itdmstorereferences-count.md) | Specifies in a data store the number of references of a References collection. |
| [`ITDMTimeDisp.Day`](itdmtimedisp-day.md) | Specifies the day in a UsiTimeDisp type object. |
| [`ITDMTimeDisp.Fraction`](itdmtimedisp-fraction.md) | Specifies in an USITimeDisp type object the fractions of a second with an accuracy of nanoseconds. |
| [`ITDMTimeDisp.Hour`](itdmtimedisp-hour.md) | Specifies the hours in a UsiTimeDisp type object. |
| [`ITDMTimeDisp.Microsecond`](itdmtimedisp-microsecond.md) | Specifies the microseconds in a UsiTimeDisp type object. |
| [`ITDMTimeDisp.MilliSecond`](itdmtimedisp-millisecond.md) | Specifies the milliseconds in a UsiTimeDisp type object. |
| [`ITDMTimeDisp.Minute`](itdmtimedisp-minute.md) | Specifies the minutes in a UsiTimeDisp type object. |
| [`ITDMTimeDisp.Month`](itdmtimedisp-month.md) | Specifies the month in a UsiTimeDisp type object. |
| [`ITDMTimeDisp.Nanosecond`](itdmtimedisp-nanosecond.md) | Specifies the nanoseconds in a UsiTimeDisp type object. |
| [`ITDMTimeDisp.Second`](itdmtimedisp-second.md) | Specifies the seconds in a UsiTimeDisp type object. |
| [`ITDMTimeDisp.SecondsFrom0000`](itdmtimedisp-secondsfrom0000.md) | Specifies in a USITimeDisp type object the seconds since 00:00:00 o'clock on 01/01/0000. |
| [`ITDMTimeDisp.SecondsFrom1904`](itdmtimedisp-secondsfrom1904.md) | Specifies in a USITimeDisp type object the seconds since 00:00:00 o'clock on 1/1/1904. |
| [`ITDMTimeDisp.VariantDate`](itdmtimedisp-variantdate.md) | Specifies a date/time in the VBS date format. This entry does not include microseconds and nanoseconds. |
| [`ITDMTimeDisp.Year`](itdmtimedisp-year.md) | Specifies the year in a UsiTimeDisp type object. |
| [`IUpdateData.Count`](iupdatedata-count.md) | Specifies the number of DataPlugins available in the update source. |
| [`IUpdateDataDataPlugin.Description`](iupdatedatadataplugin-description.md) | Specifies the description of DataPlugins available in the update source. |
| [`IUpdateDataDataPlugin.FileExtensionList`](iupdatedatadataplugin-fileextensionlist.md) | Specifies the list with filename extensions of DataPlugins available in the update source. DIAdem loads files with these filename extensions with the respective DataPlugin. |
| [`IUpdateDataDataPlugin.Name`](iupdatedatadataplugin-name.md) | Specifies the name of a DataPlugin available in the update source. |
| [`IUpdateDataDataPlugin.Type`](iupdatedatadataplugin-type.md) | Specifies the DataPlugin type. |
| [`IUpdateDataDataPlugin.URL`](iupdatedatadataplugin-url.md) | Specifies the URL of a DataPlugin in the update source. |
| [`IUpdateDataDataPlugin.Version`](iupdatedatadataplugin-version.md) | Specifies the version number of a DataPlugin in the update source. |
| [`IUpdateSource.LastUpdate`](iupdatesource-lastupdate.md) | Specifies when the information about DataPlugins available in the update source was updated last. |
| [`IUpdateSource.Parameter`](iupdatesource-parameter.md) | Specifies the name of the DataFinder instance which you use as the source to update your local Data Plugins. |
| [`IUpdateSource.Type`](iupdatesource-type.md) | Specifies with which update source you synchronize your local DataPlugins. |
| [`IUpdateSource.UpdateData`](iupdatesource-updatedata.md) | Specifies the DataPlugins available in the update source. |
| [`IValueMapper.Mappings`](ivaluemapper-mappings.md) | Returns the collection of mappings of the file level (eSearchFile), channel group (eSearchChannelGroup), and channel (eSearchChannel), when mapping the values of a property. |
| [`IValueMapper.SeparatorList`](ivaluemapper-separatorlist.md) | Specifies an array with a separator which can be used when using a mapping rule, when mapping property values in the data preparation. This array is only for depositing the separator sign in the script API. |
| [`IValueMapping.PropertyName`](ivaluemapping-propertyname.md) | Specifies the name of the property for which you created a mapping, when mapping values of a property. |
| [`IValueMapping.Rules`](ivaluemapping-rules.md) | Specifies the collection of rules DIAdem uses to replace the values of a property, when mapping values of a property. |
| [`IValueMappings.Count`](ivaluemappings-count.md) | Returns the number of mappings defined for a level, when mapping the values of a property. A level can be a file (eSearchFile), a channel group (eSearchChannelGroup), or a channel (eSearchChannel). |
| [`IValueMappings.EntityName`](ivaluemappings-entityname.md) | Returns the name of the associated level, when mapping the values of a property. A level can be a file (eSearchFile), a channel group (eSearchChannelGroup), or a channel (eSearchChannel). |
| [`IValueRule.Example`](ivaluerule-example.md) | Specifies an example text with which DIAdem can check a defined rule when mapping values of a property. |
| [`IValueRule.Pattern`](ivaluerule-pattern.md) | Specifies the search pattern of the Regular expression which DIAdem uses for a rule, when mapping values of a property. In addition to the Regular expressions of VBS, you can also use the ECMAScript syntax, for example ([[:alpha:]]+)([_\.;]+)([[:digit:]]+) . |
| [`IValueRule.Schema`](ivaluerule-schema.md) | Specifies the replacement pattern according to which DIAdem replaces property values, when mapping the values of a property. The replacement patter may contain $ expressions and text. If the search pattern contains expressions in parentheses, you access the content of the parentheses with the $ expression in the replacement pattern. The regular expression saves the contents of the parenthesis according to their order in the expressions $1 , $2 , ... . For example, in the replacement pattern of the regular expression ([[:alpha:]]+)([_\.;]+)([[:digit:]]+) , the expression $1 contains the contents of the expression ([[:alpha:]]+) , $2 contains the contents of the expression ([_\.;]+) , and $3 contains the contents of the expression ([[:digit:]]+) . You can change the order of the $-expressions in the replacement pattern and additionally insert free text, for example "$1 AnyText $3$2” . Note Use Regular expressions to define search patterns. Besides the regular expressions of VBS, you can also use the ECMAScript syntax, for example ([[:alpha:]]+)([_\.;]+)([[:digit:]]+) . |
| [`IValueRules.Count`](ivaluerules-count.md) | Returns the number of rules defined for this property, when mapping the values of a property. |
