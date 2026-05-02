---
title: "IJsonParser"
description: "The JsonParser object provides methods for reading and writing JSON files in UTF8 format and for converting a JSON object into a Dictionary object and vice vers"
---

# IJsonParser

!!! abstract "Object &middot; `JsonParser.chm`"
    Object: JsonParser

The JsonParser object provides methods for reading and writing JSON files in UTF8 format and for converting a JSON object into a Dictionary object and vice versa. Use the CreateJsonParser command to create the JsonParser object.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oJsonParser = CreateJsonParser()
oMySubobject = CreateObject("Scripting.Dictionary")
oMyMainObject = CreateObject("Scripting.Dictionary")

oMySubobject.Add("intVal", CInt(1))
oMySubobject.Add("doubleVal", CDbl(1.2))
oMySubobject.Add("stringVal", "TextA")

oMyMainObject.Add("subobject", oMySubobject)
oMyMainObject.Add("array", Array("TextB", 5678, True))
oMyMainObject.Add("timestamp", oJsonParser.CreateDateTime(Now, True))

sJsonString = oJsonParser.Serialize(oMyMainObject, True)
LogFileWrite(sJsonString)
```

```python
oJsonParser = CreateJsonParser()
sJsonString = "{""path"":""task.id.592d7b9e-7816-4517-973d-ef03cc814e35"",""current"":{""timestamp"":""2018-11-27T12:33:27Z""," + """value"":{""type"":1,""value"":""47""}},""aggregates"":{""count"":1,""avg"":47.0,""min"":""47"",""max"":""47""}}"
oJsonParser.Deserialize(sJsonString, oVbsObject)
sPath = oVbsObject.Item("path")
oAggregates = oVbsObject.Item("aggregates")
sAvg = oAggregates.Item("avg")
sJsonString = oJsonParser.Serialize(oVbsObject, True)  # make pretty for viewing
LogFileWrite(sJsonString)
LogFileWrite("path: " + sPath + "\r\n" + "avg: " + sAvg)
```

```python
oJsonParser = CreateJsonParser()
oMyMainObject = CreateObject("Scripting.Dictionary")

oMyMainObject.Add("array", Array("TextB", 5678, True))
oMyMainObject.Add("timestamp", oJsonParser.CreateDateTime(Now, True))
sJsonString = oJsonParser.Serialize(oMyMainObject, True)
oJsonParser.WriteFile(sJsonString, DataWritePath + "JsonObject.json")
LogfileWrite(DataWritePath + "JsonObject.json")
```

```python
oJsonParser = CreateJsonParser()
sFile = DataWritePath + "JsonObject.json"
sJsonString = oJsonParser.ReadFile(sFile)
oJsonParser.Deserialize(sJsonString, oVbsVariant)
# select VarType(oVbsVariant)
# case vbObject
LogfileWrite("Dictionary size: " + oVbsVariant.Count)
# case vbArray + vbVariant
LogfileWrite("Array size: " + UBound(oVbsVariant)+1)
# case else
dd.MsgBox("Some other data type")
LogfileWrite(sJsonString)
```

## Members

<div markdown="1">
<div class="Methods">
<h2>Methods</h2>
<p><a href="../../methods/ijsonparser-createdatetime/">CreateDateTime</a> | <a href="../../methods/ijsonparser-deserialize/">Deserialize</a> | <a href="../../methods/ijsonparser-parsedatetime/">ParseDateTime</a> | <a href="../../methods/ijsonparser-readfile/">ReadFile</a> | <a href="../../methods/ijsonparser-serialize/">Serialize</a> | <a href="../../methods/ijsonparser-writefile/">WriteFile</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `JsonParser/objects/JsonParser_Objects_IJsonParser.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
