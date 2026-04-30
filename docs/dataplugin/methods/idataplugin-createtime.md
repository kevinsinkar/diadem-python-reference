---
title: "IDataPlugin.CreateTime"
description: "Creates a time value. You can assign this time value to a value in a time channel or to a property."
---

# IDataPlugin.CreateTime

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: CreateTime for DataPlugin

Creates a time value. You can assign this time value to a value in a time channel or to a property.

## Signature

```python
return_value = obj.CreateTime(Year, Month, Day, Hour, Minute, Second, Millisecond, Microsecond, Nanosecond)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>You can use VBS date/time functions instead of <span class="Monospace">CreateTime</span>. However, milliseconds, microseconds, and nanoseconds are not supported with these VBS functions.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.Properties.Add("Time", CreateTime(2004,6,17,10,0,0,0,0,0))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_CreateTime_IDataPlugin.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
