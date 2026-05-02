---
title: "Parse"
description: "Accesses the data that DIAdem reads from a UDI device, using the Read command in the script driver . The function especially supports access to binary data."
---

# Parse

!!! abstract "Function &middot; `Gfsvbsdr.chm`"
    Function: Parse

Accesses the data that DIAdem reads from a UDI device, using the Read command in the script driver . The function especially supports access to binary data.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
vData = oUDI.Read()  # Read all available data from the UDI object
vValue = Parse(vData,"%2L")  # Read 2 bytes from vData and return the read value to the vData variable
```

```python
vData = oUDI.Read()  # Read all available data from the UDI object
vArray = oUDI.Parse(vData,"%2L%4L")  # Read a total of 6 bytes from vData and return 2 values to the field
for L in range(1, UBound(vArray) + 1):  # Display the two values in a message box
    dd.MsgBox(CStr(vArray(L))
```

```python
vData = oUDI.Read()  # Read all available data from the UDI object
vArray = oUDI.Parse(vData,"%2L<Trigger>%4L<Temperature>")  # Read a total of 6 bytes from vData and return 2 values to the vArray field
vScaledValue = oUDI.NamedValueGet("Temperature ")*0.01
dd.MsgBox(vScaledValue)  # Directly accesses the specified "Temperature" value and displays the scaled value in a message box
```

---

*Source: `Gfsvbsdr/parse.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
