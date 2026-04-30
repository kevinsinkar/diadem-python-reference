---
title: "ITDMDataFinderIndexer.Status"
description: "Specifies in a DataFinder the status of the indexer."
---

# ITDMDataFinderIndexer.Status

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Status for Indexer

Specifies in a DataFinder the status of the indexer.

## Signature

```python
obj.Status
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you abort indexing the <span class="Monospace">My DataFinder</span> DataFinder by selecting <strong>Pause Indexing</strong> from the context menu of the DataFinder symbol on the Windows task bar, you overlap the functionality of the methods of the Indexer object, for example, <a href="../../methods/itdmdatafinderindexer-indexfile/">IndexFile</a> or <a href="../../methods/itdmdatafinderindexer-updateindex/">UpdateIndex</a>. If you stopped the indexing through the context menu, the DataFinder does not index the files in the search area even if you generate a new search area with the <span class="Monospace">DataFinder.GetSettings.SearchAreas.Add</span> method. However, if you open a search area in the NAVIGATOR tree, DIAdem indexes the files in the search area and ignores the command <strong>Pause Indexing</strong> previously selected in the context menu of the <span class="Monospace">My DataFinder</span> DataFinder.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eIndexerRunning` | 1 | The indexing is active. |
| `eIndexerPaused` | 2 | The indexing is not active. |

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyIndexer = oMyDataFinder.Indexer
dd.MsgBoxDisp(oMyIndexer.Status)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Status_ITDMDataFinderIndexer.htm`*
