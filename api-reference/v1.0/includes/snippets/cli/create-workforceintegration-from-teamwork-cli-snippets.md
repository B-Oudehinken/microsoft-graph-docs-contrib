---
description: "Automatically generated file. DO NOT MODIFY"
---

```bash


mgc teamwork workforce-integrations create --body '{\
  "displayName": "ABCWorkforceIntegration",\
  "apiVersion": 1,\
  "isActive": true,\
  "encryption": {\
    "protocol": "sharedSecret",\
    "secret": "My Secret"\
  },\
  "url": "https://ABCWorkforceIntegration.com/Contoso/",\
  "supportedEntities": "Shift,SwapRequest",\
  "eligibilityFilteringEnabledEntities": "SwapRequest"\
}\
'

```