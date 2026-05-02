---
title: "ITextStream"
description: "The TextStream object enables access to a file."
---

# ITextStream

!!! abstract "Object &middot; `Scripting.chm`"
    Object: TextStream

The TextStream object enables access to a file.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
fso = win32com.client.Dispatch("Scripting.FileSystemObject")
MyFile= fso.CreateTextFile(ScriptWritePath + "\testfile.txt", True)
MyFile.WriteLine("This is the first line")
MyFile.Close
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itextstream-atendofline/">AtEndOfLine</a> | <a href="../../properties/itextstream-atendofstream/">AtEndOfStream</a> | <a href="../../properties/itextstream-column/">Column</a> | <a href="../../properties/itextstream-line/">Line</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itextstream-close/">Close</a> | <a href="../../methods/itextstream-read/">Read</a> | <a href="../../methods/itextstream-readall/">ReadAll</a> | <a href="../../methods/itextstream-readline/">ReadLine</a> | <a href="../../methods/itextstream-skip/">Skip</a> | <a href="../../methods/itextstream-skipline/">SkipLine</a> | <a href="../../methods/itextstream-write/">Write</a> | <a href="../../methods/itextstream-writeblanklines/">WriteBlankLines</a> | <a href="../../methods/itextstream-writeline/">WriteLine</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ifile/">File</a>.<a href="../../methods/ifile-openastextstream/">OpenAsTextStream</a> | <a href="../ifilesystem3/">FileSystemObject</a>.<a href="../../methods/ifilesystem3-createtextfile/">CreateTextFile</a> | <a href="../ifilesystem3/">FileSystemObject</a>.<a href="../../methods/ifilesystem3-getstandardstream/">GetStandardStream</a> | <a href="../ifilesystem3/">FileSystemObject</a>.<a href="../../methods/ifilesystem3-opentextfile/">OpenTextFile</a> | <a href="../ifolder/">Folder</a>.<a href="../../methods/ifolder-createtextfile/">CreateTextFile</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/objects/Scripting_Objects_ITextStream.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
