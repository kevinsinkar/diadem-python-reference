---
title: "IRegisteredDataPlugin"
description: "The RegisteredDataPlugin object provides information about a DataPlugin registered on your computer."
---

# IRegisteredDataPlugin

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: RegisteredDataPlugin <Navigator>

The RegisteredDataPlugin object provides information about a DataPlugin registered on your computer.

## Python example

```python
oMyDataPlugins = dd.Navigator.Settings.RegisteredDataPlugins
for DataPlugin in oMyDataPlugins:
    sOutput = sOutput + DataPlugin.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iregistereddataplugin-description/">Description</a> | <a href="../../properties/iregistereddataplugin-fileextensionlist/">FileExtensionList</a> | <a href="../../properties/iregistereddataplugin-isfastloadingsupported/">IsFastLoadingSupported</a> | <a href="../../properties/iregistereddataplugin-isfilebased/">IsFileBased</a> | <a href="../../properties/iregistereddataplugin-isloadingsupported/">IsLoadingSupported</a> | <a href="../../properties/iregistereddataplugin-isprotected/">IsProtected</a> | <a href="../../properties/iregistereddataplugin-isquerysupported/">IsQuerySupported</a> | <a href="../../properties/iregistereddataplugin-isregistersupported/">IsRegisterSupported</a> | <a href="../../properties/iregistereddataplugin-issavingsupported/">IsSavingSupported</a> | <a href="../../properties/iregistereddataplugin-isselectiveloadingsupported/">IsSelectiveLoadingSupported</a> | <a href="../../properties/iregistereddataplugin-istdmmodel/">IsTdmModel</a> | <a href="../../properties/iregistereddataplugin-modelname/">ModelName</a> | <a href="../../properties/iregistereddataplugin-name/">Name</a> | <a href="../../properties/iregistereddataplugin-type/">Type</a> | <a href="../../properties/iregistereddataplugin-version/">Version</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iregistereddataplugin-export/">Export</a> | <a href="../../methods/iregistereddataplugin-exportencrypted/">ExportEncrypted</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/registereddataplugins/">RegisteredDataPlugins &lt;Navigator&gt;</a>.<a href="../../methods/iregistereddataplugincollection-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IRegisteredDataPlugin.htm`*
