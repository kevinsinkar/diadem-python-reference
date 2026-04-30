---
title: "IDataFileHeader.GroupChnSwap"
description: "Swaps two channels in one group in a TDM header file."
---

# IDataFileHeader.GroupChnSwap

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupChnSwap for DataFileHeader

Swaps two channels in one group in a TDM header file.

## Signature

```python
obj.GroupChnSwap(SourceChn, TargetChn)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  You only can swap channels within one group.</td></tr></table>
</div>

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyDataFileHeader.GroupChnSwap("1/1","1/4")
oMyDataFileHeader.close(True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupChnSwap_IDataFileHeader.htm`*
