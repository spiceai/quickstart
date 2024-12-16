# spiceai/quickstart

```shell
spice add spiceai/quickstart
```

or

```shell
spice connect spiceai/quickstart
```

## Datasets

### `taxi_trips`

| table_catalog | table_schema | table_name | column_name           | data_type                    | is_nullable |
|---------------|--------------|------------|-----------------------|------------------------------|-------------|
| spice         | public       | taxi_trips | VendorID              | Int32                        | YES         |
| spice         | public       | taxi_trips | tpep_pickup_datetime  | Timestamp(Microsecond, None) | YES         |
| spice         | public       | taxi_trips | tpep_dropoff_datetime | Timestamp(Microsecond, None) | YES         |
| spice         | public       | taxi_trips | passenger_count       | Int64                        | YES         |
| spice         | public       | taxi_trips | trip_distance         | Float64                      | YES         |
| spice         | public       | taxi_trips | RatecodeID            | Int64                        | YES         |
| spice         | public       | taxi_trips | store_and_fwd_flag    | Utf8View                     | YES         |
| spice         | public       | taxi_trips | PULocationID          | Int32                        | YES         |
| spice         | public       | taxi_trips | DOLocationID          | Int32                        | YES         |
| spice         | public       | taxi_trips | payment_type          | Int64                        | YES         |
| spice         | public       | taxi_trips | fare_amount           | Float64                      | YES         |
| spice         | public       | taxi_trips | extra                 | Float64                      | YES         |
| spice         | public       | taxi_trips | mta_tax               | Float64                      | YES         |
| spice         | public       | taxi_trips | tip_amount            | Float64                      | YES         |
| spice         | public       | taxi_trips | tolls_amount          | Float64                      | YES         |
| spice         | public       | taxi_trips | improvement_surcharge | Float64                      | YES         |
| spice         | public       | taxi_trips | total_amount          | Float64                      | YES         |
| spice         | public       | taxi_trips | congestion_surcharge  | Float64                      | YES         |
| spice         | public       | taxi_trips | Airport_fee           | Float64                      | YES         |


**Example**

```sql
SELECT * FROM taxi_trips LIMIT 10;
```

| VendorID | tpep_pickup_datetime | tpep_dropoff_datetime | passenger_count | trip_distance | RatecodeID | store_and_fwd_flag | PULocationID | DOLocationID | payment_type | fare_amount | extra | mta_tax | tip_amount | tolls_amount | improvement_surcharge | total_amount | congestion_surcharge | Airport_fee |
|----------|----------------------|-----------------------|-----------------|---------------|------------|--------------------|--------------|--------------|--------------|-------------|-------|---------|------------|--------------|-----------------------|--------------|----------------------|-------------|
| 2        | 2024-01-17T13:42:19  | 2024-01-17T13:59:08   | 1               | 4.99          | 1          | N                  | 170          | 261          | 1            | 24.0        | 0.0   | 0.5     | 3.0        | 0.0          | 1.0                   | 31.0         | 2.5                  | 0.0         |
| 1        | 2024-01-17T13:43:35  | 2024-01-17T13:56:06   | 1               | 1.2           | 1          | N                  | 158          | 186          | 1            | 11.4        | 2.5   | 0.5     | 3.05       | 0.0          | 1.0                   | 18.45        | 2.5                  | 0.0         |
| 2        | 2024-01-17T13:09:15  | 2024-01-17T13:31:44   | 1               | 1.57          | 1          | N                  | 161          | 236          | 1            | 19.8        | 0.0   | 0.5     | 7.14       | 0.0          | 1.0                   | 30.94        | 2.5                  | 0.0         |
| 2        | 2024-01-17T13:42:54  | 2024-01-17T13:55:28   | 1               | 1.15          | 1          | N                  | 236          | 163          | 1            | 12.1        | 0.0   | 0.5     | 3.22       | 0.0          | 1.0                   | 19.32        | 2.5                  | 0.0         |
| 2        | 2024-01-17T13:05:24  | 2024-01-17T13:18:38   | 1               | 0.48          | 1          | N                  | 234          | 107          | 1            | 12.1        | 0.0   | 0.5     | 3.22       | 0.0          | 1.0                   | 19.32        | 2.5                  | 0.0         |
| 2        | 2024-01-17T13:31:24  | 2024-01-17T14:23:19   | 1               | 17.99         | 2          | N                  | 132          | 107          | 1            | 70.0        | 0.0   | 0.5     | 20.23      | 6.94         | 1.0                   | 102.92       | 2.5                  | 1.75        |
| 2        | 2024-01-17T13:41:12  | 2024-01-17T14:06:54   | 1               | 3.45          | 1          | N                  | 237          | 113          | 1            | 23.3        | 0.0   | 0.5     | 3.0        | 0.0          | 1.0                   | 30.3         | 2.5                  | 0.0         |
| 2        | 2024-01-17T13:31:21  | 2024-01-17T13:47:00   | 1               | 0.57          | 1          | N                  | 163          | 162          | 4            | -13.5       | 0.0   | -0.5    | 0.0        | 0.0          | -1.0                  | -17.5        | -2.5                 | 0.0         |
| 2        | 2024-01-17T13:31:21  | 2024-01-17T13:47:00   | 1               | 0.57          | 1          | N                  | 163          | 229          | 4            | 13.5        | 0.0   | 0.5     | 0.0        | 0.0          | 1.0                   | 17.5         | 2.5                  | 0.0         |
| 2        | 2024-01-17T13:59:41  | 2024-01-17T14:19:06   | 1               | 5.04          | 1          | N                  | 170          | 87           | 1            | 26.8        | 0.0   | 0.5     | 6.16       | 0.0          | 1.0                   | 36.96        | 2.5                  | 0.0         |
