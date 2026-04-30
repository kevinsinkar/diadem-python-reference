---
title: "Methods (Unit Catalog Scripting)"
---

# Methods

51 methods from `ScriptUnitCatalog.chm`.

| Name | Summary |
| --- | --- |
| [`IPhysicalQuantityCollection.Add`](iphysicalquantitycollection-add.md) | Adds a physical quantity to the units catalog. |
| [`IPhysicalQuantityCollection.Exists`](iphysicalquantitycollection-exists.md) | Checks whether a physical quantity already exists in the units catalog. |
| [`IPhysicalQuantityCollection.GetIndex`](iphysicalquantitycollection-getindex.md) | Returns the index of a physical quantity from the collection of all the physical quantities in the units catalog. |
| [`IPhysicalQuantityCollection.Item`](iphysicalquantitycollection-item.md) | Returns a Quantity object in the units catalog. A Quantity object is a physical quantity in the units catalog. |
| [`IPhysicalQuantityCollection.Move`](iphysicalquantitycollection-move.md) | Changes the position of a physical quantity in the Quantities collection in the units catalog. If you change the position, you also change the index of the physical quantity. |
| [`IPhysicalQuantityCollection.Remove`](iphysicalquantitycollection-remove.md) | Deletes a physical quantity with all the associated units and symbols, from the units catalog. |
| [`IPhysicalUnitCollection.Add`](iphysicalunitcollection-add.md) | Adds a unit to a physical quantity, in the units catalog. |
| [`IPhysicalUnitCollection.Exists`](iphysicalunitcollection-exists.md) | Checks whether a unit already exists in the units catalog. |
| [`IPhysicalUnitCollection.GetIndex`](iphysicalunitcollection-getindex.md) | Returns the index of a unit of a physical quantity from the entire units catalog. |
| [`IPhysicalUnitCollection.Item`](iphysicalunitcollection-item.md) | Returns a Unit object in the units catalog. A Unit object is a unit of a physical quantity in the units catalog. |
| [`IPhysicalUnitCollection.Move`](iphysicalunitcollection-move.md) | Changes the position of a unit in the Units collection in the units catalog. If you change the position, you also change the index of the unit. |
| [`IPhysicalUnitCollection.Remove`](iphysicalunitcollection-remove.md) | Deletes a unit with all the associated symbols, from the units catalog. |
| [`IUnitCatalog.Clear`](iunitcatalog-clear.md) | Deletes the contents of the current units catalog. |
| [`IUnitCatalog.Load`](iunitcatalog-load.md) | Loads the contents of a units catalog from a file with the filename extension *.tuc . DIAdem overwrites existing contents. The UnitCatalog object is available as a global object in scripts and in dialog boxes. If you want to prepare further catalog units without changing the loaded units catalog, use the OpenExternalCatalog method. |
| [`IUnitCatalog.OpenExternalCatalog`](iunitcatalog-openexternalcatalog.md) | Opens an external units catalog in DIAdem. This units catalog is only available in a script and does not influence the standard units catalog or the dialog boxes in DIAdem. You can use it to prepare further units catalogs, then save it with the method SaveAs , and load it with the method Load , in order to make it available as a global object in scripts and dialog boxes. |
| [`IUnitCatalog.Reset`](iunitcatalog-reset.md) | Restores the delivery status of the units catalog. |
| [`IUnitCatalog.ResetModified`](iunitcatalog-resetmodified.md) | Identifies the current units catalog as unchanged. |
| [`IUnitCatalog.SaveAs`](iunitcatalog-saveas.md) | Saves the current units catalog in a file with the extension .tuc . |
| [`IUnitCatalog.ShowChannelUnitAssistanceDlg`](iunitcatalog-showchannelunitassistancedlg.md) | Opens the Waveform X-Unit: Symbol Input Help dialog box or the Channel Unit: Symbol Entry Helper dialog box. |
| [`IUnitCatalog.ShowSettingsDlg`](iunitcatalog-showsettingsdlg.md) | Opens the dialog box where you edit the unit sets, physical quantities, units, and symbols, of the units catalog. |
| [`IUnitCatalog.ShowSymbolAssistanceDlg`](iunitcatalog-showsymbolassistancedlg.md) | Opens the dialog box Unit Symbol Input Help , where you select unit symbols or add a symbol to a unit set and to a physical quantity. |
| [`IUnitCatalogSymbolCollection.Exists`](iunitcatalogsymbolcollection-exists.md) | Checks whether a symbol already exists in the units catalog. |
| [`IUnitCatalogSymbolCollection.GetIndex`](iunitcatalogsymbolcollection-getindex.md) | Returns the index of a symbol from the collection of all the symbols in the units catalog. |
| [`IUnitCatalogSymbolCollection.Item`](iunitcatalogsymbolcollection-item.md) | Returns an AllSymbols object in the units catalog. An AllSymbols object is a symbol in the units catalog. |
| [`IUnitSet.Activate`](iunitset-activate.md) | Enables the selected unit set as the default unit set. DIAdem then displays this units set as the default set in all dialog boxes of the units catalog if ActiveSetEnable is true. |
| [`IUnitSetCollection.Add`](iunitsetcollection-add.md) | Adds a unit set to the units catalog. |
| [`IUnitSetCollection.Exists`](iunitsetcollection-exists.md) | Checks whether a unit set already exists in the units catalog. |
| [`IUnitSetCollection.GetIndex`](iunitsetcollection-getindex.md) | Returns the index of a unit set from the units catalog. |
| [`IUnitSetCollection.Item`](iunitsetcollection-item.md) | Returns a Set object in the units catalog. A Set object is a unit set in the units catalog. |
| [`IUnitSetCollection.Move`](iunitsetcollection-move.md) | Changes the position of a unit set in the Sets collection in the units catalog. If you change the position, you also change the index of the unit set. |
| [`IUnitSetCollection.Remove`](iunitsetcollection-remove.md) | Deletes a unit set with all the quantities and units it contains, from the units catalog. |
| [`IUnitSetQuantityCollection.Add`](iunitsetquantitycollection-add.md) | Adds a physical quantity to a unit set, in the units catalog. |
| [`IUnitSetQuantityCollection.Exists`](iunitsetquantitycollection-exists.md) | Checks whether a physical quantity already exists in a unit set. |
| [`IUnitSetQuantityCollection.GetIndex`](iunitsetquantitycollection-getindex.md) | Returns the index of a physical quantity that is used, from a unit set in the units catalog. |
| [`IUnitSetQuantityCollection.Item`](iunitsetquantitycollection-item.md) | Returns a UsedQuantity object in the units catalog. A UsedQuantity object is a physical quantity of a unit set in the units catalog. |
| [`IUnitSetQuantityCollection.Move`](iunitsetquantitycollection-move.md) | Changes the position of a physical quantity in the UsedQuantities collection in the units catalog. If you change the position, you also change the index of the physical quantity. |
| [`IUnitSetQuantityCollection.Remove`](iunitsetquantitycollection-remove.md) | Deletes a physical quantity and all the associated units, from a unit set of the units catalog. The physical quantity and the associated units remain in the units catalog. |
| [`IUnitSetUnitCollection.Add`](iunitsetunitcollection-add.md) | Adds a unit to a physical quantity of a unit set, in the units catalog. |
| [`IUnitSetUnitCollection.Exists`](iunitsetunitcollection-exists.md) | Checks whether the unit of a physical quantity already exists in a unit set in the units catalog. |
| [`IUnitSetUnitCollection.GetIndex`](iunitsetunitcollection-getindex.md) | Returns the index of the unit of a physical quantity from a unit set in the units catalog. |
| [`IUnitSetUnitCollection.Item`](iunitsetunitcollection-item.md) | Returns a SetUnit object that is used in a unit set in the units catalog. A SetUnit object is a unit of a physical quantity in a unit set. |
| [`IUnitSetUnitCollection.Move`](iunitsetunitcollection-move.md) | Changes the position of a unit in the UsedUnits collection in the units catalog. If you change the position, you also change the index of the unit. |
| [`IUnitSetUnitCollection.Remove`](iunitsetunitcollection-remove.md) | Deletes a unit from a unit set of the units catalog. The unit remains in the units catalog. |
| [`IUnitSetUnitCollection.SetAsDefault`](iunitsetunitcollection-setasdefault.md) | Specifies a unit as the default unit of a physical quantity within a unit set in the units catalog. |
| [`IUnitSymbol.Activate`](iunitsymbol-activate.md) | Makes the selected symbol the enabled symbol of a unit. DIAdem displays only the enabled symbols, in all the units catalog dialog boxes. |
| [`IUnitSymbolCollection.Add`](iunitsymbolcollection-add.md) | Adds a new symbol to a unit in the units catalog. |
| [`IUnitSymbolCollection.Exists`](iunitsymbolcollection-exists.md) | Checks whether the symbol of a unit already exists in a unit set in the units catalog. |
| [`IUnitSymbolCollection.GetIndex`](iunitsymbolcollection-getindex.md) | Returns the index of an alternative symbol of the unit of a physical quantity from a unit set in the units catalog. |
| [`IUnitSymbolCollection.Item`](iunitsymbolcollection-item.md) | Returns a Symbol object in the units catalog. A Symbol object is a unit symbol of a physical quantity from a unit set in the units catalog. |
| [`IUnitSymbolCollection.Move`](iunitsymbolcollection-move.md) | Changes the position of the alternative symbol in the SymbolAliases collection in the units catalog. If you change the position, you also change the index of the alternative symbol. |
| [`IUnitSymbolCollection.Remove`](iunitsymbolcollection-remove.md) | Deletes an alternative symbol of a unit of the units catalog. |
