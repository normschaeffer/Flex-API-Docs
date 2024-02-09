### Equipment List Line Item Nodes by Ids<a name="equipment-list-line-item-nodes-by-id"></a> 
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
    "resourceImageUrl": "https://yourcompany.flexrentalsolutions.com/f5/api/image/file/d7e89502-03fb-4690-98cf-5642bf77f371",
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