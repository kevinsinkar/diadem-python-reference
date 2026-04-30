---
title: "ICommonExportParameter"
description: "The CommonExportParameter <Navigator> object provides the properties and methods for configuring the export of data with a specified DataPlugin."
---

# ICommonExportParameter

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: CommonExportParameter <Navigator>

The CommonExportParameter <Navigator> object provides the properties and methods for configuring the export of data with a specified DataPlugin.

## Python example

```python
oMyDataPluginExport = dd.Navigator.Settings.CreateDataPluginParameter("CSV_Export")
if IsObject(oMyDataPluginExport) :
    print(oMyDataPluginExport.DataPluginName)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/icommonexportparameter-datapluginname/">DataPluginName</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/icommonexportparameter-showdialog/">ShowDialog</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../inavigatorsettings/">Settings &lt;Navigator&gt;</a>.<a href="../../methods/inavigatorsettings-createdatapluginparameter/">CreateDataPluginParameter</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ICommonExportParameter.htm`*
