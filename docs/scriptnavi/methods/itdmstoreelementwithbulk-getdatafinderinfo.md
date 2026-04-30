---
title: "ITDMStoreElementWithBulk.GetDataFinderInfo"
description: "Returns the name of a DataFinder instance and the name of the computer on which this DataFinder instance is running as DataFinderName@Server if the element in a"
---

# ITDMStoreElementWithBulk.GetDataFinderInfo

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetDataFinderInfo for ElementWithValues <DataStore>

Returns the name of a DataFinder instance and the name of the computer on which this DataFinder instance is running as DataFinderName@Server if the element in a data store in DIAdem NAVIGATOR originates from a Federation server or from an NI ASAM server. The method outputs an error message if the data store that contains the element is not a Federation instance and not an NI ASAM server. Note Only the data elements derived from the base type AoLocalColumn are ElementWithValues <DataStore> types.

## Signature

```python
sGetDataFinderInfo = Object.GetDataFinderInfo()
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Only the data elements derived from the base type <span class="Monospace">AoLocalColumn</span> are <span class="Monospace">ElementWithValues &lt;DataStore&gt;</span> types.</td></tr></table>
</div>

## Python example

```python
dd.MsgBoxDisp(dd.Navigator.Display.CurrDataStore.Browser.SelectedElements(1).GetDataFinderInfo)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetDataFinderInfo_ITDMStoreElementWithBulk.htm`*
