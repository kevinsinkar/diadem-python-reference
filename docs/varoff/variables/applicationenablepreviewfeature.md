---
title: "ApplicationEnablePreviewFeature"
description: "Specifies whether DIAdem activates soon available functions."
---

# ApplicationEnablePreviewFeature

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ApplicationEnablePreviewFeature

Specifies whether DIAdem activates soon available functions.

## Python example

```python
dd.ApplicationEnablePreviewFeature = True
for I in range( 1, dd.ApplicationPreviewFeatureCount+1):
    print("ID " , dd.ApplicationPreviewFeatureID(I) , "\r\n" , "Title: " , dd.ApplicationPreviewFeatureTitle(I) , "\r\n" , "Enabled: " , dd.ApplicationPreviewFeatureEnabled(I) )
```

---

*Source: `VarOff/ApplicationEnablePreviewFeature.htm`*
