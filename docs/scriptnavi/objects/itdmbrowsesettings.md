---
title: "ITDMBrowseSettings"
description: "The browse settings object provides the Browse Settings for a data store. Browse settings have the filename extension *.tbs ."
---

# ITDMBrowseSettings

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: BrowseSettings

The browse settings object provides the Browse Settings for a data store. Browse settings have the filename extension *.tbs .

## Python example

```python
dd.Navigator.Display.OpenDataStore("ASAM Browse Settings Example")
oMyStore = dd.Navigator.Display.CurrDataStore.GetDataStore()
oMyBrowseSettings = dd.Navigator.Settings.LoadBrowseSettings(dd.ConfReadPath + "BS_TestBeds.tbs", oMyStore)
dd.WndShow("NAVIGATOR", "SHOW")
dd.InterActionOn("Please select an element")
oMyElement = dd.Navigator.Display.CurrDatastore.Browser.FocusedElement
oMyBrowseEntity = oMyBrowseSettings.GetBrowseEntity(oMyElement)
dd.MsgBoxDisp(oMyBrowseEntity.EntityType.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmbrowsesettings-rootelements/">RootElements</a> | <a href="../../properties/itdmbrowsesettings-rootentity/">RootEntity</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmbrowsesettings-getbrowseentity/">GetBrowseEntity</a> | <a href="../../methods/itdmbrowsesettings-getchildren/">GetChildren</a> | <a href="../../methods/itdmbrowsesettings-getparent/">GetParent</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itdmdatastore/">DataStore</a>.<a href="../../methods/itdmdatastore-getbrowsesettings/">GetBrowseSettings</a> | <a href="../idatastoredisplay/">DataStoreDisplay</a>.<a href="../../methods/idatastoredisplay-getbrowsesettings/">GetBrowseSettings</a> | <a href="../inavigatorsettings/">Settings &lt;Navigator&gt;</a>.<a href="../../methods/inavigatorsettings-createbrowsesettings/">CreateBrowseSettings</a> | <a href="../inavigatorsettings/">Settings &lt;Navigator&gt;</a>.<a href="../../methods/inavigatorsettings-loadbrowsesettings/">LoadBrowseSettings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMBrowseSettings.htm`*
