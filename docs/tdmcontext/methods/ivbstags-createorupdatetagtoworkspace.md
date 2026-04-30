---
title: "IVbsTags.CreateOrUpdateTagToWorkspace"
description: "Generates a SystemLink tag in the specified workspace. Whether you can execute this method in a task with the specified workspace depends on the privileges of t"
---

# IVbsTags.CreateOrUpdateTagToWorkspace

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: CreateOrUpdateTagToWorkspace for Tags <SystemLink>

Generates a SystemLink tag in the specified workspace. Whether you can execute this method in a task with the specified workspace depends on the privileges of the service or user who executes the task. Use the CreateOrUpdateTagToWorkspace method instead of the CreateOrUpdateTag method to also specify the workspace.

## Signature

```python
obj.CreateOrUpdateTagToWorkspace(path, type, keywords, properties, collectAggregates, workspace)
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
    oContext.Tags.CreateOrUpdateTagToWorkspace("task.id." + oContext.TaskExecution.Id, 1, sJsonString, sProperty, True, "0aadbc36-9498-4928-94cf-b600eab14562")
    sValue = TimeStampedValue("47", "1")
    oContext.Tags.UpdateTagTimestampedValueInWorkspace("task.id." + oContext.TaskExecution.Id, sValue, "0aadbc36-9498-4928-94cf-b600eab14562")

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
<div class="SeeAlso">
<p class="body">The following example creates a SystemLink tag and then writes the value <span class="Monospace">47</span> together with the JSON string <span class="Monospace">{"value":{"type":"1","value":"47"},"timestamp":"2018-11-27T11:58:55Z"}</span> to the tag:</p>
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p></div><div class="codeblue"><pre><donottranslate><span class="HlVBSKeyword">Sub</span> On_Run_AnalysisProcedure(oContext)
  <span class="HlVBSKeyword">Dim</span> oJsonParser, sJsonString, aMyArray, ResultsPath, sProperty, sValue
  <span class="HlVBSKeyword">Set</span> oJsonParser = <span class="Hldiademcommand">CreateJsonParser</span>()
  aMyArray = <span class="HlVBSKeyword">Array</span>(<span class="HlString">"Key 1"</span>,<span class="HlString">"Key 2"</span>)
  sJsonString = oJsonParser.Serialize(aMyArray)
  ResultsPath = oContext.Procedure.Arguments.Item(<span class="HlString">"ResultsPath"</span>).Value
  sProperty = AddKeyValue(<span class="HlVBSKeyword">Array</span>(<span class="HlString">"Resultpath"</span>,<span class="HlString">"Procedure"</span>),<span class="HlVBSKeyword">Array</span>(ResultsPath, oContext.TaskExecution.Procedure.Name))
  <span class="HlVBSKeyword">Call</span> oContext.Tags.CreateOrUpdateTagToWorkspace(<span class="HlString">"task.id."</span> &amp; oContext.TaskExecution.Id, <span class="HlNumbers">1</span>, sJsonString, sProperty, <span class="HlVBSKeyword">true</span>, <span class="HlString">"0aadbc36-9498-4928-94cf-b600eab14562"</span>)
  sValue = TimeStampedValue(<span class="HlString">"47"</span>, <span class="HlString">"1"</span>)
  <span class="HlVBSKeyword">Call</span> oContext.Tags.UpdateTagTimestampedValueInWorkspace(<span class="HlString">"task.id."</span> &amp; oContext.TaskExecution.Id, sValue, <span class="HlString">"0aadbc36-9498-4928-94cf-b600eab14562"</span>)
<span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">Sub</span>

<span class="HlVBSKeyword">Function</span> TimeStampedValue(sValue,sType)
  <span class="HlVBSKeyword">Dim</span> oJsonParser, oMySubobject, oMyMainObject
  <span class="HlVBSKeyword">Set</span> oJsonParser = <span class="Hldiademcommand">CreateJsonParser</span>()
  <span class="HlVBSKeyword">Set</span> oMySubobject = <span class="HlVBSKeyword">CreateObject</span>(<span class="HlString">"Scripting.Dictionary"</span>)
  <span class="HlVBSKeyword">Set</span> oMyMainObject = <span class="HlVBSKeyword">CreateObject</span>(<span class="HlString">"Scripting.Dictionary"</span>)
  
  <span class="HlVBSKeyword">Call</span> oMySubobject.Add(<span class="HlString">"type"</span>, sType)  
  <span class="HlVBSKeyword">Call</span> oMySubobject.Add(<span class="HlString">"value"</span>, sValue)
  
  <span class="HlVBSKeyword">Call</span> oMyMainObject.Add(<span class="HlString">"value"</span>, oMySubobject)
  <span class="HlVBSKeyword">Call</span> oMyMainObject.Add(<span class="HlString">"timestamp"</span>, oJsonParser.CreateDateTime(<span class="HlVBSKeyword">Now</span>, <span class="HlVBSKeyword">False</span>))
  TimeStampedValue = oJsonParser.Serialize(oMyMainObject, <span class="HlVBSKeyword">False</span>)
<span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">Function</span>

<span class="HlVBSKeyword">Function</span> AddKeyValue(sKeyArray,sValueArray)
  <span class="HlVBSKeyword">Dim</span> oJsonParser, oMyObject, iCount
  <span class="HlVBSKeyword">Set</span> oJsonParser = <span class="Hldiademcommand">CreateJsonParser</span>()
  <span class="HlVBSKeyword">Set</span> oMyObject = <span class="HlVBSKeyword">CreateObject</span>(<span class="HlString">"Scripting.Dictionary"</span>)
  <span class="HlVBSKeyword">For</span> iCount = <span class="HlNumbers">0</span> <span class="HlVBSKeyword">to</span> <span class="HlVBSKeyword">UBound</span>(sKeyArray) 
    <span class="HlVBSKeyword">Call</span> oMyObject.Add(sKeyArray(iCount), sValueArray(iCount))
  <span class="HlVBSKeyword">Next</span>
  AddKeyValue = oJsonParser.Serialize(oMyObject, <span class="HlVBSKeyword">False</span>)
<span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">Function</span></donottranslate></pre></div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate><span class="HlVBSKeyword">import</span> win32com
<span class="HlVBSKeyword">import</span> datetime
<span class="HlVBSKeyword">def</span> On_Run_AnalysisProcedure(oContext): 
    oJsonParser = dd.CreateJsonParser() 
    aMyArray = [<span class="HlString">"Key 1"</span>,<span class="HlString">"Key 2"</span>] 
    sJsonString = oJsonParser.Serialize(aMyArray) 
    ResultsPath = oContext.Procedure.Arguments.Item(<span class="HlString">"ResultsPath"</span>).Value 
    sProperty = AddKeyValue([<span class="HlString">"Resultpath"</span>,<span class="HlString">"Procedure"</span>],[ResultsPath, oContext.TaskExecution.Procedure.Name]) 
    oContext.Tags.CreateOrUpdateTagToWorkspace(<span class="HlString">"task.id."</span> + oContext.TaskExecution.Id, <span class="HlNumbers">1</span>, sJsonString, sProperty, <span class="HlVBSKeyword">True</span>, <span class="HlString">"0aadbc36-9498-4928-94cf-b600eab14562"</span>) 
    sValue = TimeStampedValue(<span class="HlString">"47"</span>, <span class="HlString">"1"</span>) 
    oContext.Tags.UpdateTagTimestampedValueInWorkspace(<span class="HlString">"task.id."</span> + oContext.TaskExecution.Id, sValue, <span class="HlString">"0aadbc36-9498-4928-94cf-b600eab14562"</span>) 

<span class="HlVBSKeyword">def</span> TimeStampedValue(sValue,sType): 
    oJsonParser = dd.CreateJsonParser() 
    oMySubobject = win32com.client.Dispatch(<span class="HlString">"Scripting.Dictionary"</span>) 
    oMyMainObject = win32com.client.Dispatch(<span class="HlString">"Scripting.Dictionary"</span>) 

    oMySubobject.Add(<span class="HlString">"type"</span>, sType) 
    oMySubobject.Add(<span class="HlString">"value"</span>, sValue) 

    oMyMainObject.Add(<span class="HlString">"value"</span>, oMySubobject) 
    oMyMainObject.Add(<span class="HlString">"timestamp"</span>, oJsonParser.CreateDateTime(datetime.datetime.now(), <span class="HlVBSKeyword">False</span>)) 
    TimeStampedValue = oJsonParser.Serialize(oMyMainObject, <span class="HlVBSKeyword">False</span>) 
    <span class="HlVBSKeyword">return</span> TimeStampedValue

<span class="HlVBSKeyword">def</span> AddKeyValue(sKeyArray,sValueArray): 
    oJsonParser = dd.CreateJsonParser() 
    oMyObject = win32com.client.Dispatch(<span class="HlString">"Scripting.Dictionary"</span>) 
    <span class="HlVBSKeyword">for</span> iCount <span class="HlVBSKeyword">in</span> <span class="HlVBSKeyword">range</span>( <span class="HlNumbers">0</span>, <span class="HlVBSKeyword">len</span>(sKeyArray)-<span class="HlNumbers">1</span>): 
        oMyObject.Add(sKeyArray(iCount), sValueArray(iCount)) 
    AddKeyValue = oJsonParser.Serialize(oMyObject, <span class="HlVBSKeyword">False</span>) 
    <span class="HlVBSKeyword">return</span> AddKeyValue</donottranslate></pre></div>
<div class="SeeAlso"><h2> </h2>
</div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_CreateOrUpdateTagToWorkspace_IVbsTags.htm`*
