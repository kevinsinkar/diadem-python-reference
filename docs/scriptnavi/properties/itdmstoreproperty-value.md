---
title: "ITDMStoreProperty.Value"
description: "Specifies in a data store the value of a property of a data element."
---

# ITDMStoreProperty.Value

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Value for Property <DataStore>

Specifies in a data store the value of a property of a data element.

## Signature

```python
obj.Value
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you read out a value of a date/time property from a data store or assign a date/time value to the property of a data store, this property is a <a href="../../objects/itdmtimedisp/">UsiTimeDisp</a> type. Use the set statement to assign an object to this property in order to continue working with the property. Use the <a href="../itdmtimedisp-variantdate/">VariantDate</a> object property to read or write date/time values in the VBS date format.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note </strong>If you read the value of an enumeration type property (DataTypeEnum) from a data store, you receive this value as text.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  The properties of the USITimeDisp object operate with accurate values even in smaller fractions than in seconds whereas the VBS property <a href="../itdmtimedisp-variantdate/">VariantDate</a> rounds up smaller values to seconds.</td></tr></table>
</div>

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyProperties = oMyDataStore.RootElements(1).Children(1).Children(1).Properties
for MyProperty in oMyProperties:
    if IsObject(MyProperty.Value) :
#Date/Time value
        dd.MsgBoxDisp("Date/Time Property Name: " + MyProperty.Name + "\r\n" +"Property value: " + MyProperty.Value.VariantDate)
    else:
#String, Float, or Integer value
        dd.MsgBoxDisp("String, Float, or Integer Property Name: " + MyProperty.Name + "\r\n" +"Property value: " + MyProperty.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Value_ITDMStoreProperty.htm`*
