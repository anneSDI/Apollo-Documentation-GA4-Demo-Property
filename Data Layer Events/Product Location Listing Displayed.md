# Product Location Listing Displayed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "Product Location Listing Displayed",
    "ecommerce": {
        "item_list_id": "<item_list_id>",
        "item_list_name": "<item_list_name>",
        "items": [
            {
                "item_id": "<item_id>",
                "item_name": "<item_name>"
            }
        ],
        "listing_type": "<listing_type>",
        "product_location_listing_item_impressions": "<product_location_listing_item_impressions>",
        "product_location_listing_result_count": <product_location_listing_result_count>,
        "product_sku": "<product_sku>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\) |SKU\_12345|||||||
|item_list_id|string|The computer-readible machine name of the list the item showed up in \(if sent with a view\_item\_list event\). Use UUID provided by the component if no more specific ID is available.|12345abcde12345|||||||
|item_list_name|string|The human-readible name of the item list the item showed up in \(if sent with a view\_item\_list event\). If one is not available, populate with numerical index of which list this is on the page \(1-indexed\). For filter\_by\_group component, use that value.|filter\_by\_group, recommended\_products, recently\_viewed\_products|||||||
|item_name|string|Item Name \(context-specific\).|jeggings|||||||
|listing_type|string|Captures the methods that bring users to listings \(i.e. Onsite Search, Top Nav, External Link, Category Landing Page\). Does not update if listings are sorted, filtered, or paginated.|Product, Location, Event, Room, Content|||||||
|product_location_listing_item_impressions|unknown|Count of product locations displayed in product location \(i.e. store\) listings.|high-low, low-high, nearest-farthest, a-z, newest-oldest|||||||
|product_location_listing_result_count|integer|Captures the total number of product locations returned in a product location listing.|1, 21, 111, 166||||0|||
|product_sku|string|Captures the ID associated with CTA links used.|34567890, 4567890, 00155-large-cornflower|||||||




