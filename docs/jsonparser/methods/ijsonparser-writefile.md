---
title: "IJsonParser.WriteFile"
description: "Saves a text to an UTF-8 file."
---

# IJsonParser.WriteFile

!!! abstract "Method &middot; `JsonParser.chm`"
    Method: WriteFile for JsonParser

Saves a text to an UTF-8 file.

## Signature

```python
obj.WriteFile(String, Filename)
```

## Python example

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

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `JsonParser/methods/JsonParser_method_WriteFile_IJsonParser.htm`*
