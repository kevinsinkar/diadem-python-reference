---
title: "IJsonParser.CreateDateTime"
description: "Converts a VBS variable with the subtype Date into a date according to ISO 8601."
---

# IJsonParser.CreateDateTime

!!! abstract "Method &middot; `JsonParser.chm`"
    Method: CreateDateTime for JsonParser

Converts a VBS variable with the subtype Date into a date according to ISO 8601.

## Signature

```python
sCreateDateTime = Object.CreateDateTime(Date, LocalTime)
```

## Python example

```python
import win32com
import datetime
oJsonParser = dd.CreateJsonParser()
oMyDict = win32com.client.Dispatch("Scripting.Dictionary")
oMyDict.Add("timestamp", oJsonParser.CreateDateTime(datetime.datetime.now(),True))
sJsonDateTimeTag = oJsonParser.Serialize(oMyDict, True)
dd.LogFileWrite(sJsonDateTimeTag)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `JsonParser/methods/JsonParser_method_CreateDateTime_IJsonParser.htm`*
