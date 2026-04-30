---
title: "IJsonParser.Serialize"
description: "Converts a Dictionary Object or a VBS Array into a JSON object. The items of the dictionary object can contain dictionary objects, VBS arrays , and primitive da"
---

# IJsonParser.Serialize

!!! abstract "Method &middot; `JsonParser.chm`"
    Method: Serialize for JsonParser

Converts a Dictionary Object or a VBS Array into a JSON object. The items of the dictionary object can contain dictionary objects, VBS arrays , and primitive data types, such as strings, integer, double, and boolean.

## Signature

```python
sSerialize = Object.Serialize(Value, [PrettifyJson])
```

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

sJsonString  = oJsonParser.Serialize(oMyMainObject, True)
dd.LogFileWrite(sJsonString)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `JsonParser/methods/JsonParser_method_Serialize_IJsonParser.htm`*
