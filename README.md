# assignment4TaxiPANMO
 ### Question 1. What datetime range does your data cover?  How many rows are there total?
 ```
 Date range: 2013-01-01 00:00:00 to 2013-01-31 23:59:59
Total rows: 14776616
 ```

 ### Question 2a). What are the field names?
 ```
 ['medallion', 'hack_license', 'vendor_id', 'rate_code', 'store_and_fwd_flag', 'pickup_datetime', 'dropoff_datetime', 'passenger_count', 'trip_time_in_secs', 'trip_distance', 'pickup_longitude', 'pickup_latitude', 'dropoff_longitude', 'dropoff_latitude']
 ```
 
 ### Question 2b). Give descriptions for each field.
 ```
 Field Names and Descriptions:
+--------------------+-------------------------------------------------------------------------------+
|     Field Name     |                                  Description                                  |
+--------------------+-------------------------------------------------------------------------------+
|     medallion      |                         An identifier for the taxi cab                        |
|    hack_license    |                       An identifier for the taxi driver                       |
|     vendor_id      |             An identifier for the vendor that provided the record             |
|     rate_code      |    The rate code for the trip, as defined in the vendor's operating region    |
| store_and_fwd_flag |  Indicates whether the trip record was held in vehicle memory before sending  |
|  pickup_datetime   |             The date and time when the passenger(s) were picked up            |
|  dropoff_datetime  |            The date and time when the passenger(s) were dropped off           |
|  passenger_count   |                    The number of passengers in the vehicle                    |
| trip_time_in_secs  |               The time in seconds between the pickup and dropoff              |
|   trip_distance    | The distance of the trip in miles (the unit of measure for distance may vary) |
|  pickup_longitude  |         The longitude coordinate where the passenger(s) were picked up        |
|  pickup_latitude   |         The latitude coordinate where the passenger(s) were picked up         |
| dropoff_longitude  |        The longitude coordinate where the passenger(s) were dropped off       |
|  dropoff_latitude  |        The latitude coordinate where the passenger(s) were dropped off        |
+--------------------+-------------------------------------------------------------------------------+
 ```
