---
title: "ITDMDataStore.SetBrowseSettings"
description: "Assigns new Browse Settings to a data store."
---

# ITDMDataStore.SetBrowseSettings

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: SetBrowseSettings for DataStore

Assigns new Browse Settings to a data store.

## Signature

```python
obj.SetBrowseSettings(BrowseSettings)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  When you assign new browse settings to a data store, the <a href="../../properties/itdmstoreelement-children/">children</a> and <a href="../../properties/itdmstoreelement-parent/">parent</a> properties of an element return other entities.</td></tr></table>
</div>

## Python example

```python
oMyStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyBrowseSettings = dd.Navigator.Settings.LoadBrowseSettings("D:\\MyBrowseSettings.tbs", oMyStore)
oMyStore.SetBrowseSettings(oMyBrowseSettings)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_SetBrowseSettings_ITDMDataStore.htm`*
