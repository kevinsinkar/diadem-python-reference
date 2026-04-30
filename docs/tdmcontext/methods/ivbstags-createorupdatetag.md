---
title: "IVbsTags.CreateOrUpdateTag"
description: "Creates a SystemLink tag in the workspace of the associated task. Whether you can create the tag in the task's workspace depends on the privileges of the servic"
---

# IVbsTags.CreateOrUpdateTag

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: CreateOrUpdateTag for Tags <SystemLink>

Creates a SystemLink tag in the workspace of the associated task. Whether you can create the tag in the task's workspace depends on the privileges of the service or user who executes the task. Instead of the CreateOrUpdateTag method, use the CreateOrUpdateTagToWorkspace method to specify the workspace.

## Signature

```python
obj.CreateOrUpdateTag(path, Type, keywords, properties, collectAggregates)
```

## Python example

```python
import win32com
import datetime
def On_Run_AnalysisProcedure(oContext):
    oJsonParser = dd.CreateJsonParser()
    aMyArray = ["Key 1","Key 2"]
    sJsonString = oJsonParser.Serialize(aMyArray)
    ResultsPath = oContext.Procedure.Arguments.Item("ResultsPath").Value
    sProperty = AddKeyValue(["Resultpath","Procedure"],[ResultsPath, oContext.TaskExecution.Procedure.Name])
    oContext.Tags.CreateOrUpdateTag("task.id." + oContext.TaskExecution.Id, 1, sJsonString, sProperty, True)
    sValue = TimeStampedValue("47", "1")
    oContext.Tags.UpdateTagTimestampedValue("task.id." + oContext.TaskExecution.Id, sValue)

def TimeStampedValue(sValue,sType):
    oJsonParser = dd.CreateJsonParser()
    oMySubobject = win32com.client.Dispatch("Scripting.Dictionary")
    oMyMainObject = win32com.client.Dispatch("Scripting.Dictionary")

    oMySubobject.Add("type", sType)
    oMySubobject.Add("value", sValue)

    oMyMainObject.Add("value", oMySubobject)
    oMyMainObject.Add("timestamp", oJsonParser.CreateDateTime(datetime.datetime.now(), False))
    TimeStampedValue = oJsonParser.Serialize(oMyMainObject, False)
    return TimeStampedValue

def AddKeyValue(sKeyArray,sValueArray):
    oJsonParser = dd.CreateJsonParser()
    oMyObject = win32com.client.Dispatch("Scripting.Dictionary")
    for iCount in range( 0, len(sKeyArray)-1):
        oMyObject.Add(sKeyArray(iCount), sValueArray(iCount))
    AddKeyValue = oJsonParser.Serialize(oMyObject, False)
    return AddKeyValue
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_CreateOrUpdateTag_IVbsTags.htm`*
