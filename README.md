# Enkadia-Alloy-Project
Respository for the planning and development of the Alloy inventory control application

### This is a document and project management repository only

#### Flex API Notes

*Working on a lightweight application for location and quick reference (Pinpoint)*

#### General Notes
*The API documentation uses names such as locationId, notesId, modelId. In most cases these names don't exist in the record, but instead are the unique Id.



#### Useful Methods
- Business location - get locationID for Inspirmedia - Main (used for some lookups) *this should be declared a constant in appdev for IM, since there is only one location*
- Global search - can search by text, barcode, various categories (e.g. inventory-model, contact, serial, all ...)
- Inventory - includes a global get using modelId

***Sample response from Inventory - /api/inventory-model/{modelId}***
```{
  "id": "ce98d110-5c87-11e5-9666-00259031aaaa",
  "name": "Shapeshifter C2",
  "createdByUserId": "3fd5a940-5024-11e5-992f-00259031aaaa",
  "createdDate": "2015-09-16T15:30:06",
  "lastEditUserId": "6a83b8b3-f653-49d1-ae60-199dc283cb75",
  "lastEditDate": "2023-10-10T04:26:57",
  "code": null,
  "shortName": "Shapeshifter C2",
  "preferredDisplayString": "Shapeshifter C2",
  "narrativeDescription": "",
  "barcode": "00583",
  "rfidTag": null,
  "deleted": false,
  "deletedByUserId": null,
  "deletedByDate": null,
  "presumedMissing": false,
  "lineMuteByDefault": false,
  "noteMuteByDefault": false,
  "numberSequence": 583,
  "catalogueItem": false,
  "publicCatalogueItem": false,
  "number": "00583",
  "discountable": true,
  "maxDiscount": null,
  "barcodeLabel": null,
  "externalNumber": null,
  "referenceData": {
    "canViewInventoryPricingPermission": true,
    "tagIds": [],
    "icon": {
      "id": "21df2fe0-9b63-11e4-bda6-00259031aaaa",
      "name": "Elation Blade",
      "category": "Lighting",
      "imageId": "21de6c90-9b63-11e4-bda6-00259031aaaa",
      "domainId": "icon"
    },
    "isTrackDepreciation": false,
    "preset": {
      "id": "serialized-model-with-acc",
      "name": "Serialized Model with Accessories"
    },
    "scheduledMaintenanceEnabled": false,
    "linearUnit": {
      "id": "917184f0-c5c2-11df-9467-00e08175e43e",
      "name": "Inch",
      "namePlural": "Inches",
      "defaultLinearUnit": true,
      "defaultWeightUnit": false,
      "countUnit": true,
      "domainId": "unit-of-measure"
    },
    "additionalGroupIdentityList": [],
    "imageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/e9a875a0-5c87-11e5-9666-00259031aaaa",
    "canManageInventoryPricingPermission": true,
    "averageCost": 2250,
    "weightUnit": {
      "id": "7015642c-abee-11df-b8d5-00e08175e43e",
      "name": "Pound",
      "namePlural": "Pounds",
      "defaultLinearUnit": false,
      "defaultWeightUnit": true,
      "countUnit": true,
      "domainId": "unit-of-measure"
    },
    "group": {
      "id": "a2ff8fe0-8ac7-11e4-aebc-00259031aaaa",
      "name": "Moving Head",
      "fullDisplayString": "Lighting > Moving Head",
      "globalSortOrdinal": 133,
      "domainId": "inventory-group"
    }
  },
  "imported": false,
  "tagIds": null,
  "shortHand": null,
  "size": null,
  "trackedBySerialUnit": true,
  "container": true,
  "virtualModel": false,
  "serializedContents": false,
  "freePickContainer": false,
  "contentsAvailable": false,
  "contentsPermanent": false,
  "replacementCost": 2700,
  "purchaseCost": 4500,
  "depreciationPeriod": null,
  "salvageValue": null,
  "contentListId": null,
  "imageId": "e9a875a0-5c87-11e5-9666-00259031aaaa",
  "imageThumbnailId": "e9aa4a60-5c87-11e5-9666-00259031aaaa",
  "manufacturer": "Highend",
  "manufactureCountry": null,
  "notes": null,
  "prepTime": 0,
  "deprepTime": 0,
  "weight": 44.7,
  "height": 22.4,
  "modelLength": 12.6,
  "width": 15.3,
  "trackedByRunningHours": false,
  "expendable": false,
  "expendableReturnEstimate": 0,
  "partNumber": null,
  "sku": "IM-LMOD-SSC2-00",
  "stackable": false,
  "discontinued": false,
  "msrp": 0,
  "alwaysSubrented": false,
  "onWheels": false,
  "weightSupported": 0,
  "manufactured": false,
  "estimatedValue": 0,
  "currencyId": null,
  "vehicle": false,
  "displayOrder": 0,
  "batteryPowered": false,
  "masterQuantity": 0,
  "weightUnitId": "7015642c-abee-11df-b8d5-00e08175e43e",
  "linearUnitId": "917184f0-c5c2-11df-9467-00e08175e43e",
  "groupId": "a2ff8fe0-8ac7-11e4-aebc-00259031aaaa",
  "iconId": "21df2fe0-9b63-11e4-bda6-00259031aaaa",
  "iconImageId": null,
  "presetCode": "serialized-model-with-acc",
  "alternateDisplayOrder": 0,
  "scheduledMaintenanceCount": 0,
  "storageContainer": false,
  "domainId": "inventory-model",
  "serialContainer": false,
  "flagField": "1010000",
  "shortNameOrName": "Shapeshifter C2"
}
```
***Sample response from Inventory - /api/inventory-model/{modelId}key-info***<br>
*Note this includes total qty, # out, # allocated*

```
{
  "id": "ce98d110-5c87-11e5-9666-00259031aaaa",
  "name": "Shapeshifter C2",
  "size": null,
  "barcode": "00583",
  "trackedBySerialUnit": true,
  "groupFullDisplayString": "Lighting > Moving Head",
  "imageId": "e9a875a0-5c87-11e5-9666-00259031aaaa",
  "imageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/e9a875a0-5c87-11e5-9666-00259031aaaa",
  "icon": {
    "id": "21df2fe0-9b63-11e4-bda6-00259031aaaa",
    "name": "Elation Blade",
    "category": "Lighting",
    "imageId": "21de6c90-9b63-11e4-bda6-00259031aaaa",
    "domainId": "icon"
  },
  "deleted": false,
  "out": 4,
  "freeScannedOut": 0,
  "ooc": 0,
  "presumedMissing": 0,
  "inContainers": 12,
  "totalSold": 0,
  "totalDecommissioned": 0,
  "totalDeleted": 2,
  "onHand": 8,
  "allocated": 12,
  "total": 14
}
```
- Inventory Group List - may come in handy / contains all inventory group categories
- Inventory Model Storage Location

***sample response from api/inventory-model-storage-location***
```[
  {
    "id": "6f005890-7901-11e5-9b05-00259031aaaa",
    "modelId": "ce98d110-5c87-11e5-9666-00259031aaaa",
    "locationId": "2f49c62c-b139-11df-b8d5-00e08175e43e",
    "section": "",
    "aisle": "113",
    "shelf": "A",
    "bin": null,
    "domainId": "inventory-model-storage-location"
  }
]
```




