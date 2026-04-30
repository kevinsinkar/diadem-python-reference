---
title: "IImportParameterSet"
description: "The ImportParameter <Navigator> object provides all properties for the import of data in DIAdem. Note You can use the Import parameter <Navigator>Object as a pa"
---

# IImportParameterSet

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: ImportParameter <Navigator>

The ImportParameter <Navigator> object provides all properties for the import of data in DIAdem. Note You can use the Import parameter <Navigator>Object as a parameter in the following commands and methods: DataFileLoad , DataFileLoadSel , Navigator . LoadData , navigator . LoadProperty and StorageImport .

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  You can use the Import parameter &lt;Navigator&gt;Object as a parameter in the following commands and methods: <a href="../../../comoff/commands/datafileload/">DataFileLoad</a>, <a href="../../../comoff/commands/datafileloadsel/">DataFileLoadSel</a>, <a href="../inavigator/">Navigator</a>.<a href="../../methods/inavigator-loaddata/">LoadData</a>, <a href="../inavigator/">navigator</a>.<a href="../../methods/inavigator-loadproperty/">LoadProperty</a> and <a href="../../../comoff/commands/storageimport/">StorageImport</a>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  As of DIAdem version 2017, the load parameters use the settings of the ImportParameter object as soon as you transfer this object to the load parameter. The modifications to the global load parameters as known from previous DIAdem versions are no longer necessary.</td></tr></table>
</div>

## Python example

```python
oMyImportParameter = dd.Navigator.Settings.CreateImportParameter("Append")
oMyImportParameter.AppendCheckGroupName = dd.eAppendCheckGroupNameAutomatic
oMyImportParameter.BulkDataLoadingMode = dd.eBulkDataLoadingImmediately
dd.DataFileLoad("Example.tdm", "TDM", oMyImportParameter)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iimportparameterset-appendcheckgroupname/">AppendCheckGroupName</a> | <a href="../../properties/iimportparameterset-bulkdataloadingmode/">BulkDataLoadingMode</a> | <a href="../../properties/iimportparameterset-channelrelationmode/">ChannelRelationMode</a> | <a href="../../properties/iimportparameterset-importmode/">ImportMode</a> | <a href="../../properties/iimportparameterset-loadreturnmode/">LoadReturnMode</a> | <a href="../../properties/iimportparameterset-propertyhandling/">PropertyHandling</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../inavigatorsettings/">Settings &lt;Navigator&gt;</a>.<a href="../../methods/inavigatorsettings-createimportparameter/">CreateImportParameter</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IImportParameterSet.htm`*
