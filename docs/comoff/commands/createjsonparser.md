---
title: "CreateJsonParser"
description: "Creates a JsonParser object with methods for reading and writing JSON files in UTF8 format and for converting a JSON object into a Dictionary object or a VBS ar"
---

# CreateJsonParser

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CreateJsonParser

Creates a JsonParser object with methods for reading and writing JSON files in UTF8 format and for converting a JSON object into a Dictionary object or a VBS array , or vice versa.

## Signature

```python
return_value = dd.CreateJsonParser()
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>A <a href="../../../jsonparser/objects/ijsonparser/">JsonParser object</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
import win32com
import datetime
oJsonParser = dd.CreateJsonParser()
oMySubobject = win32com.client.Dispatch("Scripting.Dictionary")
oMyMainObject = win32com.client.Dispatch("Scripting.Dictionary")

oMySubobject.Add("intVal", int(1))
oMySubobject.Add("doubleVal", float(1.2))
oMySubobject.Add("stringVal", "TextA")

oMyMainObject.Add("subobject", oMySubobject)
oMyMainObject.Add("array", ["TextB", 5678, True])
oMyMainObject.Add("timestamp", oJsonParser.CreateDateTime(datetime.datetime.now(), True))

sJsonString = oJsonParser.Serialize(oMyMainObject, True)
dd.LogFileWrite(sJsonString)
```

```python
oJsonParser = dd.CreateJsonParser()
sJsonString = "{\"path\":\"task.id.592d7b9e-7816-4517-973d-ef03cc814e35\",\"current\":{\"timestamp\":\"2018-11-27T12:33:27Z\"," + "\"value\":{\"type\":1,\"value\":\"47\"}},\"aggregates\":{\"count\":1,\"avg\":47.0,\"min\":\"47\",\"max\":\"47\"}}"
oJsonParser.Deserialize(sJsonString, oVbsObject)
sPath = oVbsObject.Item("path")
oAggregates = oVbsObject.Item("aggregates")
sAvg = oAggregates.Item("avg")
sJsonString = oJsonParser.Serialize(oVbsObject, True) # make pretty for viewing
dd.LogFileWrite(sJsonString)
dd.LogFileWrite("path: " +  sPath + "\r\n" + "avg: " + sAvg)
```

```python
import win32com
import datetime
oJsonParser = dd.CreateJsonParser()
oMyMainObject = win32com.client.Dispatch("Scripting.Dictionary")

oMyMainObject.Add("array", ["TextB", 5678, True])
oMyMainObject.Add("timestamp", oJsonParser.CreateDateTime(datetime.datetime.now(), True))
sJsonString = oJsonParser.Serialize(oMyMainObject, True)
oJsonParser.WriteFile(sJsonString, dd.DataWritePath + "JsonObject.json")
dd.LogfileWrite(dd.DataWritePath + "JsonObject.json")
```

```python
oJsonParser = dd.CreateJsonParser()
sFile = dd.DataWritePath + "JsonObject.json"
sJsonString = oJsonParser.ReadFile(sFile)
oJsonParser.Deserialize(sJsonString, oVbsVariant)
select_variable_0 = VarType(oVbsVariant)
if (select_variable_0 == vbObject) :
    dd.LogfileWrite("Dictionary size: "  + oVbsVariant.Count)
elif (select_variable_0 == vbArray + vbVariant) :
    dd.LogfileWrite("Array size: "  + len(oVbsVariant)+1)
else:
    print("Some other data type")
dd.LogfileWrite(sJsonString)
```

---

*Source: `ComOff/CreateJsonParser.htm`*
