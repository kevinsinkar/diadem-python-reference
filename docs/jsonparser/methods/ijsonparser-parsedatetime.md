---
title: "IJsonParser.ParseDateTime"
description: "Converts a date according to ISO 8601 into a variable with the subtype Date ."
---

# IJsonParser.ParseDateTime

!!! abstract "Method &middot; `JsonParser.chm`"
    Method: ParseDateTime for JsonParser

Converts a date according to ISO 8601 into a variable with the subtype Date .

## Signature

```python
return_value = obj.ParseDateTime(String, LocalTime)
```

## Python example

```python
oJsonParser = dd.CreateJsonParser()
sJsonDateTimeTag = "{\"timestamp\":\"2018-11-27T12:33:27Z\"}"
oJsonParser.Deserialize(sJsonDateTimeTag, oVbsObject)
sVbsDictItem = oVbsObject("timestamp")
VbsDate = oJsonParser.ParseDateTime(sVbsDictItem,True)
dd.LogFileWrite("Local Time: " + str(VbsDate))
VbsDate = oJsonParser.ParseDateTime(sVbsDictItem,False)
dd.LogFileWrite("UTC Time: " + str(VbsDate))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `JsonParser/methods/JsonParser_method_ParseDateTime_IJsonParser.htm`*
