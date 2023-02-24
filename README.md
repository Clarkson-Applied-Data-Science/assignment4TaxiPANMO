# assignment4TaxiPANMO
 ### Question 1). What datetime range does your data cover?  How many rows are there total?
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

### Question 3). Give some sample data for each field.
 ```
 +--------------------+----------------------------------+
| Field Name         |           Sample Data            |
+--------------------+----------------------------------+
| dropoff_datetime   |       2013-01-01 15:18:10        |
| dropoff_latitude   |            40.751171             |
| dropoff_longitude  |            -73.989838            |
| hack_license       | BA96DE419E711691B9445D6A6307C170 |
| medallion          | 89D227B655E5C82AECF13C3F540D4CF4 |
| passenger_count    |                4                 |
| pickup_datetime    |       2013-01-01 15:11:48        |
| pickup_latitude    |            40.757977             |
| pickup_longitude   |            -73.978165            |
| rate_code          |                1                 |
| store_and_fwd_flag |                N                 |
| trip_distance      |               1.00               |
| trip_time_in_secs  |               382                |
| vendor_id          |               CMT                |
+--------------------+----------------------------------+
 ```

### Question 4). What MySQL data types / len would you need to store each of the fields?
*int(xx), varchar(xx),date,datetime,bool, decimal(m,d)*

 ```
 +--------------------+--------------+
|    Column Name     |  Data Type   |
+--------------------+--------------+
|     medallion      | VARCHAR(32)  |
|    hack_license    | VARCHAR(32)  |
|     vendor_id      |  VARCHAR(3)  |
|     rate_code      |   SMALLINT   |
| store_and_fwd_flag |   BOOLEAN    |
|  pickup_datetime   |   DATETIME   |
|  dropoff_datetime  |   DATETIME   |
|  passenger_count   |   SMALLINT   |
| trip_time_in_secs  |     INT      |
|   trip_distance    | DECIMAL(4,2) |
|  pickup_longitude  | DECIMAL(9,6) |
|  pickup_latitude   | DECIMAL(8,6) |
| dropoff_longitude  | DECIMAL(9,6) |
|  dropoff_latitude  | DECIMAL(8,6) |
+--------------------+--------------+
 ```

### Question 5). What is the geographic range of your data (min/max - X/Y)?
*Plot this (approximately on a map)*

 ```
Geographic range of the data (min longitude, min latitude) - (max longitude, max latitude):
((-179.36124, -39.762348), (112.40418, 83.516693))
 ```
