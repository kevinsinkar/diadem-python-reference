---
title: "Open"
description: "Opens a communication channel to an interface in the script driver and initializes it with the current interface parameters."
---

# Open

!!! abstract "Function &middot; `Gfsvbsdr.chm`"
    Function: Open

Opens a communication channel to an interface in the script driver and initializes it with the current interface parameters.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oUDI.Open("COM", "COM1")
oUDI.ParamSet("BAUDRATE", "9600")
```

```python
oUDI.Open("NI GPIB", "DEV14")
```

---

*Source: `Gfsvbsdr/schntrb_open.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
