---
title: "ITDMStoreElementWithBulk.IsValid"
description: "Specifies whether the data element is valid for accessing bulk data. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues "
---

# ITDMStoreElementWithBulk.IsValid

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: IsValid for ElementWithValues <DataStore>

Specifies whether the data element is valid for accessing bulk data. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types.

## Signature

```python
bIsValid = Object.IsValid()
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>Only the data elements derived from the base type <span class="Monospace">AoLocalColumn</span> are <span class="Monospace">ElementWithValues &lt;DataStore&gt;</span> types.</td>
</tr>
</table>
</div>

## Python example

```python
oMyDataStore = dd.NAVIGATOR.ConnectDataStore("ASAM Browse Settings Example")
oMyModel = oMyDataStore.Model
oMyLocalColumn = oMyDataStore.CreateElement(oMyModel.Entities("AolocalColumn").SubTypes(1), "MyLocalColumn")
dd.MsgBoxDisp(oMyLocalColumn.IsValid)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_IsValid_ITDMStoreElementWithBulk.htm`*
