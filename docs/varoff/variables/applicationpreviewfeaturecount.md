---
title: "ApplicationPreviewFeatureCount"
description: "Specifies the number of preview features."
---

# ApplicationPreviewFeatureCount

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ApplicationPreviewFeatureCount

Specifies the number of preview features.

## Python example

```python
dd.ApplicationEnablePreviewFeature = True
for I in range( 1, dd.ApplicationPreviewFeatureCount+1):
    print("ID " , dd.ApplicationPreviewFeatureID(I) , "\r\n" , "Title: " , dd.ApplicationPreviewFeatureTitle(I) , "\r\n" , "Enabled: " , dd.ApplicationPreviewFeatureEnabled(I) )
```

---

*Source: `VarOff/ApplicationPreviewFeatureCount.htm`*
