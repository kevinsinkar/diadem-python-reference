---
title: "IVIRuntime.HelpPath"
description: "Returns the path for the HTML file ( *.htm or *.html ) or the help file ( *.chm or *.hlp ) for which the VI contains a link. If the path leads to a compiled hel"
---

# IVIRuntime.HelpPath

!!! abstract "Property &middot; `LVHelper.chm`"
    Property: HelpPath for VIRuntime

Returns the path for the HTML file ( *.htm or *.html ) or the help file ( *.chm or *.hlp ) for which the VI contains a link. If the path leads to a compiled help file, the HelpTag property enables the selection of a topic in the help file. This property is similar to the Help path textbox from the Documentation page in the LabVIEW VI properties dialog field.

## Signature

```python
obj.HelpPath
```

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test.vi")
dd.MsgBoxDisp(objVI.HelpPath) #Get HelpPath
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

*Source: `LVHelper/properties/LVHelper_property_HelpPath_IVIRuntime.htm`*
