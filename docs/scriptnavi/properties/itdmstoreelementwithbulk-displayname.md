---
title: "ITDMStoreElementWithBulk.DisplayName"
description: "Specifies in a data store the display name of a data element."
---

# ITDMStoreElementWithBulk.DisplayName

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: DisplayName for ElementWithValues <DataStore>

Specifies in a data store the display name of a data element.

## Signature

```python
obj.DisplayName
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Only the data elements derived from the base type <span class="Monospace">AoLocalColumn</span> are <span class="Monospace">ElementWithValues &lt;DataStore&gt;</span> types.</td></tr></table>
</div>

## Python example

```python
oMyDataStore = dd.NAVIGATOR.ConnectDataStore("ASAM Browse Settings Example")
oMyRootElement = oMyDataStore.RootElements(1)
oMyStoreElement = oMyRootElement.Children(1)
dd.MsgBoxDisp(oMyStoreElement.DisplayName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_DisplayName_ITDMStoreElementWithBulk.htm`*
