---
title: "ApplicationPreviewFeatureID"
description: "Specifies the ID of a preview feature."
---

# ApplicationPreviewFeatureID

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ApplicationPreviewFeatureID

Specifies the ID of a preview feature.

## Python example

```python
dd.ApplicationEnablePreviewFeature = True
for I in range( 1, dd.ApplicationPreviewFeatureCount+1):
    print("ID " , dd.ApplicationPreviewFeatureID(I) , "\r\n" , "Title: " , dd.ApplicationPreviewFeatureTitle(I) , "\r\n" , "Enabled: " , dd.ApplicationPreviewFeatureEnabled(I) )
```

---

*Source: `VarOff/ApplicationPreviewFeatureID.htm`*
