# Onsite Search Performed

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Onsite Search Performed",
    "onsiteSearch": {
        "capacity": {
            "people": {
                "numAdults": <numAdults>,
                "numChildren": <numChildren>
            }
        },
        "keyword": {
            "searchTerm": "<searchTerm>",
            "searchType": "<searchType>"
        },
        "location": {
            "map": {
                "zoomLevel": "<zoomLevel>"
            }
        }
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|onsiteSearch.capacity.people.numAdults|integer|Integer number of adults for the booking|1, 2, 3, 4, 5||||1|||
|onsiteSearch.capacity.people.numChildren|integer|Integer number of kids for the booking|1, 2, 3, 4, 5||||0|||
|onsiteSearch.keyword.searchTerm|string|Describes the search keyword used after auto-correct, auto-complete, or keyword suggestion. |bluth, blue, red lobster|||||||
|onsiteSearch.keyword.searchType|string|Describes the domain of the search. |products, properties, articles, authors, coupons, publications|||||||
|onsiteSearch.location.map.zoomLevel|string|Indicator of the zoom level in a map presentation. Values are typically integers, but can vary depending on the map service used. |1, 2, 3, 4, 5, 6|||||||




