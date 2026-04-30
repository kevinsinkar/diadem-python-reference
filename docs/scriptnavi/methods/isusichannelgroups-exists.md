---
title: "ISUSIChannelGroups.Exists"
description: "Checks in a DataFinder whether a ChannelGroup object with a specific name already exists in the channel group collection."
---

# ISUSIChannelGroups.Exists

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Exists for ChannelGroups <DataFinder>

Checks in a DataFinder whether a ChannelGroup object with a specific name already exists in the channel group collection.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
#--- Search with GUI
oMyQueryForm = dd.Navigator.Display.CurrDataFinder.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType = dd.eSearchFile
#--- Fill the query
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","TR_M17_QT_32-1.*")
oMyConditions.Logic = "C1"
#--- Search with GUI
oMyQueryForm.Search()
#--- Search in results
oMyResultsElements = dd.Navigator.Display.CurrDataFinder.ResultsList.Elements
for Element in oMyResultsElements:
    if Element.IsKindOf(dd.eSearchFile) :
        oMyChannelgroup = Element.Channelgroups
        if oMyChannelgroup.Exists("QT_32-1_Lower") :
            dd.MsgBoxDisp (oMyChannelgroup.Item("QT_32-1_Lower").Properties("Test_Name").Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Exists_ISUSIChannelGroups.htm`*
