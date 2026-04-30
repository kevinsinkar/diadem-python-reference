---
title: "IUnitCatalogSymbolCollection.Item"
description: "Returns an AllSymbols object in the units catalog. An AllSymbols object is a symbol in the units catalog."
---

# IUnitCatalogSymbolCollection.Item

!!! abstract "Method &middot; `ScriptUnitCatalog.chm`"
    Method: Item for AllSymbols

Returns an AllSymbols object in the units catalog. An AllSymbols object is a symbol in the units catalog.

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

```python
dd.MsgBoxDisp (dd.UnitCatalog.AllSymbols.Item(1).Name)
dd.MsgBoxDisp (dd.UnitCatalog.AllSymbols(1).Name)
```

```python
dd.MsgBoxDisp (dd.UnitCatalog.AllSymbols.Item("%").Name)
dd.MsgBoxDisp (dd.UnitCatalog.AllSymbols("%").Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/methods/DiaCmpnt_method_Item_IUnitCatalogSymbolCollection.htm`*
