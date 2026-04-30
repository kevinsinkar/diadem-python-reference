---
title: "ApplicationPreviewFeatureEnabled"
description: "Specifies whether a preview feature is active or inactive."
---

# ApplicationPreviewFeatureEnabled

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ApplicationPreviewFeatureEnabled

Specifies whether a preview feature is active or inactive.

## Python example

```python
dd.ApplicationEnablePreviewFeature = True
for I in range( 1, dd.ApplicationPreviewFeatureCount+1):
    print("ID " , dd.ApplicationPreviewFeatureID(I) , "\r\n" , "Title: " , dd.ApplicationPreviewFeatureTitle(I) , "\r\n" , "Enabled: " , dd.ApplicationPreviewFeatureEnabled(I) )
```

---

*Source: `VarOff/ApplicationPreviewFeatureEnabled.htm`*
