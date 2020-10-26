# Postman Collections

This repository holds a series of postman collections demonstrating a variety of use cases for all of the [HERE REST and Platform Extension APIs](https://developer.here.com/documentation) and are updated in sync with changes to the respective APIs.
More information about our APIs can be found on [developer.here.com](https://developer.here.com/).

These examples have been created for use with the **Postman** utility. Postman is a testing framework for REST APIs. The tool can be downloaded from [www.getpostman.com](https://www.getpostman.com).

To import the collection, first `clone` this repository, then open the Postman utility and select the *`Import`* option. Select the *`Folder`* tab from the dialog and drag and drop the cloned repository folder into the target.

The collections contained in this repository are organized under this scheme:

* [REST APIs](#rest-apis)
  * [Batch Geocoder API](#batch-geocoder-api)
  * [Geocoder API](#geocoder-api)
  * [Map Image API](#map-image-api)
  * [Map Tile API](#map-tile-api)
  * [Places API](#places-api)
  * [Public Transit API](#public-transit-api)
  * [Routing API](#routing-api)
  * [Traffic API](#traffic-api)
  * [Venue Maps](#venue-maps)
  * [Weather API](#weather-api)
* [Platform Extensions](#platform-extensions)
  * [Custom Location Extension API](#custom-location-extension-api)
  * [Platform Data Extension API](#platform-data-extension-api)
  * [Route Match Extension API](#route-match-extension-api)
  * [Waypoint Sequence Extension API](#waypoint-sequence-extension-api)

> **NOTE:** In order to get the postman requests to work, you **must** replace all instances of the `{YOUR_APP_ID}` and `{YOUR_APP_CODE}` variables within the collection and use your own HERE credentials. Within Postman, set the variables using the *`Manage environments`* menu.

> You can obtain a set of credentials from the [Plans Page](https://developer.here.com/plans/api/consumer-mapping) on **developer.here.com**.

See the [LICENSE](LICENSE) file in the root of this project for license details.

# REST APIs

The **HERE REST APIs** provide a flexible and fast access to a variety of map data and other map data functions. Developers can use the HERE Rest APIs to perform tasks ranging from batch geocode requests and advanced traffic incident reports to creating an isoline route.

> Documentation on these APIs can be found on the [developer.here.com portal](https://developer.here.com/rest-apis).

## [Batch Geocoder API](batch-geocoder.postman_collection)

* **Batch Geocode Addresses** -  Start asynchronously geocoding a large set of addresses in one batch
* **Batch Geocode Job Status** - Request the status of a batch geocoder job
* **Batch Reverse Geocode Locations** - Start asynchronously reverse-geocoding a large set of locations in one batch
* **Download Geocoded Data**  - Download a zipped geocoded dataset from a completed job

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/6337161a8efcffb6f72a)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/batch-geocoder.postman_collection)

## [Geocoder API](geocoder.postman_collection)

* **Geocode a Street Intersection** - Request the latitude, longitude and details of a street intersection
* **Geocode an Address within a Bounding Box** - Request the latitude, longitude and details of an address restricting results to a specific area
* **Geocode using free-form input** - Request the latitude, longitude and details of an address based on free-form text input
* **Geocode using partial address information** - Request the latitude, longitude and details of an address based on partial address information
* **Multi-reverse Geocode Addresses** - Request the addresses of up to one hundred locations with one multi-reverse geocoding request
* **Multi-reverse Geocode Landmarks** - Request the nearest landmarks for up to one hundred locations with one multi-reverse geocoding request
* **Reverse Geocode Landmarks** - Request details of landmarks near to a given latitude and longitude
* **Reverse Geocode an Address from a Location** - Request address details for a given latitude and longitude
* **Reverse Geocode the District containing a Location** - Request details about the district containing a given latitude and longitude
* **Reverse Geocode the Shape of a Postal Code** - Request the shape of a postal district for a given latitude and longitude
* **Suppressing Response Attributes** - Request only the latitude, longitude for a given address

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/4f968ce760f14ed986dc)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/geocoder.postman_collection)

## [Map Image API](map-image.postman_collection)

* **Changing from the Metric System** - Request an image of a map including a scale bar in miles or yards
* **Default Map Image** - Request the default image of a map
* **Language Support** - Request an image of a map including labels in a foreign language
* **Map Image at a specified location** - Request an image of a map at a specified location and zoom level
* **Map Image using Bounding Box** - Request an image of a map based around a given area
* **Map Image with Address** - Request an image of a map displaying an address
* **Map Image with Height and Width** - Request an image of a map with a defined height and width
* **Map Image with Polylines** - Request an image of a map including a polyline
* **Map Image with Scale Bar** - Request an image of a map including a scale bar
* **Map Image with Standard Markers** - Request an image of a map highlighting points of interest
* **Map Image with Text Markers**- Request an image of a map including additional texts
* **Map Image with a Proximity Circle** - Request the image of a map showing uncertainty of position
* **Picture in Picture** - Request an image of a map including an embedded overview map
* **Styling Markers Individually** - Request an image of a map including markers each with a custom style
* **Styling a Set of Markers** - Request an image of a map including markers styled with a common theme
* **Terrain Map Image** - Request an image of a topographical map

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/639497e869981f6ca24d)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/map-image.postman_collection)

## [Map Tile API](map-tile.postman_collection)

* **Base64 Encoded Map Tile** - Request a base64 encoded map tile
* **Color-reduced Street Map** - Request a greyed out street map tile
* **Color-reduced Transit Map** - Request a color-reduced map tile with public transport
* **Copyright Information** - Request map tile copyright information
* **Display Points of Interest** - Request a map tile including points of interest
* **Filtering Points of Interest** - Request a map tile including selected points of interest
* **Fleet Vehicle Map** - Request a street map tile using the fleet vehicle color scheme
* **Foreign Language Support** - Request a map tile with labels in a foreign language
* **Hi-Res Map Tiles** - Request a high-resolution street map tile
* **Hybrid Map** - Request a hybrid map tile - satellite imagery with labels
* **Map Tile Meta Data** - Request meta data about points of interest on a map tile
* **Map Tile Type Information** - Request information about the types of map tiles available on a server
* **Mobile Optimization** - Request a street map tile optimized for mobile devices
* **Multiple Base64 Encoded Map Tiles** - Request multiple base64 encoded map tiles
* **Normal Street Map** - Request a street map tile
* **Point of Interest Categories** - Request point of interest category information
* **Satellite Map** - Request a satellite map tile
* **Support for Multiple Languages** - Request a map tile with labels in two languages
* **Terrain Map** - Request a terrain map tile
* **Toll Zone Map** - Request a street map tile highlighting congestion and environmental toll zones
* **Transparent Truck Restrictions Map** - Request a transparent tile showing restrictions for heavy vehicles only
* **Truck Restrictions Map** - Request a street map tile showing restrictions for heavy vehicles

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/69119d09338b80b1feb7)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/map-tile.postman_collection)

## [Places API](places.postman_collection)

* **Explore Nearby Places** places/explore-nearby-places) - Request a list of places close to a location
* **Explore Places using Implicit Contexts** places/explore-places-implicit-contexts) - Request a list of popular places within a specified area
* **Explore Places within a Bounding Box** places/explore-places-bounding-box) - Request a list of popular places within a specified area
* **Explore Popular Places** places/explore-popular-places) - Request a list of popular places around a location
* **Explore Popular Places by Category** places/explore-popular-places-category) - Request a list of places within a category around a location
* **Multi-language support** places/explore-places-multi-language-support) - Request a list of popular places around a location using a foreign language
* **One-Box Search** places/places-search-by-query) - Request a list of nearby places based on a query string
* **Place Categories** places/place-categories) - Request a list of place categories available for a given location
* **Search Suggestions** places/search-suggestion) - Request a list of suggestions based on a partial query string

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/5512cdb6376b4f216541)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/places.postman_collection)

## [Public Transit API](public-transit.postman_collection)

* **Adjust Walking Speed in Transit Route** - Request a public transit route with faster walking speed
* **Avoid Transit Routes Involving Transfers** - Request a direct public transit route excluding changes and transfers
* **Avoiding a Form of Public Transit** - Request a public transit route for trams and metros only
* **Find Stations Nearby** - Request a list of public transit stations within a given geo-location.
* **Find Stations by ID** - Request details of a specific transit station based on a previous request
* **Find Stations by Name** - Request a list of public transit stations based on name
* **Find Transit Coverage in Cities Nearby** - Request a list of transit operators available in cities nearby
* **Multi-Station Board Departure Times** - Request a list of all next departure times and destinations
* **Next Nearby Departures from a given station** - Request a list of next departure times and destinations of a particular station
* **Plan a Transit Route to Arrive at a Certain Time** - Request a public transit route between any two place.
* **Plan a route from A to B using Public Transport** - Request a public transit route between any two place.
* **Public Transit Route That Shows Line Graph** - Request a public transit route with line graphs showing the actual route of the transit services.
* **Reachability of an Area Within a Specific Time** - Request a list of the public transit stations that can be reached in a given time
* **Reachability of an Area with Only Buses** - Request a list of the public transit stations that can be reached with certain transit types only
* **Show Intermediate Stations on a Transit Route** - Request a public transit route showing intermediate stops between stations
* **Show Up to 6 Transit Routes** - Request the maxium no of public transit routes for a journey
* **Transit Coverage Nearby** - Request a list of transit operators and station coverage nearby
* **Transit Coverage Within a City** - Request a list of transit operator coverage within a specified city

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/db160e2119445bca4955)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/public-transit.postman_collection)

## [Routing API](routing.postman_collection)

* **Abnormal Loads** - Request a truck route for long, tall or wide vehicles
* **Additional Route Settings** - Request a route specifying additional route settings.
* **Alternative routes** - Request multiple alternative routes within a single request
* **Avoiding a Form of Public Transport** - Request a public transport route avoiding rail
* **Avoiding a specified area** - Request a route avoiding a defined area by specifying a bounding box
* **Avoiding a specified stretch of road** - Request a route avoiding a specific road as defined by an avoidLink
* **Car Route from A to B** - Request a driving route between two points
* **Changing from the metric system** - Request a route with instructional distances given in miles and yards
* **Distance-based isoline with destination as center** - Request an isoline that will reach a destination within a defined distance of travel
* **Distance-based isoline with start as center** - Request the shape outlining the area that can be reached within a defined distance of travel
* **Getting route information within viewbounds** - Request partial route information for maneuvers within a given area
* **Hazardous Goods** - Request a truck route for a vehicle transporting hazardous goods
* **Link Information for a location** - Request detailed information about a path segment in the routing network given one of its coordinates
* **Link Information using linkId** - Request detailed information about a path segment in the routing network given a linkid
* **Many to Many Matrix Routing** - Matrix routing request with three start points and five destinations
* **Multi-language support** - Request route instructions in a foreign language
* **One to Many Matrix Routing** - Simultaneously calculate route distances to multiple locations
* **Pedestrian Route from A to B** - Request a walking route between two points
* **Prefer/Avoid Motorways** - Request a route preferring or avoiding specific types of road
* **Previously Calculated Route Information** - Request information about a previously calculated route
* **Route from A to B using Public Transport** - Request a route between two points using public transport
* **Route with an Intermediate Stop Point** - Request a route from A to B with stop at an intermediate point C
* **Time-based isoline with destination as center** - Request an isoline that will reach a destination within a given time
* **Time-based isoline with start point as center** - Request the shape outlining the area that can be reached within a given time
* **Timetabled Public Transport Route** - Request a public transport route between two points specifying a departure time
* **Toll Summary by Country** - Request a truck route with toll road summary by country
* **Truck Route from A to B** - Request a truck route between two points
* **Truck Route from A to B with shape information** - Request a truck route between two points including additional information
* **Truck Route via an Intermediate Point** - Request a truck route from A to C with an additional stopover at point B
* **Truck route trailer restrictions** - Request a truck route for a vehicle with a trailer
* **Weight Restrictions** - Request a truck route for a heavy vehicle specifying axel or laden weights

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/3d880860b31ef4c5019e)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/routing.postman_collection)

## [Traffic API](traffic.postman_collection)

* **Flow using Proximity** - Request traffic flow for a circle around a defined point
* **Flow using Proximity returning Additional Attributes** - Request traffic flow information using proximity, returning shape and functional class
* **Flow using Quadkey** - Request traffic flow information using a quadkey
* **Flow with a Minimum Jam Factor** - Request traffic flow information within specified area
* **Flow within a Bounding Box** - Request traffic flow information within specified area
* **Requesting Additional Attributes** - Request traffic flow including shape and functional class information
* **Traffic Flow Availability Data** - Flow availability requests allow you to see what traffic flow coverage exists in the current Traffic API.
* **Traffic Incidents using a corridor** - Request traffic incidents for a defined route
* **Traffic Incidents via Proximity** - Request traffic incident information within specified area
* **Traffic Incidents within a Bounding Box** - Request traffic incident information within specified area
* **Traffic Map** - Request a map tile with traffic flow information
* **Traffic flow using corridor** - Request traffic flow for a defined route
* **Transparent Traffic Map** - Request a transparent tile with traffic flow information

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/1adbe0abedec53e48979)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/traffic.postman_collection)

## [Venue Maps](venue-maps.postman_collection)

* **Base64 Encoded Map Tiles** - Request a base64 encoded map tile and associated room definitions with a single request
* **Full Venue Model** - Request extended details of places found within a venue
* **Obtain Signature**  - Request authentication credentials
* **Places within a Venue** - Request a list of the places within a venue
* **Room Definitions** - Request a list of the name and shape of rooms found within a single venue map tile
* **Venue Clusters within a Bounding Box** - Request an overview of the number venues across a large area
* **Venue Map Tile** - Request an individual venue map tile
* **Venues within a Bounding Box** - Request a list of venues found within a defined area

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/00f105c5cd47b15f0f08)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/venue-maps.postman_collection)

## [Weather API](weather.postman_collection)

* **Changing from the Metric System** - Request temperatures in Fahrenheit and wind speeds in mph
* **Hourly Forecast** - Request an hour-by-hour seven day weather forecast
* **Extended Seven Day Forecast**  - Request a full seven day weather forecast
* **Multi-Language Support** - Request current weather conditions in a foreign language
* **Seven Day Forecast** - Request a simplified seven day weather forecast
* **Severe Weather Alerts** - Request severe weather alerts around a city
* **Sunrise and Sunset**  - Request information on when the sun and moon will rise and set
* **Weather Conditions at a specified Latitude and Longitude** - Request current weather conditions using latitude and longitude
* **Weather Conditions for a City**  - Request current weather observations around a named location
* **Weather Conditions using Zip Codes**  - Request current weather conditions using a US Zip Codes

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/98256a1ee83071c5bbb7)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/weather.postman_collection)

# Platform Extensions

The **HERE Platform Extensions** enable developers to further enrich their HERE enabled applications by providing access to additional data sets and functionalities, currently not available through HERE Platform services, which are tailored to specific use cases. Developers can use the Platform Extensions to add more capabilities to the service results received from HERE Platform services. They can only be used as add-ons to HERE Platform Services.

> Documentation on these APIs can be found on the [developer.here.com portal](https://developer.here.com/platform-extensions).

## [Custom Location Extension API](location-custom.postman_collection)

* **Filtering by Custom Attributes** - Request a list of user-defined locations based on their attribute values
* **Filtering by both Custom Attributes and Area** - Request a list of user-defined locations within a defined area that match specific attributes
* **Find Locations along a pre-defined Route** - Request a list of user-defined locations along a pre-defined route
* **Find Locations using Corridor** - Request a list of user-defined locations near to a given corridor
* **Find Locations using Proximity** - Request a list of user-defined locations within a circle around a fixed point
* **Find Locations within a Bounding Box** - Request a list of user-defined locations within a defined area
* **Find the Five Nearest Locations** - Request a list of user-defined locations within a circle around a fixed point

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/cc3ab14488a6554821e3)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/location-custom.postman_collection)

## [Platform Data Extension API](platform-data.postman_collection)

* **Available Attributes** - Request which map data layers contain which attributes
* **Available Attributes within a Map Data Layer** - Request which attributes are available within a specified map data layer
* **Available Map Data Layers** - Request which data layers can be accessed within a specified map region and release
* **Map Data Availability and Freshness** - Request the release date and area covered by each available map region
* **Platform Data** - Request data from a specific data layer about a specified location
* **Platform Static Data** - Request enumerated content from a static data table

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/4dce366199ba57ae2c90)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/platform-data.postman_collection)

## [Route Match Extension API](route-match.postman_collection)

* **Match GPX Data to a Route** - Request a set of linkIds that match a GPX trace

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/8398d82324a1f5b60d57)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/route-match.postman_collection)


## [Waypoint Sequence Extension API](waypoints-sequence.postman_collection)

* **Waypoint Sequence for a Truck**  - Request an ordered list of destinations for the shortest truck journey
* **Waypoint Sequence for Hazardous Materials** - Request an ordered list of destinations for a truck carrying hazardous materials
* **Waypoint Sequence for a Car** - Request an ordered list of destinations for the quickest car journey
* **Waypoint Sequence for a Truck with Trailer** - Request an ordered list of destinations for a truck with trailer

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/c63afbf5dec85dff125a)  [![Download Collection](https://heremaps.github.io/postman-collections/img/download.svg)](../../raw/master/waypoints-sequence.postman_collection)
