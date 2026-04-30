---
title: "Methods (LabVIEW Helper)"
---

# Methods

8 methods from `LVHelper.chm`.

| Name | Summary |
| --- | --- |
| [`ILVRuntime.DeInit`](ilvruntime-deinit.md) | Unloads the LabVIEW Run Time Library and disconnects LabVIEW. |
| [`ILVRuntime.Init`](ilvruntime-init.md) | Loads the LabVIEW Runtime Library and connects LabVIEW. |
| [`ILVRuntime.LoadVI`](ilvruntime-loadvi.md) | Loads a VI. |
| [`ITerminals.Item`](iterminals-item.md) | Returns the Terminal object for a specific index of a VI. A terminal is an input terminal or an output terminal of a VI. |
| [`IVIRuntime.GetControlValue`](iviruntime-getcontrolvalue.md) | Returns the output value while retaining the original data type. This means the type of the return value is the same as the value type in LabVIEW. You cannot always process the type-safe values in VBS functions, because the functions usually expect variant values. Use the GetControlVariant method to receive variant values. You can use the property Value for Property or the function ArrayToChannels to edit, for example, the original data in DIAdem. You can use the ChntoValue command to convert channels into variant arrays or you can use the VariantToChn command to convert variant data arrays into channels. |
| [`IVIRuntime.GetControlVariant`](iviruntime-getcontrolvariant.md) | Returns the value of an output. The return value type is a variant. VBS converts variant values automatically into the respective data format. Use the GetControlValue command to receive the data in the original data type. |
| [`IVIRuntime.Run`](iviruntime-run.md) | Synchronous start of a LabVIEW VI which means DIAdem waits until the VI stops before DIAdem executes a script. |
| [`IVIRuntime.SetControlValue`](iviruntime-setcontrolvalue.md) | Specifies the value of an input. Depending on the input you forward the value as a single value or as a matrix. |
