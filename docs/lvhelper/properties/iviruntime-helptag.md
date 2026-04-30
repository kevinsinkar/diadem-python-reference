---
title: "IVIRuntime.HelpTag"
description: "Returns an index keyword or an HTML filename for a topic in the compiled help file to which the VI contains a link. For *.chm files this property can be an HTML"
---

# IVIRuntime.HelpTag

!!! abstract "Property &middot; `LVHelper.chm`"
    Property: HelpTag for VIRuntime

Returns an index keyword or an HTML filename for a topic in the compiled help file to which the VI contains a link. For *.chm files this property can be an HTML filename or an index keyword. For *.hlp files this property can be an index keyword. This property is similar to the Help tag textbox from the Documentation page in the LabVIEW VI properties dialog field.

## Signature

```python
obj.HelpTag
```

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test.vi")
dd.MsgBoxDisp(objVI.HelpTag) #Get HelpTag
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

*Source: `LVHelper/properties/LVHelper_property_HelpTag_IVIRuntime.htm`*
