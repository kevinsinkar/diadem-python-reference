---
title: "IJsonParser.Deserialize"
description: "Converts a JSON object into a Dictionary Object or a VBS Array . The items of the dictionary object can contain dictionary objects, VBS arrays , and primitive d"
---

# IJsonParser.Deserialize

!!! abstract "Method &middot; `JsonParser.chm`"
    Method: Deserialize for JsonParser

Converts a JSON object into a Dictionary Object or a VBS Array . The items of the dictionary object can contain dictionary objects, VBS arrays , and primitive data types, such as strings, integer, double, and boolean.

## Signature

```python
obj.Deserialize(Json, Value)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oJsonParser = CreateJsonParser()
sJsonString = "{""path"":""task.id.592d7b9e-7816-4517-973d-ef03cc814e35"",""current"":{""timestamp"":""2018-11-27T12:33:27Z""," + """value"":{""type"":1,""value"":""47""}},""aggregates"":{""count"":1,""avg"":47.0,""min"":""47"",""max"":""47""}}"
oJsonParser.Deserialize(sJsonString, oVbsObject)
sPath = oVbsObject.Item("path")
oAggregates = oVbsObject.Item("aggregates")
sAvg = oAggregates.Item("avg")
sJsonString = oJsonParser.Serialize(oVbsObject, True) ' make pretty for viewing
LogFileWrite(sJsonString)
LogFileWrite("path: " + sPath + vbCRLF + "avg: " + sAvg)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `JsonParser/methods/JsonParser_method_Deserialize_IJsonParser.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
