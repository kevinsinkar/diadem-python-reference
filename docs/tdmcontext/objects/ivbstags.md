---
title: "IVbsTags"
description: "The Tags <SystemLink> object creates and modifies SystemLink tags and returns the tag values. Tags correspond to variables that are valid throughout the SystemL"
---

# IVbsTags

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: Tags <SystemLink>

The Tags <SystemLink> object creates and modifies SystemLink tags and returns the tag values. Tags correspond to variables that are valid throughout the SystemLink environment and that you can access via a unique identifier.

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
    oContext.Tags.CreateOrUpdateTagToWorkspace("task.id." + oContext.TaskExecution.Id, 1, sJsonString, sProperty, True, "0aadbc36-9498-4928-94cf-b600eab14562")
    sValue = TimeStampedValue("47", "1")
    oContext.Tags.UpdateTagTimestampedValue("task.id." + oContext.TaskExecution.Id, sValue)
    sReturn = oContext.Tags.GetTagValues("task.id." + oContext.TaskExecution.Id)
    oContext.LogResult(sReturn)

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

## Members

<div markdown="1">
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivbstags-createorupdatetag/">CreateOrUpdateTag</a> | <a href="../../methods/ivbstags-createorupdatetagtoworkspace/">CreateOrUpdateTagToWorkspace</a> | <a href="../../methods/ivbstags-gettagvalues/">GetTagValues</a> | <a href="../../methods/ivbstags-gettagvaluesfromworkspace/">GetTagValuesFromWorkspace</a> | <a href="../../methods/ivbstags-updatetagtimestampedvalue/">UpdateTagTimestampedValue</a> | <a href="../../methods/ivbstags-updatetagtimestampedvalueinworkspace/">UpdateTagTimestampedValueInWorkspace</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ivbscontextasdeinit/">ContextFinalize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasdeinit-tags/">Tags</a> | <a href="../ivbscontextasinit/">ContextInitialize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasinit-tags/">Tags</a> | <a href="../ivbscontextas/">ContextRun &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextas-tags/">Tags</a> | <a href="../ivbscontextvnv/">ContextVnV &lt;Data Preprocessor&gt;</a>.<a href="../../properties/ivbscontextvnv-tags/">Tags</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsTags.htm`*
