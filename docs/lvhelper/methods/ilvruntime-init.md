---
title: "ILVRuntime.Init"
description: "Loads the LabVIEW Runtime Library and connects LabVIEW."
---

# ILVRuntime.Init

!!! abstract "Method &middot; `LVHelper.chm`"
    Method: Init for LVRuntime

Loads the LabVIEW Runtime Library and connects LabVIEW.

## Signature

```python
bInit = Object.Init(Version)
```

## Python example

```python
# Initialize the LVRuntime
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)

# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI("Test")

# Call the VI
objVI.Run(True)
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

*Source: `LVHelper/methods/LVHelper_method_Init_ILVRuntime.htm`*
