---
title: "IVIRuntime.Version"
description: "Returns the LabVIEW version with which the VI was generated."
---

# IVIRuntime.Version

!!! abstract "Property &middot; `LVHelper.chm`"
    Property: Version for VIRuntime

Returns the LabVIEW version with which the VI was generated.

## Signature

```python
obj.Version
```

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test.vi")
dd.MsgBoxDisp(objVI.Version) #Get version
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

*Source: `LVHelper/properties/LVHelper_property_Version_IVIRuntime.htm`*
