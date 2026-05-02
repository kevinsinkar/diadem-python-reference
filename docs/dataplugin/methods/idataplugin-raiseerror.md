---
title: "IDataPlugin.RaiseError"
description: "Aborts loading with an error message."
---

# IDataPlugin.RaiseError

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: RaiseError for DataPlugin

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Aborts loading with an error message.

## Signature

```python
obj.RaiseError([ErrMsg])
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Begin Header¶
Name: XShift¶
Name: YShift¶
End Header¶
0.162820 : 0.001234¶
0.162821 : 0.002398¶
0.162822 : 0.001296¶
0.162823 : 0.001628¶
0.162824 : 0.001683¶
0.162825 : 0.008734¶
```

```python
File.Formatter.LineFeeds  = "\n"
File.Formatter.Delimiters = ":"
File.Formatter.TrimCharacters = " "

ReDim ChNames(1)

TagName = File.GetNextStringValue(eString)
File.SkipLine()
if TagValue !="Begin Header":
    RaiseError

Do
TagName = File.GetNextStringValue(eString)
TagValue= File.GetNextStringValue(eString)
File.SkipLine()
if TagName == "Name":
    ChNames(UBound(ChNames)) = TagValue
    ReDim Preserve ChNames(UBound(ChNames)+1)
if (TagName is None):
    RaiseError("File corrupt or not xyz format.")


for i in range(1, UBound(ChNames)-1 + 1):
    oChn = oBlock.Channels.Add(ChannelNames(i), eR64)
    oGrp.Channels.AddDirectAccessChannel(oChn)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_RaiseError_IDataPlugin.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
