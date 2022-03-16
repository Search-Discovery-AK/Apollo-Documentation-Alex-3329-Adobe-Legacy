# Event Listing Displayed

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Event Listing Displayed",
    "listingDisplayed": {
        "displayCount": <displayCount>,
        "filterList": "<filterList>",
        "filterListLength": <filterListLength>,
        "listing": [
            {
                "event": {
                    "eventId": "<eventId>",
                    "eventName": "<eventName>",
                    "eventType": "<eventType>",
                    "fakeProductId": "<fakeProductId>",
                    "status": "<status>"
                },
                "isDisplayed": <isDisplayed>,
                "itemPosition": <itemPosition>,
                "location": {
                    "latitude": <latitude>,
                    "locationDistanceFromPOI": <locationDistanceFromPOI>,
                    "locationId": "<locationId>",
                    "longitude": <longitude>
                },
                "price": {
                    "currency": "<currency>"
                }
            }
        ],
        "listingDriver": "<listingDriver>",
        "listingType": "<listingType>",
        "resultsCount": <resultsCount>,
        "sortDefault": <sortDefault>,
        "sortOrder": "<sortOrder>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|listingDisplayed.displayCount|integer|The total number of items displayed out of all returned items. \(Integer\)|10, 20, 30, 40||||0|||
|listingDisplayed.filterList|string|A twice delimited string of filterType and filterValue pairs.  Use \~ between type and value.  Use \| between pairs|sort\~price ascending\|color\~green\|size\~medium|||||||
|listingDisplayed.filterListLength|integer|The number of filterValue pairs in the filterList|0, 20, 12||||0|||
|listingDisplayed.listingDriver|string|Describes the action that caused the listing to be displayed|Onsite Search, Curated Assortment, Navigation|||||||
|listingDisplayed.listingType|string|The type of results being listed|text, product, location, event, room, product location|||||||
|listingDisplayed.listing[n].event.eventId|string|Unique Identifier of an event. |155, 65588, 987764448|||||||
|listingDisplayed.listing[n].event.eventName|string|The friendly name of the event.|Max your 401K, Structured JavaScript, Mid Day Yoga, Frosty 5K Fun Run, Whiskey Wednesday|||||||
|listingDisplayed.listing[n].event.eventType|string|The type of the event|Webinar, Class, Conference, Race, Meet Up|||||||
|listingDisplayed.listing[n].event.fakeProductId|string|Helper node used by AA Product String Builder to set product to location. This field gets a static value of "event".  With updates to the AA PS extension, this will soon go away.|event|event||||||
|listingDisplayed.listing[n].event.status|string|The status of an event.|Cancelled, Sold Out, Postponed, Rescheduled|||||||
|listingDisplayed.listing[n].isDisplayed|boolean|Helper node used by AA Product String Builder to set product scoped events|true|||||||
|listingDisplayed.listing[n].itemPosition|integer|Integer position of a property within a sorted result. The first returned is position 1. For map results, this value can be the rank by distance from POI.|1, 2, 3, 4, 5||||0|||
|listingDisplayed.listing[n].location.latitude|number|The latitude of the map center for a location search.|48.858093||||-90|90||
|listingDisplayed.listing[n].location.locationDistanceFromPOI|integer|The distance from the location to the user's point of interest|12, 3, 5, 200|||||||
|listingDisplayed.listing[n].location.locationId|string|Unique Identifier of a Location. |155, 65588, 987764448|||||||
|listingDisplayed.listing[n].location.longitude|number|The longitude of the map center for a location search.|2.294694||||-180|180||
|listingDisplayed.listing[n].price.currency|string|Currency of the prices given. ISO 4217 \(3 character alpha\), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|listingDisplayed.resultsCount|integer|The total number of items returned that matched the search criteria. \(Integer\)|1, 21, 111, 166||||0|||
|listingDisplayed.sortDefault|integer|The default sort value on listings|A to Z, Low to High, Newest to Oldest||||0|||
|listingDisplayed.sortOrder|string|Indicates the sort order.|high-low, low-high, nearest-farthest, a-z, newest-oldest|||||||




