---
title: "Objects (NAVIGATOR / Data Portal / Data Finder)"
---

# Objects

77 objects from `ScriptNavi.chm`.

| Name | Summary |
| --- | --- |
| [`ICommonExportParameter`](icommonexportparameter.md) | The CommonExportParameter <Navigator> object provides the properties and methods for configuring the export of data with a specified DataPlugin. |
| [`ICSVExportParameter`](icsvexportparameter.md) | The CSVExportParameter <Navigator> object provides the properties and methods for parameterizing the export of data with the CSV_Export DataPlugin. |
| [`IDataFileHeaderAccess`](idatafileheaderaccess.md) | The DataFileHeaderAccess object provides access to an ASAM data store, which you can use to read, write, modify, or delete channel properties, group properties, or file properties from TDM files or TDMS files. |
| [`IDataFinderCell`](idatafindercell.md) | In a DataFinder the Cell object provides a cell of the search results list. |
| [`IDataFinderDisplay`](idatafinderdisplay.md) | The Display provides an open DataFinder. You can run a Quick search and an Advanced search with a DataFinder. You run the search on the DIAdem NAVIGATOR interface. To execute a search, enter the search conditions ( Conditions ) into the search input area ( QueryForm ). Use the ResultsList property to access the results of a search. |
| [`IDataFinderQuery`](idatafinderquery.md) | The Query provides a search object in a DataFinder. You can use this search object for a Search with the interface of DIAdem NAVIGATOR and for a Search without the interface . You can run a Quick search and an Advanced search with this search object. |
| [`IDataPluginParameter`](idatapluginparameter.md) | The DataPluginParameter <Navigator> object provides the properties and methods for configuring the export of data with a selected DataPlugin. DIAdem only creates the object if a DataPluginParameter object exists for the specified DataPlugin. |
| [`IDataProvider`](idataprovider.md) | The CurrDataProvider object provides the current data store or DataFinder and includes the joint methods and properties of CurrDataFinder and CurrDataStore . |
| [`IDataStoreBaseQuery`](idatastorebasequery.md) | The Query object provides a search object in a data store. You can use this search object for a Search with the interface of DIAdem NAVIGATOR and for a Search without the interface . You can run a Quick search and an Advanced search with this search object. You can only run a quick search in a data store if you access a DataFinder instance which is declared as an ASAM ODS server. The Query object corresponds to one of the following objects: AdvancedQuery (ITDMDataStoreAdvancedQuery) Advanced Search TextQuery (IDataStoreTextQuery) Quick Search |
| [`IDataStoreCell`](idatastorecell.md) | In a DataFinder the Cell object provides a cell of the search results list. |
| [`IDataStoreDisplay`](idatastoredisplay.md) | The Display object provides an open data store in DIAdem NAVIGATOR. You run the search on the DIAdem NAVIGATOR interface. To execute a search, enter the search conditions ( Conditions ) into the search input area ( QueryForm ). Use the ResultsList property to access the results of a search. |
| [`IDataStoreTextQuery`](idatastoretextquery.md) | The TextQuery object provides the properties for a quick search in a data store. If you execute a quick search, DIAdem searches to the specified value in all properties. You can only run a quick search in a data store if you access a DataFinder instance which is declared as an ASAM ODS server. |
| [`IDisplay`](idisplay.md) | The Display object provides the methods and properties of the DIAdem NAVIGATOR interface. You can use the object Display for the DataFinder and for data stores. |
| [`IEvents`](ievents.md) | The Events object combines the user commands assigned to the events in DIAdem NAVIGATOR. The properties of the Events object contain the names of the user commands that DIAdem calls when the associated event occurs. |
| [`IImportParameterSet`](iimportparameterset.md) | The ImportParameter <Navigator> object provides all properties for the import of data in DIAdem. Note You can use the Import parameter <Navigator>Object as a parameter in the following commands and methods: DataFileLoad , DataFileLoadSel , Navigator . LoadData , navigator . LoadProperty and StorageImport . |
| [`INaviDataFinderBrowser`](inavidatafinderbrowser.md) | The Browser object provides the file browser of a DataFinder. You also can use the file browser to browse in files. |
| [`INaviDataFinderQueryForm`](inavidatafinderqueryform.md) | The QueryForm object provides the search input area of a DataFinder. Use the Search method for the current search. The Search Results contains the results of the search. |
| [`INaviDataFinderResultDisplay`](inavidatafinderresultdisplay.md) | The ResultsList object provides the results of an interface search in a DataFinder. |
| [`INaviDataStoreBrowser`](inavidatastorebrowser.md) | The Browser object provides the data browser of a data store. You can use the data browser to navigate tests, SubTests, measurements, and measurement quantities. |
| [`INaviDataStoreQueryForm`](inavidatastorequeryform.md) | The QueryForm object provides the search input area of a data store in DIAdem NAVIGATOR. Use the Search method for the current search. The ResultsList object contains the results of a search. |
| [`INaviDataStoreResultDisplay`](inavidatastoreresultdisplay.md) | The ResultsList object provides the results of a search in a data store on the DIAdem NAVIGATOR interface. |
| [`INavigator`](inavigator.md) | The Navigator object enables access to the interface and the functions of DIAdem NAVIGATOR. Use the Navigator object to open data stores and DataFinders. You can search for properties of files, channel groups, and channels in DataFinders and search for properties of tests, subtests, measurements, and measurement quantities in data stores. You can display the search results and load the results directly into the Data Portal. |
| [`INavigatorSettings`](inavigatorsettings.md) | The Settings object provides access to general settings in DIAdem NAVIGATOR. |
| [`IPropertyHandling`](ipropertyhandling.md) | The PropertyHandling <Navigator> object specifies how DIAdem handles properties when importing data. |
| [`IPropertyImportProperty`](ipropertyimportproperty.md) | The ImportProperty object displays an element of a Loading configuration of data stores . |
| [`IPropertyImportSet`](ipropertyimportset.md) | The PropertyImportSet object displays the Loading configuration of a data store. |
| [`IRegisteredDataPlugin`](iregistereddataplugin.md) | The RegisteredDataPlugin object provides information about a DataPlugin registered on your computer. |
| [`IRegisteredDataStore`](iregistereddatastore.md) | The RegisteredDataStore object provides the connection definition of a data store registered on your computer. |
| [`IResultsDisplaySelection`](iresultsdisplayselection.md) | The Selection object provides the rows ( ElementsSelection <DataFinder> , ElementsSelection <DataStore> ), cells ( CellsSelection ), or columns ( ColumnsSelection ) selected in the search results list of a DataFinder or of a data store. |
| [`ISUSIChannel`](isusichannel.md) | The Channel object provides a channel in a DataFinder. Thus the Element object is a channel. |
| [`ISUSIChannelGroup`](isusichannelgroup.md) | The ChannelGroup object provides a channel group in a DataFinder. Thus the Element object is a channel group. |
| [`ISUSIElement`](isusielement.md) | The Element object provides a single element of the search results or of the file browser in a DataFinder. The elements can be files, groups, or channels. |
| [`ISUSIProperty`](isusiproperty.md) | The Property object provides in a DataFidner a property for the Root object , the ChannelGroup object , or the Channel object . |
| [`ISUSIRoot`](isusiroot.md) | The Root object provides a file in a DataFinder. Thus the Element object is a file. |
| [`ITDMBrowseEntity`](itdmbrowseentity.md) | In a DataFinder the BrowseEntity object provides an entity of the Browse path . |
| [`ITDMBrowseSettings`](itdmbrowsesettings.md) | The browse settings object provides the Browse Settings for a data store. Browse settings have the filename extension *.tbs . |
| [`ITDMCell`](itdmcell.md) | The Cell object provides a cell of the search results in a DataFinder or a data store. |
| [`ITDMColumn`](itdmcolumn.md) | In the search results list of a DataFinder or of a data store the Column object provides a column with properties. If you run an advanced search, DIAdem automatically adds columns with the properties that you searched for. Select Configure Search Results List from the context menu of the search results list to manually add further columns with properties. You only can remove columns which were added manually. |
| [`ITDMContextParameter`](itdmcontextparameter.md) | The Context Parameter object provides a context parameter. Use the Context . GetParameter method to read context parameters from an ASAM server. Use the Context . SetParameter method to write context parameters to an ASAM server. Use the Context . SetParameters method to write all context parameters of a Parameter set to an ASAM server. |
| [`ITDMContextParameterSet`](itdmcontextparameterset.md) | The ContextParameterSet object provides a set of context parameters. Use the Context . SetParameters method to write all context parameters of a Parameter set to an ASAM server. |
| [`ITDMDataFinder`](itdmdatafinder.md) | The DataFinder object provides a DataFinder without using the DIAdem NAVIGATOR interface. You can run a Quick search and an Advanced search with the DataFinder object. Use the properties ResultsElements and ResultsProperties to access the search results. |
| [`ITDMDataFinderAdvancedQuery`](itdmdatafinderadvancedquery.md) | The AdvancedQuery object provides the properties of an Advanced search in a DataFinder. If you run an advanced search, DIAdem searches for the property values of the files, groups, or channels that you selected. |
| [`ITDMDataFinderCondition`](itdmdatafindercondition.md) | The Condition object provides a row of the search parameters with a DataFinder for the advanced search. |
| [`ITDMDataFinderExcludeFolder`](itdmdatafinderexcludefolder.md) | In a DataFinder configuration the ExcludeFolder object provides a folder in a search area. The DataFinder excludes the folder from the search. |
| [`ITDMDataFinderIndexer`](itdmdatafinderindexer.md) | The Indexer object provides the methods which you use to reindex files and folders of the My DataFinder DataFinder. You cannot use the indexer object for DataFinders that are located on another host. |
| [`ITDMDataFinderIndexerSchedule`](itdmdatafinderindexerschedule.md) | The IndexerSchedule object provides the settings for the indexer schedule in a DataFinder configuration. |
| [`ITDMDataFinderSearchArea`](itdmdatafindersearcharea.md) | The SearchArea object provides a search area in a DataFinder configuration. |
| [`ITDMDataFinderSettings`](itdmdatafindersettings.md) | The DataFinderSettings object provides a DataFinder configuration. You use the DataFinderSettings object to create and to delete search areas, and folders that are to be excluded from the search, to optimize custom properties, and to import and export DataFinder configurations. You only can use the DataFinderSettings object for the My DataFinder DataFinder. |
| [`ITDMDataFinderStatistics`](itdmdatafinderstatistics.md) | The DataFinderStatistics object provides the index status of the DataFinder. |
| [`ITDMDataFinderTextQuery`](itdmdatafindertextquery.md) | The TextQuery object provides the properties for a quick search in a DataFinder. If you run a quick search, DIAdem searches all the properties of the files, groups, and channels from the search areas for the specified value. |
| [`ITDMDataStore`](itdmdatastore.md) | The DataStore object provides an ASAM data store without using the DIAdem NAVIGATOR interface. Note Use the DataStoreDisplay object to execute an interface search in the Navigator. |
| [`ITDMDataStoreAdvancedQuery`](itdmdatastoreadvancedquery.md) | The AdvancedQuery object provides the properties of an Advanced search in a data store. If you execute an advanced search, DIAdem searches for the values of the selected properties in the specified levels. Note If you enter parameters for an advanced search in the DIAdem NAVIGATOR interface and press <Ctrl-Shift-C>, DIAdem saves a script for the use of the AdvancedQuery object to the clipboard. |
| [`ITDMDataStoreCondition`](itdmdatastorecondition.md) | The Condition object provides a row of the search parameters in a search in a data store. |
| [`ITDMDataStoreContext`](itdmdatastorecontext.md) | The context object manages the context parameters of a data store on an ASAM server. Use the Context . GetParameter method to read context parameters from an ASAM server. Use the Context . SetParameter method to write context parameters to an ASAM server. Use the Context . SetParameters method to write all context parameters of a Parameter set to an ASAM server. |
| [`ITDMDataStoreModel`](itdmdatastoremodel.md) | The DataStoreModel object provides the entities and properties of a data model. You only can access the data model properties read only. |
| [`ITDMEnumerationItem`](itdmenumerationitem.md) | The EnumerationItem object provides an element of an enumeration in the model of a data store. |
| [`ITDMIndexedProperty`](itdmindexedproperty.md) | The IndexedProperty object provides a property or a custom property, that is indexed by the DataFinder. |
| [`ITDMIndexedValueLimits`](itdmindexedvaluelimits.md) | Returns in a DataFinder the indexed value range for a property , or for an optimized custom property that is an integer or numeric data type, or for a date/time property. |
| [`ITDMIndexedValueList`](itdmindexedvaluelist.md) | Provides the list with the indexed values for a text- property or an optimized text custom property in a DataFinder or a data store. |
| [`ITDMModelEntity`](itdmmodelentity.md) | The Entity object provides an entity of the data model. |
| [`ITDMModelEnumeration`](itdmmodelenumeration.md) | The ModelEnumeration object provides an enumeration in the model of a data store. |
| [`ITDMModelEnumerationProperty`](itdmmodelenumerationproperty.md) | The ModelEnumerationProperty object provides the enumeration property of an entity in the data model of a data store. |
| [`ITDMModelProperty`](itdmmodelproperty.md) | The ModelProperty object provides the property of a ModelEntity . You can read only the properties of an entity. |
| [`ITDMModelReference`](itdmmodelreference.md) | The ModelReference provides the ModelEntity reference in a data store. |
| [`ITDMModelStandardProperty`](itdmmodelstandardproperty.md) | The ModelStandardProperty object provides the standard property of an entity in the data model of a data store. |
| [`ITDMResultsDisplaySettings`](itdmresultsdisplaysettings.md) | The ResultsListSettings object provides the settings of the search results list in a DataFinder or in a data store. |
| [`ITDMResultsProperty`](itdmresultsproperty.md) | The ResultsProperty object provides a column with properties in the search results list of a column-oriented search. |
| [`ITDMStoreElement`](itdmstoreelement.md) | The Element object provides a data element in a data store. A data element is a specific instance of an entity. |
| [`ITDMStoreElementWithBulk`](itdmstoreelementwithbulk.md) | The ElementWithValues object provides a data element in a data store for accessing bulk data. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types. |
| [`ITDMStoreProperty`](itdmstoreproperty.md) | The Property object provides in a data store the property of a data element. |
| [`ITDMStoreReference`](itdmstorereference.md) | The Reference object provides a reference of an Element object in a data store. |
| [`ITDMTimeDisp`](itdmtimedisp.md) | The USITimeDisp object provides date and time information. |
| [`IUpdateDataDataPlugin`](iupdatedatadataplugin.md) | You can use the UpdateDataDataPlugin object to access information about a DataPlugin in the update source. |
| [`IUpdateSource`](iupdatesource.md) | Use the UpdateSource object to access general information about DataPlugins on the NI DataPlugin website or on a DataFinder instance. |
| [`IValueMapper`](ivaluemapper.md) | The PropertyValueMapper object provides the mapping of property values in the data preparation. |
| [`IValueMapping`](ivaluemapping.md) | The PropertyValueMapping mapping combines all rule for mapping a property in the data preparation. |
| [`IValueRule`](ivaluerule.md) | The ValueRule object provides a rule for mapping values of a property. |
