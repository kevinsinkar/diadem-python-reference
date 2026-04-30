---
title: "ITDMDataStore.Close"
description: "Closes a data store you opened with the ConnectDataStore method or the Display . OpenDataStore method. After the data store closes, all elements from the data s"
---

# ITDMDataStore.Close

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Close for DataStore

Closes a data store you opened with the ConnectDataStore method or the Display . OpenDataStore method. After the data store closes, all elements from the data store are invalid. Check whether an element is valid with the IsValid method. When all data store elements are closed, the data store closes.

## Signature

```python
obj.Close()
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Do not use the <span class="Monospace">Close</span> method if you opened a data store with the <a href="../idatastoredisplay-getdatastore/">GetDataStore</a> method.</td></tr></table>
</div>

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
dd.MsgBoxDisp("DataStore name: " + oMyDataStore.Name)
oMyDataStore.Close()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Close_ITDMDataStore.htm`*
