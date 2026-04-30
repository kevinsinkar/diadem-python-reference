---
title: "IJsonParser.ReadFile"
description: "Reads in a string from a JSON file in UTF-8 format."
---

# IJsonParser.ReadFile

!!! abstract "Method &middot; `JsonParser.chm`"
    Method: ReadFile for JsonParser

Reads in a string from a JSON file in UTF-8 format.

## Signature

```python
sReadFile = Object.ReadFile(Filename)
```

## Python example

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `JsonParser/methods/JsonParser_method_ReadFile_IJsonParser.htm`*
