---
title: "ScriptScope"
description: "Specifies the name space of a script. By default the ScriptCode variable contains an empty text."
---

# ScriptScope

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ScriptScope

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.IntegerVarSet('ScriptScope', ...)   # instead of dd.ScriptScope = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

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
