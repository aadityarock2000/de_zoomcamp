ANSWERS [code to the week 1 questions] :

Select count(*) from yellow_taxi_trips 
where tpep_pickup_datetime >= '2021-01-15%' AND
Tpep_pickup_datetime < '2021-01-16%';


SELECT * from yellow_taxi_trips
where tpep_pickup_datetime >= '2021-01-01' AND
 tpep_pickup_datetime <= '2021-01-31'
 ORDER BY TIP_AMOUNT DESC LIMIT 1;

 SELECT "PULocationID", COUNT(*) from yellow_taxi_trips
where tpep_pickup_datetime >= '2021-01-14' AND
 tpep_pickup_datetime < '2021-01-15'
 GROUP BY "PULocationID"
 ORDER BY count(*) DESC;

 SELECT "PULocationID","DOLocationID",AVG(total_amount)
from yellow_taxi_trips
GROUP BY "PULocationID","DOLocationID"
ORDER BY AVG(total_amount) DESC;
