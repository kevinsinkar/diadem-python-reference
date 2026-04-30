---
title: "ILVRuntime"
description: "The LVRuntime object enables access to LabVIEW. Use the LVRuntime object to load and to execute VIs. The LVRuntime object is available as a global object in scr"
---

# ILVRuntime

!!! abstract "Object &middot; `LVHelper.chm`"
    Object: LVRuntime

The LVRuntime object enables access to LabVIEW. Use the LVRuntime object to load and to execute VIs. The LVRuntime object is available as a global object in scripts and in dialog boxes. Do not create an object or a variable with the name LVRuntime , because that overwrites the Navigator object.

## Python example

```python
# Initialize the LVRuntime
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)

# Load "Test.vi"
objVIVIT = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test")

# Call the VI
objVI.Run(True)
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

## Members

<div markdown="1">
<div class="Properties"><div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ilvruntime-version/">Version</a></p>
</div>
</div>
<div class="Methods"><div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ilvruntime-deinit/">DeInit</a> | <a href="../../methods/ilvruntime-init/">Init</a> | <a href="../../methods/ilvruntime-loadvi/">LoadVI</a></p>
</div>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p>
</div>
</div>

---

*Source: `LVHelper/objects/LVHelper_Objects_ILVRuntime.htm`*
