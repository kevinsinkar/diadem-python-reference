---
title: "ScriptScope"
description: "Specifies the name space of a script. By default the ScriptCode variable contains an empty text."
---

# ScriptScope

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ScriptScope

Specifies the name space of a script. By default the ScriptCode variable contains an empty text.

## Python example

```python
dd.ScriptScope = "Test"
dd.ScriptInclude("Test.vbs",dd.ScriptScope)
dd.ScriptScope = "GlobalLib"
dd.ScriptInclude("MyLib.vbs",dd.ScriptScope)
MyResult = Test.MyFunc
MyOtherResult = GlobalLib.MyFunc
```

---

*Source: `VarOff/ScriptScope.htm`*
