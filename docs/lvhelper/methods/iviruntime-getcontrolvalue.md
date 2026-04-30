---
title: "IVIRuntime.GetControlValue"
description: "Returns the output value while retaining the original data type. This means the type of the return value is the same as the value type in LabVIEW. You cannot al"
---

# IVIRuntime.GetControlValue

!!! abstract "Method &middot; `LVHelper.chm`"
    Method: GetControlValue for VIRuntime

Returns the output value while retaining the original data type. This means the type of the return value is the same as the value type in LabVIEW. You cannot always process the type-safe values in VBS functions, because the functions usually expect variant values. Use the GetControlVariant method to receive variant values. You can use the property Value for Property or the function ArrayToChannels to edit, for example, the original data in DIAdem. You can use the ChntoValue command to convert channels into variant arrays or you can use the VariantToChn command to convert variant data arrays into channels.

## Signature

```python
vGetControlValue = Object.GetControlValue(OutputName)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  You only can read out LabVIEW waveforms and LabVIEW clusters with the <a href="../iviruntime-getcontrolvariant/">GetControlVariant</a> command.</td></tr></table>
</div>

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test.vi")
objVI.Run(True)
dd.MsgBoxDisp(objVI.GetControlValue("OutPut1"))
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

*Source: `LVHelper/methods/LVHelper_method_GetControlValue_IVIRuntime.htm`*
