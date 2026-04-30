---
title: "IDataFileHeaderAccess.Open"
description: "Provides a DataStore object by opening a data store with which you read, write, change, and delete the channel properties, group properties, and root properties"
---

# IDataFileHeaderAccess.Open

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Open for DataFileHeaderAccess

Provides a DataStore object by opening a data store with which you read, write, change, and delete the channel properties, group properties, and root properties of files, whereby the associated mass data is write-protected. For full access to a data store, use the DataStoreDisplay . GetDataStore , the Navigator . ConnectDataStore , or the Navigator . ConnectDataStoreByParameter method.

## Signature

```python
return_value = obj.Open(DataFileName, FileImportFilter, ReadOnly)
```

## Python example

```python
oMyDataFileHeaderAccess = CreateDataFileHeaderAccess
oMyDataStore            = oMyDataFileHeaderAccess.Open(dd.DataReadPath + "Example.tdm" ,"TDM", False)
print(oMyDataStore.RootElements(1).Children(1).Children(2).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Open_IDataFileHeaderAccess.htm`*
