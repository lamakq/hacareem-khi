### Execute the publisher using the following command:

`java -jar publisher.jar <CSV file path> <consumer endpoint>`


**Example:**

`java -jar publisher.jar C:\Users\x\Desktop\rides.csv http://localhost:8080`


## Sample POST request / JSON:

```
{"userId":"358a71abf8","rideId":"4552b7a9c1884cf3c75eec2dc74aa140","pickUpTime":1472577534,"pickup":{"display":"Cosmopolitan - Main E Street - Block 4, Clifton - Karachi","latitude":24.8042,"longitude":67.0329,"geohash":"tkrtj77yej8w"},"dropoff":{"display":"Florida Homes Apartment - Defence Housing Authority -  - Sindh","latitude":24.797,"longitude":67.041,"geohash":"tkrtjd1v1pf4"}}
```

## Data types:

```
userId - UUID (String)
rideId UUID (String)
pickUpTime - Epoch time in seconds (Long)
pickup.display - (String)
pickup.latitude - (Float)
pickup.longitude - (Float)
pickup.geohash - (String)
dropoff.display - (String)
dropoff.latitude - (Float)
dropoff.longitude - (Float)
dropoff.geohash - (String)
```

## Timeout:

The publisher will allow 2 seconds per request before timing out.
