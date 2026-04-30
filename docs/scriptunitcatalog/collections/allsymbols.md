---
title: "AllSymbols"
description: "The AllSymbols collection provides all the symbols from the units catalog."
---

# AllSymbols

!!! abstract "Collection &middot; `ScriptUnitCatalog.chm`"
    Collection: AllSymbols

The AllSymbols collection provides all the symbols from the units catalog.

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The symbols are listed in alphabetical order in the <span class="Monospace">AllSymbols</span> collection. Use the <span class="Monospace">SymbolAliases</span> collection of the <span class="Monospace">Unit</span> object to delete or to add symbols.</td></tr></table>
</div>

## Python example

```python
for oMySymbol in dd.UnitCatalog.AllSymbols:
    sOutput = sOutput + oMySymbol.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

```python
oMySymbol = dd.Unitcatalog.AllSymbols("Km")
oMySymbol.Unit.SymbolAliases.Add("KM")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iunitcatalogsymbolcollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iunitcatalogsymbolcollection-exists/">Exists</a> | <a href="../../methods/iunitcatalogsymbolcollection-getindex/">GetIndex</a> | <a href="../../methods/iunitcatalogsymbolcollection-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/iunitcatalog/">UnitCatalog</a>.<a href="../../properties/iunitcatalog-allsymbols/">AllSymbols</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div></div>
</div>

---

*Source: `ScriptUnitCatalog/objects/DiaCmpnt_Objects_IUnitCatalogSymbolCollection.htm`*
