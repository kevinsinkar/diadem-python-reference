---
title: "INavigatorSettings.CreateImportParameter"
description: "Returns an object with all parameters for importing data in DIAdem. Note You can only use the ImportParameter object in the 64-bit version of DIAdem. Note You c"
---

# INavigatorSettings.CreateImportParameter

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: CreateImportParameter for Settings <Navigator>

Returns an object with all parameters for importing data in DIAdem. Note You can only use the ImportParameter object in the 64-bit version of DIAdem. Note You can use the ImportParameter <Navigator> object as a parameter in the following commands and methods: DataFileLoad , DataFileLoadSel , Navigator . LoadData , Navigator . LoadProperty , and StorageImport .

## Signature

```python
return_value = obj.CreateImportParameter([ImportAction])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  You can only use the ImportParameter object in the 64-bit version of DIAdem.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  You can use the ImportParameter &lt;Navigator&gt; object as a parameter in the following commands and methods: <a href="../../../comoff/commands/datafileload/">DataFileLoad</a>, <a href="../../../comoff/commands/datafileloadsel/">DataFileLoadSel</a>, <a href="../../objects/inavigator/">Navigator</a>.<a href="../inavigator-loaddata/">LoadData</a>, <a href="../../objects/inavigator/">Navigator</a>.<a href="../inavigator-loadproperty/">LoadProperty</a>, and <a href="../../../comoff/commands/storageimport/">StorageImport</a>.</td></tr></table>
</div>

## Python example

```python
if dd.ApplicationBitness == 64 :
    oMyImportParameter = dd.Navigator.Settings.CreateImportParameter("Append")
    oMyImportParameter.AppendCheckGroupName = dd.eAppendCheckGroupNameAutomatic
    oMyImportParameter.BulkDataLoadingMode = dd.eBulkDataLoadingOnFirstAccess
    dd.DataFileLoad("Example.tdm", "TDM", oMyImportParameter)
else:
    print("ImportParameter object only supported in 64 bit")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_CreateImportParameter_INavigatorSettings.htm`*
