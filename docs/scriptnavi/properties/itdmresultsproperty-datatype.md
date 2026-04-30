---
title: "ITDMResultsProperty.DataType"
description: "Specifies in a column-oriented search the data type of a property in the search results. Note DIAdem automatically specifies the data type of base properties an"
---

# ITDMResultsProperty.DataType

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: DataType for ResultsProperty

Specifies in a column-oriented search the data type of a property in the search results. Note DIAdem automatically specifies the data type of base properties and optimized custom properties. Use the Add method to specify the data type of non-optimized custom properties.

## Signature

```python
obj.DataType
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  DIAdem automatically specifies the data type of base properties and optimized custom properties. Use the <a href="../../methods/itdmcolumns-add/">Add</a> method to specify the data type of non-optimized custom properties.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `Enumeration` | 24 | DataTypeEnum |

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
for Result in oMyResultsProps:
    sOutput = sOutput + "Property name: " + Result.Property + " - Property data type: " + Result.DataType + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_DataType_ITDMResultsProperty.htm`*
