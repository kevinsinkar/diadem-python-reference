---
title: "ITDMBrowseEntity"
description: "In a DataFinder the BrowseEntity object provides an entity of the Browse path ."
---

# ITDMBrowseEntity

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: BrowseEntity

In a DataFinder the BrowseEntity object provides an entity of the Browse path .

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
<p><a href="../../properties/itdmbrowseentity-childentity/">ChildEntity</a> | <a href="../../properties/itdmbrowseentity-childpath/">ChildPath</a> | <a href="../../properties/itdmbrowseentity-entitytype/">EntityType</a> | <a href="../../properties/itdmbrowseentity-parententity/">ParentEntity</a> | <a href="../../properties/itdmbrowseentity-parentpath/">ParentPath</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="./">BrowseEntity</a>.<a href="../../properties/itdmbrowseentity-childentity/">ChildEntity</a> | <a href="./">BrowseEntity</a>.<a href="../../properties/itdmbrowseentity-parententity/">ParentEntity</a> | <a href="../itdmbrowsesettings/">BrowseSettings</a>.<a href="../../methods/itdmbrowsesettings-getbrowseentity/">GetBrowseEntity</a> | <a href="../itdmbrowsesettings/">BrowseSettings</a>.<a href="../../properties/itdmbrowsesettings-rootentity/">RootEntity</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMBrowseEntity.htm`*
