---
title: "ApplicationPreviewFeatureTitle"
description: "Specifies the title of a preview feature."
---

# ApplicationPreviewFeatureTitle

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ApplicationPreviewFeatureTitle

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.BoolVarSet('ApplicationEnablePreviewFeature', ...)   # instead of dd.ApplicationEnablePreviewFeature = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Specifies the title of a preview feature.

## Python example

```python
dd.ApplicationEnablePreviewFeature = True
for I in range( 1, dd.ApplicationPreviewFeatureCount+1):
    print("ID " , dd.ApplicationPreviewFeatureID(I) , "\r\n" , "Title: " , dd.ApplicationPreviewFeatureTitle(I) , "\r\n" , "Enabled: " , dd.ApplicationPreviewFeatureEnabled(I) )
```

---

*Source: `VarOff/ApplicationPreviewFeatureTitle.htm`*
