---
title: "IUpdateSource.Install"
description: "Installs a DataPlugin from the update source on your computer. You can install only VBS and VBCrypt DataPlugins with a script on your computer."
---

# IUpdateSource.Install

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Install for UpdateSource <Navigator>

Installs a DataPlugin from the update source on your computer. You can install only VBS and VBCrypt DataPlugins with a script on your computer.

## Signature

```python
bInstall = Object.Install(DataPluginName)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If you created a DataPlugin on your computer with the same name as a DataPlugin, which the update source is to install, the <span class="Monospace">Install</span> method overwrites the DataPlugin you created. The <span class="Monospace">Install</span> method only overwrites the URI file. The VBS file of the DataPlugin you created remains in the local DataPlugin folder. You can restore the DataPlugin you created by generating a new URI file with the VBS file you created.</td></tr></table>
</div>

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
oMyUpdateData = oMyDataUpdateSource.UpdateData
if oMyUpdateData.Exists("GPX") :
    oPluginData = oMyUpdateData("GPX")
    if ((oPluginData.Type == dd.ePluginCodeVbCrypt) or (oPluginData.Type == dd.ePluginCodeVbs)) :
        oMyDataUpdateSource.Install("GPX")
    else:
        dd.MsgBoxDisp("DataPlugin " + oPluginData.Name + " is no VBCrypt or VBS DataPlugin." + "\r\n" + "Please install the DataPlugin manually from the NI website.")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Install_IUpdateSource.htm`*
