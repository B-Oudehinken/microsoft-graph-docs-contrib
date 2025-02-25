---
title: "macOSMicrosoftEdgeApp resource type"
description: "Contains properties and inherited properties for the macOS Microsoft Edge App."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 09/13/2024
---

# macOSMicrosoftEdgeApp resource type

Namespace: microsoft.graph

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Contains properties and inherited properties for the macOS Microsoft Edge App.


Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List macOSMicrosoftEdgeApps](../api/intune-apps-macosmicrosoftedgeapp-list.md)|[macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) collection|List properties and relationships of the [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) objects.|
|[Get macOSMicrosoftEdgeApp](../api/intune-apps-macosmicrosoftedgeapp-get.md)|[macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md)|Read properties and relationships of the [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object.|
|[Create macOSMicrosoftEdgeApp](../api/intune-apps-macosmicrosoftedgeapp-create.md)|[macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md)|Create a new [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object.|
|[Delete macOSMicrosoftEdgeApp](../api/intune-apps-macosmicrosoftedgeapp-delete.md)|None|Deletes a [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md).|
|[Update macOSMicrosoftEdgeApp](../api/intune-apps-macosmicrosoftedgeapp-update.md)|[macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md)|Update the properties of a [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the entity. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|channel|[microsoftEdgeChannel](../resources/intune-apps-microsoftedgechannel.md)|The channel to install on target devices. Possible values are: `dev`, `beta`, `stable`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSMicrosoftEdgeApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String",
  "channel": "String"
}
```
