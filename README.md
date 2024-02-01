# Enkadia - Pinpoint (for Inspirmedia)
Respository for the planning and development of the Pinpoint equipment availability and warehouse locator app. This repository contains notes and some sample code for the Flex API.

### This is a document and project management repository only

#### Flex API Notes

#### Contents
[General Notes](https://github.com/normschaeffer/Flex-API-Docs/blob/main/README.md#general-notes)  
[Business Location](business location link here)  
[Equipment List](https://github.com/normschaeffer/Flex-API-Docs/edit/main/README.md#equipment-list)  
  + [Equipment List Line Item Nodes by Ids](https://github.com/normschaeffer/Flex-API-Docs/blob/main/README.md#equipment-list-line-item-nodes-by-ids)
  + [Equipment List find items in a parent node](https://github.com/normschaeffer/Flex-API-Docs/blob/main/README.md#equipment-list-find-items-in-a-parent-node)



#### General Notes<a name="general-notes"></a>

* Flex uses Swagger API for documentation and methods testing.
* In the Flex API Swagger documentation, you will frequently find names such as locationId, notesId, modelId. In most cases these are *not* field names found in the record, but rather are the record's unique Id.
* Because Flex uses a SQL type database, desired information will typically require joins of multiple tables. 



#### Useful Methods
- Business location - get locationID for Inspirmedia - Main (used for some lookups) *this should be declared a constant in appdev for IM, since there is only one location*
  
#### Equipment List<a name="equipment-list"></a>
   contains methods to get list from pull sheet?? *need to use global search to find Pull Sheet unique id*

 ***Sample response from Equipment List api/equipment-list/{id}***
 
```
{
  "id": "838a13a0-8492-11ee-9ae0-e2999141f70a",
  "name": "Kimmy Lea Event",
  "createdByUserId": "6a83b8b3-f653-49d1-ae60-199dc283cb75",
  "createdDate": "2023-11-16T15:12:10",
  "lastEditUserId": "6a83b8b3-f653-49d1-ae60-199dc283cb75",
  "lastEditDate": "2023-11-16T15:14:43",
  "documentNumber": "PPKLC",
  "parentElementId": "3b9298f3-a7bb-4856-826d-37be80af0337",
  "definitionId": "a220432c-af33-11df-b8d5-00e08175e43e",
  "plannedStartDate": "2023-11-29T18:00:00",
  "plannedEndDate": "2023-12-01T04:00:00",
  "calcStartDate": "2023-11-29T18:00:00",
  "calcEndDate": "2023-12-01T04:00:00",
  "departmentId": null,
  "locationId": "2f49c62c-b139-11df-b8d5-00e08175e43e",
  "secondaryLocationId": null,
  "pickupLocationId": null,
  "returnLocationId": null,
  "personResponsibleId": "05e9efe0-8723-11e4-b7ee-00259031aaaa",
  "clientId": "03d34a10-b6d8-11e8-9dc3-00259031aaaa",
  "secondaryClientId": null,
  "vendorId": null,
  "billToId": null,
  "secondaryBillToId": null,
  "venueId": "4271c8e0-da9e-11e6-baf6-00259031aaaa",
  "secondaryVenueId": null,
  "artistId": null,
  "returnMethodId": null,
  "shippingMethodId": null,
  "statusId": "f44019cc-aee1-11df-b8d5-00e08175e43e",
  "currentWorkflowStateId": "a8d6ee0c-af31-11df-b8d5-00e08175e43e",
  "deleted": false,
  "locked": false,
  "open": true,
  "documentNumberSequence": 0,
  "ordinal": 0,
  "actualCost": 0,
  "actualRevenue": 0,
  "budgetedCost": 0,
  "budgetedRevenue": 1125,
  "resolvedActualCost": 0,
  "resolvedActualRevenue": 0,
  "resolvedBudgetedCost": 0,
  "resolvedBudgetedRevenue": 0,
  "depositDueDate": "2022-12-01T14:00:00",
  "dueDate": null,
  "loadInDate": "2023-11-29T20:00:00",
  "loadOutDate": "2023-11-30T23:00:00",
  "preparedDate": null,
  "showStartDate": "2023-11-30T19:00:00",
  "eventDate": null,
  "showEndDate": null,
  "rehearsalDate": null,
  "doorsDate": null,
  "customerPO": null,
  "clientInsurance": 0,
  "currencyId": "911e3d4c-aedc-11df-b8d5-00e08175e43e",
  "accountExecutiveId": null,
  "administrativeAssistantId": null,
  "backstageManagerId": null,
  "eventPlannerId": null,
  "projectManagerId": null,
  "salesPersonId": null,
  "stageDirectorId": null,
  "technicalDirectorId": null,
  "customContactOneId": null,
  "customContactTwoId": null,
  "customContactThreeId": null,
  "customField1Value": null,
  "customField2Value": null,
  "customField3Value": null,
  "customField4Value": null,
  "customField5Value": null,
  "customField6Value": null,
  "customField7Value": null,
  "customField8Value": null,
  "customField9Value": null,
  "customField10Value": null,
  "corporateIdentityId": null,
  "deposit": 0,
  "depositPercentage": 0,
  "insurableValue": 24099.5,
  "facilityId": null,
  "referralSourceId": null,
  "colorCode": "8de2ea",
  "textColor": "0",
  "elementTypeId": null,
  "assignedToUserId": "e86be360-8722-11e4-b7ee-00259031aaaa",
  "notes": null,
  "printNotes": true,
  "defaultTime": 1,
  "defaultPricingModelId": "af4a35ac-aedf-11df-b8d5-00e08175e43e",
  "probabilityPercent": null,
  "privateElement": false,
  "prepCompleted": false,
  "deprepCompleted": false,
  "returnCompleted": false,
  "shipCompleted": false,
  "receiveCompleted": false,
  "subrentalReturnCompleted": false,
  "prepCompletedUserId": null,
  "deprepCompletedUserId": null,
  "returnCompletedUserId": null,
  "shipCompletedUserId": null,
  "receiveCompletedUserId": null,
  "subrentalReturnCompletedUserId": null,
  "prepCompletedTimestamp": null,
  "deprepCompletedTimestamp": null,
  "returnCompletedTimestamp": null,
  "shipCompletedTimestamp": null,
  "receiveCompletedTimestamp": null,
  "subrentalReturnCompletedTimestamp": null,
  "prepManifestId": null,
  "deprepManifestId": null,
  "shipManifestId": null,
  "returnManifestId": null,
  "receiveManifestId": null,
  "subrentalReturnManifestId": null,
  "weight": 34.80000002682209,
  "totalPrepTime": 0,
  "totalDeprepTime": 0,
  "totalPrepTimeAsTimeString": "00:00",
  "totalDeprepTimeAsTimeString": "00:00",
  "leftAddressString": "LimeLight Expressions\nKimmy Lea\nP.O. Box 45414\nOmaha, NE  68145\nPhone: 402.915.3534\nEmail: Kimmylea@limelightexpressions.com",
  "rightAddressString": "Omaha Design Center\n1502 Cuming St\nOmaha, NE  68102\nPhone: (402) 819-8792",
  "domainId": "equipment-list",
  "displayName": "Kimmy Lea Event (PPKLC)"
}
```
#### Equipment List Line Item Nodes by Ids<a name="equipment-list-line-item-nodes-by-id"></a> 
This method shows the ids of the parent groups and ungrouped items on a pull sheet.

***sample response from Equipment List api/eqlist-line-item/nodes-by-ids***
```
[
  {
    "id": "325d24ef-814a-44e0-aee4-da065d3e9b51",
    "displayName": "Electrical\n",
    "parentLineItemId": null,
    "resourceId": null,
    "resourceBarcode": null,
    "resourceClassName": null,
    "resourceImageUrl": null,
    "group": true,
    "leaf": false,
    "virtual": false,
    "lineQtyInfo": {
      "preppedQty": 0,
      "dePreppedQty": 0,
      "shippedQty": 0,
      "returnedQty": 0,
      "requiredQty": 0,
      "prepped": true,
      "deprepped": true,
      "returned": true,
      "shipped": true,
      "overPrepped": false,
      "overDeprepped": false,
      "overShipped": false,
      "overReturned": false
    },
    "groupQtyInfo": {
      "preppedQty": 0,
      "dePreppedQty": 0,
      "shippedQty": 0,
      "returnedQty": 0,
      "requiredQty": 4,
      "prepped": false,
      "deprepped": false,
      "returned": false,
      "shipped": false,
      "overPrepped": false,
      "overDeprepped": false,
      "overShipped": false,
      "overReturned": false
    }
  },
  {
    "id": "83dd63c0-8492-11ee-9ae0-e2999141f70a",
    "displayName": "FOH Power Strip",
    "parentLineItemId": null,
    "resourceId": "10cffa94-8dba-4695-942c-54bfba3a5da8",
    "resourceBarcode": "03983",
    "resourceClassName": "com.shoptick.inventory.domain.InventoryItem",
    "resourceImageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/d7e89502-03fb-4690-98cf-5642bf77f371",
    "group": false,
    "leaf": true,
    "virtual": false,
    "lineQtyInfo": {
      "preppedQty": 0,
      "dePreppedQty": 0,
      "shippedQty": 0,
      "returnedQty": 0,
      "requiredQty": 1,
      "prepped": false,
      "deprepped": false,
      "returned": false,
      "shipped": false,
      "overPrepped": false,
      "overDeprepped": false,
      "overShipped": false,
      "overReturned": false
    },
    "groupQtyInfo": null
  },
  {
    "id": "83a71180-8492-11ee-9ae0-e2999141f70a",
    "displayName": "Video",
    "parentLineItemId": null,
    "resourceId": null,
    "resourceBarcode": null,
    "resourceClassName": null,
    "resourceImageUrl": null,
    "group": true,
    "leaf": false,
    "virtual": false,
    "lineQtyInfo": {
      "preppedQty": 0,
      "dePreppedQty": 0,
      "shippedQty": 0,
      "returnedQty": 0,
      "requiredQty": 0,
      "prepped": true,
      "deprepped": true,
      "returned": true,
      "shipped": true,
      "overPrepped": false,
      "overDeprepped": false,
      "overShipped": false,
      "overReturned": false
    },
    "groupQtyInfo": {
      "preppedQty": 0,
      "dePreppedQty": 0,
      "shippedQty": 0,
      "returnedQty": 0,
      "requiredQty": 24,
      "prepped": false,
      "deprepped": false,
      "returned": false,
      "shipped": false,
      "overPrepped": false,
      "overDeprepped": false,
      "overShipped": false,
      "overReturned": false
    }
  }
]
```
#### Equipment List find items in a parent node<a name="equipment-list-find-items-in-a-parent-node"></a>  
   This method finds all items in a parent group or ungrouped item. Requires the use of the equipmentListId (from equipment-list/{id}) and the parentLineItemId (from api/eqlist-line-item/nodes-by-ids)

***sample response from api/eqlist-line-item/node-list/{parentLineItemId}*** <br>
http request <br>
*note in the request the parentLineItemId is follows the method without any identifier (i.e. there is not ...node-list/parentLineItemId=83a711...)*
```
https://inspirmedia.flexrentalsolutions.com/f5/api/eqlist-line-item/node-list/83a71180-8492-11ee-9ae0-e2999141f70a?equipmentListId=838a13a0-8492-11ee-9ae0-e2999141f70a&page=0&size=20
```
response
```
{
  "content": [
    {
      "id": "5396c40e-0d47-47e4-8462-f92c962447bd",
      "displayName": "HD SDI Cable - 5'",
      "parentLineItemId": "83a71180-8492-11ee-9ae0-e2999141f70a",
      "resourceId": "a02ae6e0-8ad9-11e4-bda6-00259031aaaa",
      "resourceBarcode": "00150",
      "resourceClassName": "com.shoptick.inventory.domain.InventoryItem",
      "resourceImageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/b69a45c2-28b0-4586-a623-7fee40c73897",
      "group": false,
      "leaf": true,
      "virtual": false,
      "lineQtyInfo": {
        "preppedQty": 0,
        "dePreppedQty": 0,
        "shippedQty": 0,
        "returnedQty": 0,
        "requiredQty": 6,
        "prepped": false,
        "deprepped": false,
        "returned": false,
        "shipped": false,
        "overPrepped": false,
        "overDeprepped": false,
        "overShipped": false,
        "overReturned": false
      },
      "groupQtyInfo": null
    },
    {
      "id": "1ea7d9a2-6c80-423d-b25d-f31d16091ac5",
      "displayName": "HD SDI Cable - 10'",
      "parentLineItemId": "83a71180-8492-11ee-9ae0-e2999141f70a",
      "resourceId": "a00d4cc0-8ad9-11e4-bda6-00259031aaaa",
      "resourceBarcode": "00144",
      "resourceClassName": "com.shoptick.inventory.domain.InventoryItem",
      "resourceImageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/6a590630-4c85-11e7-af45-00259031aaaa",
      "group": false,
      "leaf": true,
      "virtual": false,
      "lineQtyInfo": {
        "preppedQty": 0,
        "dePreppedQty": 0,
        "shippedQty": 0,
        "returnedQty": 0,
        "requiredQty": 4,
        "prepped": false,
        "deprepped": false,
        "returned": false,
        "shipped": false,
        "overPrepped": false,
        "overDeprepped": false,
        "overShipped": false,
        "overReturned": false
      },
      "groupQtyInfo": null
    },
    {
      "id": "bc567bd9-9a41-4630-b99e-b0f5867440c1",
      "displayName": "HD SDI Cable - 50'",
      "parentLineItemId": "83a71180-8492-11ee-9ae0-e2999141f70a",
      "resourceId": "a02f53b0-8ad9-11e4-bda6-00259031aaaa",
      "resourceBarcode": "00151",
      "resourceClassName": "com.shoptick.inventory.domain.InventoryItem",
      "resourceImageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/912bafae-554f-43ba-a09e-31e8ae233935",
      "group": false,
      "leaf": true,
      "virtual": false,
      "lineQtyInfo": {
        "preppedQty": 0,
        "dePreppedQty": 0,
        "shippedQty": 0,
        "returnedQty": 0,
        "requiredQty": 2,
        "prepped": false,
        "deprepped": false,
        "returned": false,
        "shipped": false,
        "overPrepped": false,
        "overDeprepped": false,
        "overShipped": false,
        "overReturned": false
      },
      "groupQtyInfo": null
    },
    {
      "id": "83b394a0-8492-11ee-9ae0-e2999141f70a",
      "displayName": "Panasonic AW-UE150 PTZ 4k Camera",
      "parentLineItemId": "83a71180-8492-11ee-9ae0-e2999141f70a",
      "resourceId": "bb25eadf-679c-4c68-8bd1-2eafdd917dde",
      "resourceBarcode": "03118",
      "resourceClassName": "com.shoptick.inventory.domain.InventoryItem",
      "resourceImageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/5ff9694f-0418-404b-9510-09a9139bceb5",
      "group": false,
      "leaf": true,
      "virtual": false,
      "lineQtyInfo": {
        "preppedQty": 0,
        "dePreppedQty": 0,
        "shippedQty": 0,
        "returnedQty": 0,
        "requiredQty": 1,
        "prepped": false,
        "deprepped": false,
        "returned": false,
        "shipped": false,
        "overPrepped": false,
        "overDeprepped": false,
        "overShipped": false,
        "overReturned": false
      },
      "groupQtyInfo": null
    },
    {
      "id": "83b9af20-8492-11ee-9ae0-e2999141f70a",
      "displayName": "Robo Combo Cable 150'",
      "parentLineItemId": "83a71180-8492-11ee-9ae0-e2999141f70a",
      "resourceId": "f260eb48-ba7e-4c34-add1-3a643f56d7ad",
      "resourceBarcode": "04135",
      "resourceClassName": "com.shoptick.inventory.domain.InventoryItem",
      "resourceImageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/36756aec-c600-4ed6-9fbc-e46a1036e64c",
      "group": false,
      "leaf": true,
      "virtual": false,
      "lineQtyInfo": {
        "preppedQty": 0,
        "dePreppedQty": 0,
        "shippedQty": 0,
        "returnedQty": 0,
        "requiredQty": 1,
        "prepped": false,
        "deprepped": false,
        "returned": false,
        "shipped": false,
        "overPrepped": false,
        "overDeprepped": false,
        "overShipped": false,
        "overReturned": false
      },
      "groupQtyInfo": null
    },
    {
      "id": "83beb830-8492-11ee-9ae0-e2999141f70a",
      "displayName": "Panasonic AW-RP150 PTZ Controller",
      "parentLineItemId": "83a71180-8492-11ee-9ae0-e2999141f70a",
      "resourceId": "c575b4b9-f33a-4410-b1fe-aa80423c110e",
      "resourceBarcode": "03117",
      "resourceClassName": "com.shoptick.inventory.domain.InventoryItem",
      "resourceImageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/d8ca3c85-8fc8-4845-b311-bc934c5074ca",
      "group": false,
      "leaf": true,
      "virtual": false,
      "lineQtyInfo": {
        "preppedQty": 0,
        "dePreppedQty": 0,
        "shippedQty": 0,
        "returnedQty": 0,
        "requiredQty": 1,
        "prepped": false,
        "deprepped": false,
        "returned": false,
        "shipped": false,
        "overPrepped": false,
        "overDeprepped": false,
        "overShipped": false,
        "overReturned": false
      },
      "groupQtyInfo": null
    },
    {
      "id": "83c4d2b0-8492-11ee-9ae0-e2999141f70a",
      "displayName": "536 CF Tripod 509HD",
      "parentLineItemId": "83a71180-8492-11ee-9ae0-e2999141f70a",
      "resourceId": "1e5829e9-8f6c-49bc-8f07-4ad529083fba",
      "resourceBarcode": "04197",
      "resourceClassName": "com.shoptick.inventory.domain.InventoryItem",
      "resourceImageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/52d43c30-3f41-4577-93e4-34b7e1921721",
      "group": false,
      "leaf": true,
      "virtual": false,
      "lineQtyInfo": {
        "preppedQty": 0,
        "dePreppedQty": 0,
        "shippedQty": 0,
        "returnedQty": 0,
        "requiredQty": 1,
        "prepped": false,
        "deprepped": false,
        "returned": false,
        "shipped": false,
        "overPrepped": false,
        "overDeprepped": false,
        "overShipped": false,
        "overReturned": false
      },
      "groupQtyInfo": null
    },
    {
      "id": "d6027fe4-a3d1-4094-91cc-8599d92120be",
      "displayName": "Lumantek SDI to HDMI ",
      "parentLineItemId": "83a71180-8492-11ee-9ae0-e2999141f70a",
      "resourceId": "cb81ebc0-3260-11ea-a66f-f23c91d0e296",
      "resourceBarcode": "02633",
      "resourceClassName": "com.shoptick.inventory.domain.InventoryItem",
      "resourceImageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/308e865a-59b8-45bc-b24d-dac71431a36a",
      "group": false,
      "leaf": false,
      "virtual": false,
      "lineQtyInfo": {
        "preppedQty": 0,
        "dePreppedQty": 0,
        "shippedQty": 0,
        "returnedQty": 0,
        "requiredQty": 2,
        "prepped": false,
        "deprepped": false,
        "returned": false,
        "shipped": false,
        "overPrepped": false,
        "overDeprepped": false,
        "overShipped": false,
        "overReturned": false
      },
      "groupQtyInfo": {
        "preppedQty": 0,
        "dePreppedQty": 0,
        "shippedQty": 0,
        "returnedQty": 0,
        "requiredQty": 2,
        "prepped": false,
        "deprepped": false,
        "returned": false,
        "shipped": false,
        "overPrepped": false,
        "overDeprepped": false,
        "overShipped": false,
        "overReturned": false
      }
    },
    {
      "id": "83cb3b50-8492-11ee-9ae0-e2999141f70a",
      "displayName": "Hyperdeck Studio Mini",
      "parentLineItemId": "83a71180-8492-11ee-9ae0-e2999141f70a",
      "resourceId": "a2a11596-85bd-4bcd-990e-ade17828e337",
      "resourceBarcode": "02629",
      "resourceClassName": "com.shoptick.inventory.domain.InventoryItem",
      "resourceImageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/3400e15d-fc2e-4636-852e-0788f28c4098",
      "group": false,
      "leaf": false,
      "virtual": false,
      "lineQtyInfo": {
        "preppedQty": 0,
        "dePreppedQty": 0,
        "shippedQty": 0,
        "returnedQty": 0,
        "requiredQty": 1,
        "prepped": false,
        "deprepped": false,
        "returned": false,
        "shipped": false,
        "overPrepped": false,
        "overDeprepped": false,
        "overShipped": false,
        "overReturned": false
      },
      "groupQtyInfo": {
        "preppedQty": 0,
        "dePreppedQty": 0,
        "shippedQty": 0,
        "returnedQty": 0,
        "requiredQty": 2,
        "prepped": false,
        "deprepped": false,
        "returned": false,
        "shipped": false,
        "overPrepped": false,
        "overDeprepped": false,
        "overShipped": false,
        "overReturned": false
      }
    },
    {
      "id": "83d72230-8492-11ee-9ae0-e2999141f70a",
      "displayName": "Roland VR-50 MK II",
      "parentLineItemId": "83a71180-8492-11ee-9ae0-e2999141f70a",
      "resourceId": "ac089f90-062e-11ea-a09f-f23c91d0e296",
      "resourceBarcode": "02521",
      "resourceClassName": "com.shoptick.inventory.domain.InventoryItem",
      "resourceImageUrl": "https://inspirmedia.flexrentalsolutions.com/f5/api/image/file/2abdaea0-109f-11ea-a66f-f23c91d0e296",
      "group": false,
      "leaf": true,
      "virtual": false,
      "lineQtyInfo": {
        "preppedQty": 0,
        "dePreppedQty": 0,
        "shippedQty": 0,
        "returnedQty": 0,
        "requiredQty": 1,
        "prepped": false,
        "deprepped": false,
        "returned": false,
        "shipped": false,
        "overPrepped": false,
        "overDeprepped": false,
        "overShipped": false,
        "overReturned": false
      },
      "groupQtyInfo": null
    }
  ],
  "pageable": {
    "sort": {
      "unsorted": true,
      "sorted": false,
      "empty": true
    },
    "pageNumber": 0,
    "pageSize": 20,
    "offset": 0,
    "paged": true,
    "unpaged": false
  },
  "last": true,
  "totalPages": 1,
  "totalElements": 10,
  "sort": {
    "unsorted": true,
    "sorted": false,
    "empty": true
  },
  "first": true,
  "numberOfElements": 10,
  "size": 20,
  "number": 0,
  "empty": false
}
```


- Global search - can search by text, barcode, various categories (e.g. inventory-model, contact, serial, all ...)
- Inventory - includes a global get using modelId

***Sample response from Inventory - /api/inventory-model/{modelId}***
```{
  "id": "ce98d110-5c87-11e5-9666-00259031aaaa",
  "name": "Shapeshifter C2",
  "createdByUserId": "3fd5a940-5024-11e5-992f-00259031aaaa",
  "createdDate": "2015-09-16T15:30:06",
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






