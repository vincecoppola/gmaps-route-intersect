# Google Maps Polygon-Route Intersect
Determines the point where a route (polyline) exits a given polygon and returns both the in-polygon distance as well as the out-of-polygon distance. This is accomplished by iterating over each coordinate pair in a polyline and passing each pair to a function that determines whether or not the point lies within a given polygon. Once the function returns 'False', you've roughly discovered the point of intersect.

Useful for determining region-specific mileages along a route. This specific example determines the cost of medical transportation once a trip crosses the King County border. A live version can be seen [here](http://outofcounty.com).
