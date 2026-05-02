---
title: "IFixedWidthBlock.BlockLength"
description: "Specifies the number of values that a channel in the FixedWidthBlock contains. If the number is -1 , the block extends to the end of the file."
---

# IFixedWidthBlock.BlockLength

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: BlockLength for FixedWidthBlock

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the number of values that a channel in the FixedWidthBlock contains. If the number is -1 , the block extends to the end of the file.

## Signature

```python
obj.BlockLength
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  If the property <a href="../ifixedwidthchannelformatter-samplewidth/">SampleWidth</a> is not equal to 1 in a FixedWidthBlock, the <span class="Monospace">BlockLength</span> contains the number of lines in a text file.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oBlock.BlockLength = File.GetNextStringValue(eI32)

oChannelGroup = Root.ChannelGroups.Add(GroupName)
oChannelGroup.Properties.Add("BlockLength", oBlock.BlockLength)

oChannel.Formatter.CharacterCount = 4
oChannel.Formatter.SampleWidth = 4
oChannelGroup.Channels.AddDirectAccessChannel(Channel)

File.SkipLines(oBlock.BlockLength+1)
oBlock.Position = File.Position
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_BlockLength_IFixedWidthBlock.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
