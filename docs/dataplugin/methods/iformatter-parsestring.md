---
title: "IFormatter.ParseString"
description: "Parses a text into the specified data type."
---

# IFormatter.ParseString

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: ParseString for Formatter

Parses a text into the specified data type.

## Signature

```python
vParseString = Object.ParseString(sPString, eDataType)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>If the text is converted to a numeric type, only the first number in the text is used. If the text does not contain a number, the return value is NULL.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The conversion uses the current format.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>If the data types eU16 or eU32 are returned, the return value <em>ConvString</em> can cause problems in VBS.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eNoType` | 0 | Not defined |
| `eI8` | 1 | 8-bit integer values |
| `eI16` | 2 | 16-bit integer values |
| `eI32` | 3 | 32-bit integer values |
| `eI64` | 4 | 64-bit integer values |
| `eByte` | 5 | Byte |
| `eU16` | 6 | 16-bit unsigned integer |
| `eU32` | 7 | 32-bit unsigned integer |
| `eU64` | 8 | 64-bit unsigned integer |
| `eR32` | 9 | 32-bit real values |
| `eR64` | 10 | 64-bit real values |
| `eString` | 23 | Text |
| `eEnum` | 24 | Enumeration |
| `eTime` | 30 | Time values |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
if (rChnCount is None):
    RaiseError
if (rChnDelta is None):
    RaiseError
if (rChnMin is None):
    RaiseError
```

```python
if (oMyDate is None):
    RaiseError
Root.Properties.Add("Year/Month", oMyDate.Year&"/"oMyDate.Month)
```

---

*Source: `DataPlugin/Methods/DataPlugin_method_ParseString_IFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
