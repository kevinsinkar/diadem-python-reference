---
title: "IVIRuntime.Description"
description: "Returns the description of a VI."
---

# IVIRuntime.Description

!!! abstract "Property &middot; `LVHelper.chm`"
    Property: Description for VIRuntime

Returns the description of a VI.

## Signature

```python
obj.Description
```

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test.vi")
dd.MsgBoxDisp(objVI.Description) #Get description
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p>
</div>
</div>

---

*Source: `LVHelper/properties/LVHelper_property_Description_IVIRuntime.htm`*
