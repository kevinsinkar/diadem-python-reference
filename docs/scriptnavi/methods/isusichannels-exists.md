---
title: "ISUSIChannels.Exists"
description: "Checks in a DataFinder whether a Channel object with a specific name already exists in the Channels <DataFinder> collection. The Channels <DataFinder> collectio"
---

# ISUSIChannels.Exists

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Exists for Channels <DataFinder>

Checks in a DataFinder whether a Channel object with a specific name already exists in the Channels <DataFinder> collection. The Channels <DataFinder> collection contains all channels of a channel group.

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
        oMyChannel = Element.Channelgroups(1).Channels
        if oMyChannel.Exists("Temp_A") :
            dd.MsgBoxDisp (oMyChannel.Item("Temp_A").Properties("description").Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Exists_ISUSIChannels.htm`*
