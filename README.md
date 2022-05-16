# SOQL-best-examples-
```
```
__FIND LEAD BASED ON DISTANCE__
```
  SELECT Id, Name, Address
  FROM Lead
  WHERE DISTANCE(Address, GEOLOCATION(37.775,-122.418), 'mi') < 20 
  ORDER BY DISTANCE(Address, GEOLOCATION(37.775,-122.418), 'mi')
  LIMIT 10
```
