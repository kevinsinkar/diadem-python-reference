---
title: "IExcelSheet.Find"
description: "Determines the position of a character or a character string in a worksheet of the open work folder. The search is executed rowwise."
---

# IExcelSheet.Find

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Find for Sheet

Determines the position of a character or a character string in a worksheet of the open work folder. The search is executed rowwise.

## Signature

```python
return_value = obj.Find(SearchText, [Row], [Column])
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
while (RetVal.Row>0) and (RetVal.Column>0):
    Count = Count +1
    Group.Properties.Add("Pos" + Cstr(Count), Cstr(RetVal.Row) + "," + cstr(RetVal.Column))
    RetVal = oSheet.Find("a", RetVal.Row, RetVal.Column+1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Find_IExcelSheet.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
