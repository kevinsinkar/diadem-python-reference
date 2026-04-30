---
title: "IVIRuntime.GetControlVariant"
description: "Returns the value of an output. The return value type is a variant. VBS converts variant values automatically into the respective data format. Use the GetContro"
---

# IVIRuntime.GetControlVariant

!!! abstract "Method &middot; `LVHelper.chm`"
    Method: GetControlVariant for VIRuntime

Returns the value of an output. The return value type is a variant. VBS converts variant values automatically into the respective data format. Use the GetControlValue command to receive the data in the original data type.

## Signature

```python
vGetControlVariant = Object.GetControlVariant(OutputName)
```

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test")
objVI.run(True)
dd.MsgBoxDisp(objVI.GetControlVariant("OutPut1"))
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.loadvi(dd.AutoActPath + "Test")
objVI.Run(True)
MyMatrix = objVI.GetControlVariant("MyStringMatrix")
for I in range( 0, len(MyMatrix,1)-1):
    for J in range( 0, len(MyMatrix,2)-1):
        strOutput = strOutput + I + " Row " + j + " Column: " + MyMatrix(I, J) + "\r\n"
dd.MsgBoxDisp(strOutput)
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.loadvi(dd.AutoActPath + "Test")

objVI.Run(True)
aMyCluster = objVI.GetControlVariant("MyCluster")
strOutput = aMyCluster(0) + "\r\n" #Get the value MyI32Scalar
MyMatrix= aMyCluster(1) #Get the matrix values MyStringMatrix
for I in range( 0, len(MyMatrix,1)-1):
    for J in range( 0, len(MyMatrix,2)-1):
        strOutput = strOutput + MyMatrix(I, J) + "\r\n"
dd.MsgBoxDisp(strOutput)
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.loadvi(dd.AutoActPath + "Test")

objVI.Run(True)

WaveFormT = objVI.GetControlVariant("MyWaveformOut")

strOutput = ""
strOutput = strOutput + "T0: " + WaveFormT(0) + "\r\n"
strOutput = strOutput + "dT: " + WaveFormT(1) + "\r\n"

AttributesT = WaveFormT(2)
for I in range( 0, len(AttributesT,1)-1):
    strOutput = strOutput + "Attribute: " + AttributesT(I, 0) + " = " + AttributesT(I, 0) + "\r\n"

ValuesT = WaveFormT(3)
for I in range( 0, len(ValuesT)-1):
    strOutput = strOutput + "Values: " + ValuesT(I) + "\r\n"
dd.MsgBoxDisp (strOutput)

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

*Source: `LVHelper/methods/LVHelper_method_GetControlVariant_IVIRuntime.htm`*
